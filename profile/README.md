# AgentiCraft

**Enterprise-grade agentic AI platform**

Build, deploy, and scale AI agents with production-ready infrastructure.

---

## What is AgentiCraft?

AgentiCraft is a full-stack platform for building production-ready AI agents. It provides both agent logic (patterns, coordination) and enterprise infrastructure (security, observability, multi-tenancy) in one unified platform.

## Platform Overview

| Component | Details |
| --------- | ------- |
| **LLM Providers** | 18 providers (OpenAI, Anthropic, Google, Mistral, Groq, and more) |
| **Agent Patterns** | 214+ patterns across 17 categories |
| **Mesh Services** | 45+ services with defined SLAs |
| **Security** | 9-layer defense-in-depth architecture |
| **Protocols** | Native MCP, A2A, and ANP support |

## Key Capabilities

### Agent Patterns (214+)

- **Cognitive**: Chain-of-Thought, Tree-of-Thoughts, ReAct, Reflection
- **Coordination**: Consensus, Swarm, Gossip, Team
- **Workflow**: Pipeline, StateMachine, DAG, HITL
- **Resilience**: Circuit Breaker, Retry, Saga, Bulkhead
- **RAG**: GraphRAG, HybridRAG, AdaptiveRAG
- **Safety**: Constitutional, Adversarial, Guardrails

### Mesh Services (45+)

| Tier | SLA | Services |
| ---- | --- | -------- |
| Critical | 99.99% | Security, Discovery, Observability |
| Core | 99.95% | Agents, Events, Orchestration |
| Platform | 99.9% | LLM, Data, MCP |
| Standard | 99.5% | A2A, Streaming, Patterns |

### Enterprise Features

- Multi-tenancy with per-tenant quotas
- SOC2, GDPR, HIPAA, ISO27001 compliance controls
- OpenTelemetry distributed tracing
- Cost tracking and budget management

## Protocol Support

| Protocol | Purpose | What It Enables |
| -------- | ------- | --------------- |
| **MCP** | Agent ↔ Tools | Tool discovery, context sharing, resource management |
| **A2A** | Agent ↔ Agent | Task delegation, coordination, state sync |
| **ANP** | Agent ↔ External Networks | Decentralized identity, federated discovery |

## Quick Start

```python
from agenticraft import Craft

# Create an agent
agent = (
    Craft.agent("Assistant")
    .model("gpt-4o")
    .memory("conversation")
    .tools(["web_search", "calculator"])
    .create()
)

response = await agent.run("Analyze this quarterly report")
```

### Multi-Provider Support

```python
from agenticraft import Craft

# OpenAI
openai_agent = Craft.agent("GPT").model("gpt-4o").create()

# Anthropic Claude
claude_agent = Craft.agent("Claude").model("claude-3-5-sonnet").create()

# Google Gemini
gemini_agent = Craft.agent("Gemini").model("gemini-pro").create()

# Local with Ollama
local_agent = Craft.agent("Local").model("ollama/llama3").create()
```

### Multi-Agent Teams

```python
from agenticraft import Craft

# Create a research team with consensus voting
team = (
    Craft.team("MarketResearch")
    .agents([
        Craft.analyst("Researcher").model("gpt-4o"),
        Craft.analyst("Validator").model("claude-3-5-sonnet"),
        Craft.writer("Synthesizer").model("gemini-pro")
    ])
    .strategy("consensus")
    .create()
)

report = await team.run("Analyze Q4 market trends and provide recommendations")
```

## Contact

Contact us for access to the AgentiCraft platform.

- Email: hello@agenticraft.ai
- Website: agenticraft.ai
