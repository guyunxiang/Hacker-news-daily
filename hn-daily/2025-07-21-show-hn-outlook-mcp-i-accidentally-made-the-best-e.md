# Show HN: Outlook MCP – I accidentally made the best email assistant

**Posted by Norcim133 on 2025-07-21**

I couldn't understand the hype around MCP, so I decided to build a simple server for Outlook (requires admin in Azure).

For the implementation, I used a Python MCP SDK: [https://github.com/modelcontextprotocol/python-sdk](https://github.com/modelcontextprotocol/python-sdk)

I'm not a fast developer, but in just two days, I had Claude Desktop filing and responding to emails more effectively than any assistant I've used before—human or AI. This wasn't due to my skill; I was mainly wrapping MSGraph calls in the same `@mcp.tool` decorator repeatedly.

In fact, I spent more time fiddling with MSGraph authentication and API calls than on the MCP server itself.

**Workflow Example:**  
Today, I simply tell Claude to "sort my inbox," and it handles everything—from filing emails, creating folders, writing responses, scheduling meetings, to flagging actions.

### Key Takeaways About MCP

1. **Fastest time-to-capability:** It was the quickest I've become productive with any software build.  
2. **Human-like operation:** It felt truly "human-capable" in a way I haven't seen with typical agentic workflows—it just worked.  
3. **Nuances matter:** How you "architect" your tool signatures significantly impacts results. For example, I named one parameter `html_code_mail_body` to prevent Claude from defaulting to plaintext emails.  
4. **Build simple, cohesive tools:** It's better to create small, highly focused, atomic tools and let the LLM combine them for complex tasks.  
5. **Ease of building:** The simplicity suggests that eventually, all companies will launch official MCP servers.

### Overall Thoughts

MCP offers a stark alternative to traditional "agentic workflows." Typically, such workflows involve tightly coupled steps, making them rigid and fragile—sometimes leading to "RPA smells." 

MCP embodies the classic dependency inversion principle: the LLM becomes an abstraction layer that can self-orchestrate using any number of tools, in any order, based on the task at hand. This approach enables flexible, resilient automation.