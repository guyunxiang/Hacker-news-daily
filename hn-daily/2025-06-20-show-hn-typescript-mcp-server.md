# Show HN: TypeScript MCP Server

**Posted by johnwheeler on 2025-06-20**

---

Hello, everybody. I want to introduce the TypeScript MCP server I've been working on. The goal is to reduce the thrashing that happens when the LLM struggles to resolve types. It provides tools for the LLM to perform semantic analysis and editing more efficiently.

There's still a lot to do, and numerous features I want to add. I’d appreciate early feedback from the community. Currently, there's no installer available.

At this stage, I can use the server to build on itself and work with itself when integrated into Claude code.

### How to Use

1. Clone the repository.

2. From the project root, install dependencies and add the MCP:

```bash
pnpm i
claude mcp add ts tsx packages/mcp-server/src/index.ts
```

3. Run Claude:

```bash
claude
```

### GitHub Repository

[https://github.com/screencam/typescript-mcp-server](https://github.com/screencam/typescript-mcp-server)

Thanks!