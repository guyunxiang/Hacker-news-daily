# Show HN: Visual Editor for Cursor

**Posted by kemyd on 2025-07-08**

---

Hi!

We noticed that our users extensively use Shuffle (a visual editor for developers) in conjunction with Cursor. That’s why we built the Shuffle CLI, a lightweight tool that creates a seamless bridge between Shuffle and Cursor.

With this CLI, you can:

- Sync your visual components from Shuffle directly into Cursor projects
- Automatically generate clean, editable code from your designs
- Keep your design and development workflows tightly integrated without copy-pasting or re-exporting

We built this to reduce the friction between prototyping and production. If you’re using Cursor as your IDE and Shuffle for layout and styling, this tool may be a good fit for you.

Here's how to test it quickly:

```bash
mkdir website
cd website
npx @shuffle-dev/cli get example-project .shuffle --rules=cursor
```

The project will be saved in the `.shuffle` directory. You can, for example, ask Cursor:

> *Create a Next.js app from the .shuffle directory*

In a real project, you can modify it in Shuffle and sync after changes:

```bash
npx @shuffle-dev/cli sync <project_id>
```

Then, ask Cursor again:

> *Add new pages from .shuffle to my Next.js app*

We haven’t used MCP yet. We’ve tested it, but the CLI is better at maintaining consistency in format.