# Open-source control plane for Docker MCP Gateways?

**Posted by GeneBordegaray on 2025-08-08**

---

**TL;DR:** I built a control plane to manage multiple Docker MCP Gateways with guardrails like SSO/RBAC, policy-as-code, audit, and cost management. I'm considering open-sourcing the core components. Would this be useful to you? What features would you need to adopt it?

---

## What it does today

- **Fleet orchestration:** Provisioning and scaling multiple Docker MCP Gateways per organization/environment, with health checks and zero-downtime updates.  
- **Identity & access:** Supports SSO/OIDC, SCIM, service accounts, and RBAC at organization, environment, and gateway levels.  
- **Policy-as-code:** Implements guardrails for deploying applications, egress restrictions, rate limits, quotas, and approval workflows.  
- **Secrets & keys:** KMS-backed secret injection with rotation, avoiding raw environment variables.  
- **Audit & compliance:** Immutable logs for authentication, configuration, and tool calls; exportable evidence complying with SOC2/ISO standards.  
- **Observability & cost management:** Monitors latency (p95/p99), error budgets, and provides usage and cost allocation per tenant.  
- **Hardening:** Builds with rootless and read-only containers, minimal privileges, mutual TLS, and IP allowlists.

---

## What’s in scope (Prototype proposals for open-sourcing)

- Agents and operators that supervise gateways, along with Terraform and Helm modules.  
- Baseline policy packs (OPA/Rego) for common guardrails.  
- Dashboards and exporters (Prometheus/Grafana) for health, latency, and usage metrics.  
- CLI and API for provisioning, configuration, rotation, and audit export. (Considering licenses like Apache-2.0 or AGPL—open to input.)

---

## What remains managed (if there is a cloud edition)

- Multi-tenant hosted control plane and UI with SSO/SCIM integration.  
- Compliance automations, anomaly detection, and cost/chargeback analytics.

---

## I’d love your feedback

- Would you prefer to self-host this, or only consider a SaaS solution? Why?  
- Which integrations are essential: Kubernetes, ECS, Nomad, bare metal?  
- What license would you prefer (Apache/MIT vs AGPL), and why?  
- Deal-breakers for adoption: security concerns, data residency, migration paths, etc.  
- What’s missing for day-1: backups/disaster recovery, blue-green deployments, per-tenant budgets, or other features?  
- If the core is open source, would your team contribute policies and integrations?

---

## Who I think this helps

- Platform and DevOps teams managing 5 to 50 MCP servers across multiple environments.  
- Security and compliance teams needing auditability and policy guardrails out of the box.  
- Startups aiming to avoid building yet another custom control plane for Docker MCP.

---