# Show HN: Did that MCP Server leak your database?

**Posted by anand-tan on 2025-07-08**

Tansive is an open-source platform designed to help teams securely integrate AI agents into real workflows.

I posted about Tansive this morning on Show HN, but didn't receive any responses. So, I’m shamelessly riding the recent hype because it’s the reason I built Tansive.

I'm impressed with what AI agents can do, especially for routine tasks where human effort is high and errors are frequent. However, deploying these agents in production presents challenges:

- How do you prevent an agent or its tools from leaking sensitive data?  
- How can you audit an agent’s actions when something goes wrong?  
- When a workflow yields undesired results, was it due to a bug, incorrect prompt, runaway agent, or prompt injection attack?  
- How can you verify that an agent didn’t access Alice’s records when responding to Bob’s health question?  
- How do you ensure agents comply with existing security policies and regulations?

While dramatic examples often come from DevOps failures, most business processes automation requires controls and guardrails. That’s what Tansive aims to address.

## What Tansive enables

- **Runtime focus**: Instead of just building agents, Tansive emphasizes their runtime execution — tracking what they access, tools they call, actions they take, and who triggered them.  
- **Declarative Catalog**: A YAML-based repository of agents, tools, context, and resources, partitioned by environment and segmented by namespaces, allowing for policy rule definitions (GitOps-friendly).  
- **Runtime policy enforcement**: Enforce constraints like “this agent can restart pods only in dev” or “a finance agent can only reconcile certain accounts.”  
- **Session pinning**: Transform or restrict sensitive data via user-defined functions, e.g., “Bob’s session cannot access Alice’s data” or injecting WHERE clauses in SQL queries based on feature flags.  
- **Tamper-evident, hash-linked logs**: Ensuring audit trails are reliable.  
- **Language-agnostic tools**: Write tools in any language your team uses—Go, Java, JavaScript, Bash—to integrate agent workflows into your systems.

### Demo video

[Watch here](https://vimeo.com/1099257866?share=copy) — It shows policy enforcement and session pinning in action, such as:

- An agent restarting pods only in development, not production.  
- A health bot pinned to a specific patient’s ID cannot access another patient’s records.

## Building for adoption

I’ve thought a lot about how to get teams to adopt AI automation. The main obstacle is that most tools require writing in Python using specific SDKs, which isn’t practical for teams working in other languages.

To solve this, I envisioned a generic agent that manages LLMs and tool calls, with functionality in language-agnostic interfaces. Teams can then write tools in whatever language they already use—Go, Java, JavaScript, Bash—and still integrate seamlessly. This approach aligns well with existing agent frameworks.

The idea came from asking: **“How can I adapt my existing scripts to work with LLM inputs?”**

## Why this matters

AI agents are powerful, but handling security, compliance, and predictable behavior remains critical for their widespread adoption. Tansive aims to fill that gap.

Currently in early alpha (v0.1.0), it’s sized for preview purposes but still functional enough to try in real workflows outside production. I plan to focus on solving straightforward but urgent problems first, then expand from there.

I’d love feedback from anyone interested in infrastructure, AI agent security, integration, or compliance — or just curious to explore it.

Happy to answer questions and hear your thoughts!

## Links

- **GitHub**: [https://github.com/tansive/tansive](https://github.com/tansive/tansive)  
- **Docs**: [https://docs.tansive.io](https://docs.tansive.io)