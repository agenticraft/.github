<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="readme-banner.svg">
  <source media="(prefers-color-scheme: light)" srcset="readme-banner.svg">
  <img alt="AgentiCraft" src="readme-banner.svg" width="100%">
</picture>

The production infrastructure layer for AI agents. Build, deploy, and scale multi-agent systems with a high-performance Rust data plane, formal verification, and enterprise-grade governance.

---

`Rust Data Plane` · `100+ Patterns` · `60+ Mesh Services` · `17 LLM Providers` · `Formal Verification` · `MCP + A2A`

[![Website](https://img.shields.io/badge/agenticraft.ai-0D9488?style=flat-square&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA2NCA2NCIgd2lkdGg9IjY0IiBoZWlnaHQ9IjY0Ij48cG9seWdvbiBwb2ludHM9IjM5LDcgNTMsMjQgMzYsMjgiIGZpbGw9IndoaXRlIiBvcGFjaXR5PSIwLjg1Ii8+PHBvbHlnb24gcG9pbnRzPSIzOSw3IDEyLDMzIDM2LDI4IiBmaWxsPSJ3aGl0ZSIgb3BhY2l0eT0iMC43Ii8+PHBvbHlnb24gcG9pbnRzPSI1MywyNCA0Nyw0OSAzNiwyOCIgZmlsbD0id2hpdGUiIG9wYWNpdHk9IjAuNzUiLz48cG9seWdvbiBwb2ludHM9IjQ3LDQ5IDIyLDU0IDM2LDI4IiBmaWxsPSJ3aGl0ZSIgb3BhY2l0eT0iMC45Ii8+PHBvbHlnb24gcG9pbnRzPSIyMiw1NCAxMiwzMyAzNiwyOCIgZmlsbD0id2hpdGUiIG9wYWNpdHk9IjAuOTUiLz48Y2lyY2xlIGN4PSIzOSIgY3k9IjciIHI9IjMiIGZpbGw9IndoaXRlIi8+PGNpcmNsZSBjeD0iNTMiIGN5PSIyNCIgcj0iMi44IiBmaWxsPSJ3aGl0ZSIvPjxjaXJjbGUgY3g9IjQ3IiBjeT0iNDkiIHI9IjIuOCIgZmlsbD0id2hpdGUiLz48Y2lyY2xlIGN4PSIyMiIgY3k9IjU0IiByPSIyLjgiIGZpbGw9IndoaXRlIi8+PGNpcmNsZSBjeD0iMTIiIGN5PSIzMyIgcj0iMyIgZmlsbD0id2hpdGUiLz48Y2lyY2xlIGN4PSIzNiIgY3k9IjI4IiByPSIzLjIiIGZpbGw9IndoaXRlIi8+PC9zdmc+)](https://agenticraft.ai)
[![Docs](https://img.shields.io/badge/docs-0D9488?style=flat-square&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA2NCA2NCIgd2lkdGg9IjY0IiBoZWlnaHQ9IjY0Ij48cG9seWdvbiBwb2ludHM9IjM5LDcgNTMsMjQgMzYsMjgiIGZpbGw9IndoaXRlIiBvcGFjaXR5PSIwLjg1Ii8+PHBvbHlnb24gcG9pbnRzPSIzOSw3IDEyLDMzIDM2LDI4IiBmaWxsPSJ3aGl0ZSIgb3BhY2l0eT0iMC43Ii8+PHBvbHlnb24gcG9pbnRzPSI1MywyNCA0Nyw0OSAzNiwyOCIgZmlsbD0id2hpdGUiIG9wYWNpdHk9IjAuNzUiLz48cG9seWdvbiBwb2ludHM9IjQ3LDQ5IDIyLDU0IDM2LDI4IiBmaWxsPSJ3aGl0ZSIgb3BhY2l0eT0iMC45Ii8+PHBvbHlnb24gcG9pbnRzPSIyMiw1NCAxMiwzMyAzNiwyOCIgZmlsbD0id2hpdGUiIG9wYWNpdHk9IjAuOTUiLz48Y2lyY2xlIGN4PSIzOSIgY3k9IjciIHI9IjMiIGZpbGw9IndoaXRlIi8+PGNpcmNsZSBjeD0iNTMiIGN5PSIyNCIgcj0iMi44IiBmaWxsPSJ3aGl0ZSIvPjxjaXJjbGUgY3g9IjQ3IiBjeT0iNDkiIHI9IjIuOCIgZmlsbD0id2hpdGUiLz48Y2lyY2xlIGN4PSIyMiIgY3k9IjU0IiByPSIyLjgiIGZpbGw9IndoaXRlIi8+PGNpcmNsZSBjeD0iMTIiIGN5PSIzMyIgcj0iMyIgZmlsbD0id2hpdGUiLz48Y2lyY2xlIGN4PSIzNiIgY3k9IjI4IiByPSIzLjIiIGZpbGw9IndoaXRlIi8+PC9zdmc+)](https://agenticraft.ai/docs)
[![Blog](https://img.shields.io/badge/blog-0D9488?style=flat-square&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA2NCA2NCIgd2lkdGg9IjY0IiBoZWlnaHQ9IjY0Ij48cG9seWdvbiBwb2ludHM9IjM5LDcgNTMsMjQgMzYsMjgiIGZpbGw9IndoaXRlIiBvcGFjaXR5PSIwLjg1Ii8+PHBvbHlnb24gcG9pbnRzPSIzOSw3IDEyLDMzIDM2LDI4IiBmaWxsPSJ3aGl0ZSIgb3BhY2l0eT0iMC43Ii8+PHBvbHlnb24gcG9pbnRzPSI1MywyNCA0Nyw0OSAzNiwyOCIgZmlsbD0id2hpdGUiIG9wYWNpdHk9IjAuNzUiLz48cG9seWdvbiBwb2ludHM9IjQ3LDQ5IDIyLDU0IDM2LDI4IiBmaWxsPSJ3aGl0ZSIgb3BhY2l0eT0iMC45Ii8+PHBvbHlnb24gcG9pbnRzPSIyMiw1NCAxMiwzMyAzNiwyOCIgZmlsbD0id2hpdGUiIG9wYWNpdHk9IjAuOTUiLz48Y2lyY2xlIGN4PSIzOSIgY3k9IjciIHI9IjMiIGZpbGw9IndoaXRlIi8+PGNpcmNsZSBjeD0iNTMiIGN5PSIyNCIgcj0iMi44IiBmaWxsPSJ3aGl0ZSIvPjxjaXJjbGUgY3g9IjQ3IiBjeT0iNDkiIHI9IjIuOCIgZmlsbD0id2hpdGUiLz48Y2lyY2xlIGN4PSIyMiIgY3k9IjU0IiByPSIyLjgiIGZpbGw9IndoaXRlIi8+PGNpcmNsZSBjeD0iMTIiIGN5PSIzMyIgcj0iMyIgZmlsbD0id2hpdGUiLz48Y2lyY2xlIGN4PSIzNiIgY3k9IjI4IiByPSIzLjIiIGZpbGw9IndoaXRlIi8+PC9zdmc+)](https://agenticraft.ai/blog)
[![Python](https://img.shields.io/badge/Python-3.12+-3776AB?style=flat-square&logo=python&logoColor=white)](https://python.org)

---

</div>

## The Problem

88% of AI pilots never reach production. The bottleneck isn't the models — it's the infrastructure around them. Every team that gets serious about production agents ends up building the same operational stack from scratch: observability, reliability, cost control, security, deployment.

**AgentiCraft is that stack.** One platform. One command. Any scale.

## What Makes This Different

**High-performance Rust data plane.** A 29-stage middleware pipeline processes every agent request at microsecond latency — intelligent provider routing, PII masking, budget enforcement, circuit breakers, and compliance audit trails. Policy enforcement happens in the data plane, not in Python.

**Formal verification.** Agent protocols are verified before deployment. If a coordination pattern has a deadlock or a protocol violation, you find it at compile time — not in a 3 AM incident.

**One file, any platform.** Define your entire multi-agent system in `app.yaml` — agents, topology, workflows, policies, plugins. The runtime compiles it into infrastructure and deploys it on a laptop, Docker, Kubernetes, or an edge device.

**Research-backed reliability.** In our fault tolerance experiments, mesh-coordinated agents maintained 100% task completion with zero cascade failures across all tested failure rates. Hub-and-spoke dropped to 82% at 20% failure rate and 72% at 30%. The architecture isn't theoretical — it's tested.

## Architecture

| Layer | Name | What It Does |
|-------|------|-------------|
| 0 | **Foundation** | Formal verification, session types, topology analysis |
| 1 | **Transport** | Async messaging between agents |
| 2 | **Data Plane** | Rust proxy — per-request enforcement at microsecond latency |
| 3 | **Control Plane** | 60+ mesh services — orchestration, policies, LLM management |
| 4 | **Runtime** | Universal deployment — laptop, Docker, Kubernetes, edge |
| 5 | **Developer Experience** | `craft` CLI, SDK, templates, test harness |
| 6 | **App Framework** | Declarative app manifest, plugin system, marketplace |
| 7 | **Products** | End-user applications — bots, dashboards, enterprise tools |

## Define Your System

```yaml
# app.yaml — agents, topology, workflows, policies in one file
name: research-team
agents:
  - id: researcher
    capabilities: [web_search, paper_analysis]
    models: { default: gpt-5-mini, for_analysis: gpt-5.4 }
    memory: { tiers: { hot: { backend: redis } } }
    autonomy: { level: 0.9 }

  - id: analyst
    capabilities: [data_analysis, visualization]

topology:
  connections:
    - { from: researcher, to: analyst, type: delegate }

workflows:
  - id: deep-dive
    pattern: pipeline
    steps:
      - { id: search, agent: researcher }
      - { id: analyze, agent: analyst }

policies:
  budgets: { org: { monthly_usd: 10.0 } }
  guardrails: { pii: { action: mask } }
  sla: { researcher: core, analyst: standard }
```

```bash
craft start --app app.yaml
```

## By the Numbers

- **100+ production patterns** — reasoning, coordination, workflow, resilience, RAG, safety, planning
- **60+ mesh services** with defined SLAs — security, deployment, gateway, observability, and more
- **17 LLM providers** with automatic failover — OpenAI, Anthropic, Google, Mistral, Azure OpenAI, Ollama, and 11 more
- **MCP + A2A native** — open protocols for tool integration and inter-agent communication
- **3 plugin tiers** — agent, app, and middleware plugins for extensibility without forking

## Public Libraries

| Library | Description |
|---------|-------------|
| [agenticraft-foundation](https://github.com/agenticraft/agenticraft-foundation) | Formally verified mathematical foundations for multi-agent AI coordination. Process algebra, session types, spectral topology, temporal logic. 1,165 tests, zero runtime dependencies. |

## Links

- **[Website](https://agenticraft.ai)** — platform overview and early access
- **[Blog](https://agenticraft.ai/blog)** — architecture decisions, research findings, technical deep dives
- **[Foundation Docs](https://agenticraft.ai/docs/foundation/)** — formal verification toolkit
- **Email:** hello@agenticraft.ai
