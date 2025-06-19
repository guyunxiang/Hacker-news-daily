# Show HN: Agentic Trust – Enterprise MCP Server Platform for Secure AI Agents

**Posted by subramanya1997 on 2025-06-18**

Hey HN! We're building Agentic Trust, a unified platform that transforms your code into production-ready MCP (Model Context Protocol) servers with built-in authentication, security, and observability.

## The Problem
As AI agents become more capable, they require secure methods to access tools and data. MCP (Anthropic's open protocol) standardizes agent-to-tool communication, but deploying MCP servers in production is complex. You need to handle authentication, rate limiting, audit logs, multi-tenancy, and ensure your agents are protected against prompt injection and other attacks.

## Our Solution
A single endpoint (agentictrust.com) that manages all your MCP servers, so you can focus on your tool logic. We take care of:
- OAuth 2.0 authentication with scoped permissions
- Rate limiting and usage analytics
- Audit trails for compliance
- Automatic versioning and routing
- Protection against prompt injection attacks

## Technical Details
We are also working on OIDC-A (OpenID Connect for Agents), a proposal to extend OIDC to support agent identity verification. It introduces claims for agent attestation, delegation chains, and capabilities. Recently, WorkOS's CEO highlighted this initiative at Identiverse.

The goal is for agents to have verifiable identities just like users. When an agent acts on a user's behalf, tracking the delegation chain is essential for security and compliance.

## Why Now
Microsoft announced support for MCP in Windows 11, and OpenAI is adopting the protocol, leading to rapid growth in MCP adoption. However, many implementations are insecure—exposed endpoints, missing authentication, vulnerable to attacks. We're here to address those security gaps.

## Links
- [Platform](https://agentictrust.com)
- [OIDC-A Proposal](https://subramanya.ai/2025/04/28/oidc-a-proposal/)
- [WorkOS article on our work](https://workos.com/blog/identity-for-ai-agents)

We’re in early access and eager for feedback from the HN community. What security concerns do you have about AI agents? How are you handling agent authentication today?