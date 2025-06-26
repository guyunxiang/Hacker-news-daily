# The Pitfall of Open-Weight LLMs

**Posted by hiddenest on 2025-06-25**

Some startups are opting to fine-tune open-source LLMs instead of relying on proprietary models like GPT or Gemini. Sometimes they do this to specialize in a particular language, or to handle narrow tasks. However, I’ve observed a common oversight across these efforts.

By using a simple prompt (not shared here), I was able to get several "custom" LLM services to reveal their internal system prompts—such as security breach playbooks and product action lists.

For example:

- SKT A.X 4.0 (based on Qwen 2.5) disclosed internal guidelines related to a recent SKT data breach and instructions regarding compensation policies.
- Vercel’s v0 model leaked examples of actions it can generate.

**The key takeaway:** If the base model leaks, then every service built on top of it is inherently vulnerable, regardless of how much they fine-tune or customize. 

This highlights the importance of not only hardening system prompts at the service level but also improving the upstream models themselves and developing more robust defenses for open-weight LLMs. Without these measures, the foundation remains insecure, risking exposure of sensitive internal information.