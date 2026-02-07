<div align="center">

# AgentiCraft

### The Enterprise Multi-Agent Platform

**From pilot to production in weeks, not months.**

Build, deploy, and scale AI agents with enterprise-grade security, observability, and governance.

---

`214+ Patterns` · `45+ Mesh Services` · `18 LLM Providers` · `9-Layer Security` · `MCP + A2A + ANP`

---

</div>

## The Challenge

Most companies can build a prototype AI agent in days. Getting it to production — secure, reliable, compliant — takes months and often fails entirely.

| | |
|---|---|
| **65%** of AI pilots stall before scaling | **11%** reach full production |
| **86%** need tech stack upgrades | **$7B → $236B** market by 2034 |

**AgentiCraft bridges this gap** — providing both AI agent logic and enterprise infrastructure in one unified platform.

## Platform Architecture

```
┌─────────────────────────────────────────────────────────────┐
│  Protocol Layer        MCP (Tools) + A2A (Agents) + ANP     │
├─────────────────────────────────────────────────────────────┤
│  LLM Providers         18 providers, one interface           │
├─────────────────────────────────────────────────────────────┤
│  Mesh Services         45+ services, 6 SLA tiers             │
│                        Security · Observability · Events     │
├─────────────────────────────────────────────────────────────┤
│  Agent Layer           214+ patterns, 25+ mixins             │
├─────────────────────────────────────────────────────────────┤
│  Craft API             Fluent builder · REST · GraphQL       │
└─────────────────────────────────────────────────────────────┘
```

## Key Capabilities

### Agent Patterns (214+ across 19 categories)

- **Cognitive** — Chain-of-Thought, Tree-of-Thoughts, ReAct, Reflection, Self-Ask
- **Coordination** — Consensus (Paxos, Raft, PBFT), Swarm, Gossip, Contract Net
- **Workflow** — Pipeline, StateMachine, DAG, Human-in-the-Loop
- **Resilience** — Circuit Breaker, Retry, Saga, Bulkhead
- **RAG** — GraphRAG, HybridRAG, AdaptiveRAG
- **Safety** — Constitutional, Adversarial, Guardrails
- **Planning** — HTN, MCTS, Temporal Planning

### Mesh Services (45+ with defined SLAs)

| Tier | SLA | Services |
|------|-----|----------|
| **Critical** | 99.99% | Security, Discovery, Observability |
| **Core** | 99.95% | Agents, Events, Orchestration |
| **Platform** | 99.9% | LLM, Data, MCP |
| **Standard** | 99.5% | A2A, Streaming, Patterns |
| **Background** | 99% | Training, Cost, Evaluation |
| **Utility** | 95% | Governance, HITL, Plugins |

### 9-Layer Security

Authentication · Authorization · Cryptography · Audit Logging · Sandbox Isolation · Security Context · Guardrails · Policy Engine · Runtime Monitor

**Compliance:** SOC 2 · GDPR · HIPAA · PCI-DSS · ISO 27001

### LLM Providers (18)

OpenAI · Anthropic · Google · Mistral · Groq · Cerebras · Together · Fireworks · DeepSeek · Cohere · Perplexity · xAI · Azure OpenAI · AWS Bedrock · Ollama · OpenRouter · Nebius · and more

### Protocol Standards

| Protocol | Purpose | What It Enables |
|----------|---------|-----------------|
| **MCP** | Agent ↔ Tools | Tool discovery, context sharing, resource management |
| **A2A** | Agent ↔ Agent | Task delegation, coordination, state sync |
| **ANP** | Agent ↔ Networks | Decentralized identity, federated discovery |

## Quick Start

```python
from agenticraft import Craft

# Create an agent with the fluent builder API
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

openai_agent  = Craft.agent("GPT").model("gpt-4o").create()
claude_agent  = Craft.agent("Claude").model("claude-3-5-sonnet").create()
gemini_agent  = Craft.agent("Gemini").model("gemini-pro").create()
local_agent   = Craft.agent("Local").model("ollama/llama3").create()
```

### Multi-Agent Teams

```python
from agenticraft import Craft

team = (
    Craft.team("MarketResearch")
    .agents([
        Craft.analyst("Researcher").model("gpt-4o"),
        Craft.analyst("Validator").model("claude-3-5-sonnet"),
        Craft.writer("Synthesizer").model("gemini-pro"),
    ])
    .strategy("consensus")
    .create()
)

report = await team.run("Analyze Q4 market trends and provide recommendations")
```

## Research

AgentiCraft includes a built-in evaluation framework with 12 benchmarks (SWE-bench, GAIA, GSM8K, HumanEval, MMLU, and more) and 55+ coordination strategies for multi-agent research.

## Contact

- **Email:** hello@agenticraft.ai
- **Security:** security@agenticraft.ai
- **Website:** [agenticraft.ai](https://agenticraft.ai)
