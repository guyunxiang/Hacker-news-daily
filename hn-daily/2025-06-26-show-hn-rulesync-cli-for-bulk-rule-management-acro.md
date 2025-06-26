# Show HN: rulesync – CLI for bulk rule management across multiple AI coding tools

**Posted by dyoshikawa on 2025-06-26**

There are various AI coding tools like Claude Code, Cursor, Copilot, Cline, Roo, and recently Gemini CLI. However, each of these tools has its own rule file specifications, which are not compatible with one another.

To address this, I created a CLI tool called **rulesync** that can automatically generate rule files for each AI tool from a single source. By simply creating and updating one set of Markdown files, you can manage rules across multiple platforms seamlessly. The `rulesync` package is available on npm and supports Gemini CLI as well.

### How to use rulesync

1. **Initialize rule files**

   Create your `.rulesync/<name>.md` sample files by running:

   ```bash
   npx rulesync init
   ```

   If you already have rule files (e.g., for Cursor), you can convert them:

   ```bash
   npx rulesync import --cursor
   ```

2. **Edit your rules**

   Open the `.rulesync/<name>.md` files generated and customize them as needed.

   You can add new rule templates easily:

   ```bash
   npx rulesync add {RULE_NAME}
   ```

3. **Generate rule files for your AI tools**

   Once your rules are ready, generate the rule files for the AI tools you're using:

   ```bash
   npx rulesync generate --cursor --claudecode --geminicli
   ```

Thank you.