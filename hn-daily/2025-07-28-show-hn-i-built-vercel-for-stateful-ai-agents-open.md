# Show HN: I Built "Vercel for Stateful AI Agents" – open-source, cost-efficient

**Posted by cyw on 2025-07-28**

---

**TL;DR:**  
Like Vercel, but for stateful AI agents. Deploy your container and instantly get an agent with persistent memory, auto-recovery, and a live API endpoint—zero infrastructure work required.

---

Hi HN, I’m Cyw, the founder of [Agentainer](https://agentainer.io/), a platform designed to deploy and manage long-running AI agents with zero DevOps. We’ve just launched the first open-source version: **Agentainer Lab** on [GitHub](https://github.com/oso95/Agentainer-lab).

### Background  
Most modern infrastructure—Lambda, Cloud Run, Kubernetes—are optimized for short-lived, stateless workloads. But AI agents are inherently different. They’re long-running processes with memory, history, and evolving state. Running them reliably in production often involves assembling various services for volume mounts, retry queues, crash recovery, and gateways, making the setup complex.

### What I Built  
To simplify this, I created an infrastructure layer that treats agents as durable services from day one—no YAML configs, no juggling multiple services. Just provide a Docker image or Dockerfile, and Agentainer manages the rest. Think of it as a Vercel-like solution for AI agents.

### Features  
- Each agent runs in its own isolated container  
- Persistent volume mounts for memory and state  
- Crash recovery and queued request replay  
- Automatic restart if an agent crashes mid-task  
- A clean proxy endpoint, so network and port management are out of the box  
- Checkpointing to ensure progress isn’t lost (more details in [RESILIENT_AGENTS.md](https://github.com/oso95/Agentainer-lab/blob/main/docs/RESILIENT_AGENTS.md))

### How It Works  
Everything is CLI-first and API-accessible. I built this initially so my own coding agent could manage infrastructure without repeating shell commands. You can deploy, restart, or remove agents programmatically—both in development and production environments.

### Cost and Performance  
For workloads like agentic backends with frequent requests or persistent states, this architecture can cut cloud costs by 30-40%, reducing per-request billing and infrastructure sprawl.

### Future Roadmap  
Currently focused on local development and self-hosting, but plans include observability, audit logs, backup/restore, and full auto-scaling to unlock its full potential.  

You can sign up for early access on our [website](https://agentainer.io). We’ll only send one email when the production version is live, then delete your email.

### Links  
- GitHub: [Agentainer Lab](https://github.com/oso95/Agentainer-lab)  
- Platform: [agentainer.io](https://agentainer.io)  

I’d love to hear feedback from others working on LLM agents or deploying stateful workloads. What’s your current setup? Do you think this could help you?