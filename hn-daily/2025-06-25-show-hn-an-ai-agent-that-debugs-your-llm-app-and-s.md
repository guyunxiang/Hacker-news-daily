# Show HN: An AI agent that debugs your LLM app and submits pull requests

**Posted by yuto_1192 on 2025-06-25**

Hi HN,

I built Kaizen Agent, an open-source CLI tool that acts like an AI QA engineer for your LLM applications and agents.

It helps catch broken behavior, apply fixes automatically, and open a pull request — all in one workflow.

## What it does

- Runs test inputs with expected outputs  
- If a test fails, it analyzes the failure  
- Applies prompt and code fixes  
- Re-runs tests until they pass  
- Submits a GitHub pull request with the fix

## Why I built it

I got tired of manually debugging and iterating while developing multi-step LLM agents. Writing test cases, checking outputs, tweaking prompts, and rerunning — it was all too repetitive. This tool automates that loop.

## Try it

GitHub: [https://github.com/Kaizen-agent/kaizen-agent](https://github.com/Kaizen-agent/kaizen-agent)

Would love feedback — especially from anyone building agents, LLM tools, or testing frameworks. I'm curious how others are approaching evaluation, brittleness, and automation in this space.