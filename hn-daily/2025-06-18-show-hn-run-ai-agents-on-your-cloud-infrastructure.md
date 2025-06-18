# Show HN: Run AI Agents on your cloud infrastructure

**Posted by Ramiro on 2025-06-18**

Hi, founder of Okteto here!

We’ve been experimenting with AI agents in our workflows at Okteto. Running them locally worked at first, but quickly became painful. Managing git worktrees, multiple terminals, and juggling messy context switches slowed us down.

To address this, we built **Agent Fleets**: ephemeral, fully managed environments for AI agents, built on top of Okteto’s development platform. Each agent runs in its own containerized environment on your infrastructure, equipped with the necessary services, tools, and policies.

You can spin up agents with a single click or API call—no local setup required. Forget about git worktrees and local configurations.

The beta currently supports Sonnet 4 and OpenHands, with more models and frameworks coming soon.

This is in beta, and I’d love your feedback, feature requests, or thoughts on what you’d like to see from something like this.