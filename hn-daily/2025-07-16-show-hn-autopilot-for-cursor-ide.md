# Show HN: Autopilot for Cursor IDE

**Posted by Homo__Ludens on 2025-07-16**

I’ve always been looking for a way to communicate larger technical systems more efficiently. This includes sharing detailed information and creating a technical de-risking plan. It’s clear that large language models (LLMs) require structured data and are capable of digesting such information effectively.

To address this, I’ve built an MCP server that guides the Cursor IDE through a plan generated from an LLM-assisted pipeline: PRD → TRD → Project files tree → Implementation Plan.

Key features:
1. The entire process is integrated into one end-to-end solution.
2. The produced codebase is easy to navigate, thanks to automatically managed traceability.
3. Specification updates are reflected in tasks, ensuring the flow supports continuous evolution.

For requirements capturing and task management, I’m using gemini-2.5-pro. Support for Cloud Code and Gemini CLI is coming soon.