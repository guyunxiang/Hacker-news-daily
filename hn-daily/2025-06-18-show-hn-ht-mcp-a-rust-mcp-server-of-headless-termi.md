# Show HN: ht-mcp – a Rust MCP server of headless terminal for agents

**Posted by alphag33k on 2025-06-18**

We built a Rust MCP server that wraps the excellent headless terminal (HT)[1], making it available for agentic coding tools.

Most agentic coding tools struggle with blocking, interactive terminal tools like boilerplate generators, infrastructure CLIs, etc. This is because many existing CLI development tools are designed for humans and require interactive input. Our solution enables agentic coding tools (such as Claude Code, Cursor, Memex, etc.) to "see" and "interact" with terminals exactly as humans do.

In our demo video [2], you'll see it operating vim/emacs just as a human would—selecting options, navigating menus, and modifying text in real-time. This capability is crucial for AI coding assistants that need to work seamlessly with tools meant for human interaction.

Our initial proof of concept was a MCP server in TypeScript wrapping the HT (Rust) binary. It worked so well that we decided to streamline the implementation, making it more compact and easy to install. 

Using Rust and the MCP Rust SDK proved to be highly advantageous, resulting in significant performance improvements:
- 40x faster startup time (~50ms vs. ~2s)
- 70% lower memory usage (~15MB vs. ~50MB)
- Single 3MB binary compared to ~200MB of Node.js dependencies
- No subprocess overhead or external dependencies

As Andy Konwinski notes [4], *"Terminals are one of the oldest and most prolific UI frameworks in all of computing. And they are stateful."* Without HT, an agent struggles to manage this state directly, but with ht-mcp, an agent can observe and interact with the terminal just as a human would.

This is an early release, and we would love to hear if you find it useful.

Here are some resources:
- Demo using ht-mcp with Claude Code and Memex (our desktop agent coding tool):  
  [https://github.com/andyk/ht](https://github.com/andyk/ht) ([Andy Konwinski](https://github.com/andyk))
- Demo video:  
  [https://github.com/user-attachments/assets/e70a3240-77f5-4ef2-953b-202b310dbf74](https://github.com/user-attachments/assets/e70a3240-77f5-4ef2-953b-202b310dbf74)
- Memex demo details (assets):  
  [https://github.com/user-attachments/assets/6a1b6e76-5d5c-4ba4-87ee-70a31f0bc4ce](https://github.com/user-attachments/assets/6a1b6e76-5d5c-4ba4-87ee-70a31f0bc4ce)
- Hacker News discussion:  
  [https://news.ycombinator.com/item?id=40552257](https://news.ycombinator.com/item?id=40552257)

**Installation:**
```bash
brew tap memextech/tap && brew install ht-mcp
```