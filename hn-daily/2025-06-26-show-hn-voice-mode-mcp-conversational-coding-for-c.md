# Show HN: Voice-Mode MCP – Conversational Coding for Claude Code, Gemini CLI

**Posted by mike-bailey on 2025-06-26**

When I heard about Google's clone of Claude Code this morning, I tried it out with my two-week-old MCP server. Instantly, I was able to have a two-way voice conversation with it. Gemini seemed a bit confused by this. :-)

Here's a short demo: [https://youtu.be/HC6BGxjCVnM?feature=shared&t=36](https://youtu.be/HC6BGxjCVnM?feature=shared&t=36)

## About Voice-Mode MCP

It's an open-source (FOSS) MCP server I created a couple of weeks ago. You can find it here:

- [getvoicemode.com](https://getvoicemode.com)
- [GitHub Repository](https://github.com/mbailey/voicemode)

## Installation (via `~/.gemini/settings.json`)

```json
{
  "theme": "Dracula",
  "selectedAuthType": "oauth-personal",
  "mcpServers": {
    "voice-mode": {
      "command": "uvx",
      "args": [
        "voice-mode"
      ]
    }
  }
}
```