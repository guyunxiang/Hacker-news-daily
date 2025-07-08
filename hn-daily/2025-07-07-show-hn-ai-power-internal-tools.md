# Show HN: AI Power Internal Tools

**Posted by DeonRob on 2025-07-07**

Hey folks,

I’ve been building Sashi — a developer tool that reads your existing codebase and lets you create AI-driven workflows out of your backend functions.

Imagine giving your ops, product, and dev teams a natural-language interface to:
- Search users from your database
- Filter and chart usage data
- Send emails or Slack messages
- ...and much more, all by just describing what they want to do

It works with TypeScript and Zod functions, automatically generates UIs, and connects to your GitHub to stay in sync.

The long-term goal is to help teams move faster without rebuilding internal tools every time they need a new dashboard or button.

Currently, Sashi supports:
- Dynamic function registration
- AI workflow planning
- Automatic UI generation (tables, charts, forms)
- GitHub function ingestion
- Secure execution via a centralized hub

It automatically installs into any Node.js/Next.js codebase with a CLI command.

If you’re curious or want to try it out, I’d love your feedback. We are looking for beta users:  
[https://www.usesashi.com](https://www.usesashi.com)

Also, I have a question that I’d appreciate your input on:  
What’s one task in your codebase you’d love to turn into a “just say it and run it” flow?  
For example, updating user roles — especially if it triggers side effects across your system — is something I encounter often.