# Show HN: Zest – AI Agents for Slack

**Posted by kakaly040390 on 2025-07-23**

Hi HN,

A few months ago, I started experimenting with building AI agents as Slack bots. What began as a fun weekend project has now become a core part of how our team works every day.

These bots live in Slack and handle complex, real-world workflows such as:

- When a new signup comes in, one of the bots enriches the lead via Apollo, drafts a personalized email, and drops it into my mailbox.
- If someone mentions a new task in any channel, the bot jumps in, asks a few clarifying questions, and creates a Linear ticket.
- Collecting customer information from Stripe during transaction failures and automatically bringing it into the Slack thread.
- Scouring the web and drafting blog posts — you could do this with ChatGPT, but doing it collaboratively in Slack creates a different experience.
- We even made the bots proactive. For example, if someone mentions sprint planning, the bot joins the conversation and asks if it should help break things down into tasks.

Initially, this felt like mere automation. But what surprised us was how collaborative it became. Since the agents live in public Slack threads, teammates observed how others interacted with them — analyzing prompts, tagging bots, correcting outputs. It turned into a lightweight, social learning system. Everyone improved their prompting skills and thinking in “agentic workflows” simply by participating in the conversations.

We also built a lightweight dashboard to enable team members to spin up and deploy new bots, manage access, customize behaviors, and attach tools.

**Demo:**  
Here's a short video showcasing one of our bots in action — it self-corrects, navigates tools like Linear and internal APIs, and completes tasks end-to-end.

**Stack:**  
- Vercel AI SDK  
- axllm.dev (DSPy for TypeScript) for the agentic loop  
- Composio for tool integrations

We are currently running a closed beta for anyone interested in deploying Slack bots as agents. If you'd like to join, sign up for our waitlist: [https://heyzest.ai/](https://heyzest.ai/)