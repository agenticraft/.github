<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="readme-banner.svg">
  <source media="(prefers-color-scheme: light)" srcset="readme-banner.svg">
  <img alt="AgentiCraft" src="readme-banner.svg" width="100%">
</picture>

The enterprise AI agent platform. Build, deploy, and scale production agents with enterprise-grade security, deployment, and governance.

---

`200+ Patterns` · `40+ Mesh Services` · `18 LLM Providers` · `Defense-in-Depth Security` · `Open Protocols`

[![Website](https://img.shields.io/badge/agenticraft.ai-0D9488?style=flat-square&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA2NCA2NCIgd2lkdGg9IjY0IiBoZWlnaHQ9IjY0Ij48cG9seWdvbiBwb2ludHM9IjM5LDcgNTMsMjQgMzYsMjgiIGZpbGw9IndoaXRlIiBvcGFjaXR5PSIwLjg1Ii8+PHBvbHlnb24gcG9pbnRzPSIzOSw3IDEyLDMzIDM2LDI4IiBmaWxsPSJ3aGl0ZSIgb3BhY2l0eT0iMC43Ii8+PHBvbHlnb24gcG9pbnRzPSI1MywyNCA0Nyw0OSAzNiwyOCIgZmlsbD0id2hpdGUiIG9wYWNpdHk9IjAuNzUiLz48cG9seWdvbiBwb2ludHM9IjQ3LDQ5IDIyLDU0IDM2LDI4IiBmaWxsPSJ3aGl0ZSIgb3BhY2l0eT0iMC45Ii8+PHBvbHlnb24gcG9pbnRzPSIyMiw1NCAxMiwzMyAzNiwyOCIgZmlsbD0id2hpdGUiIG9wYWNpdHk9IjAuOTUiLz48Y2lyY2xlIGN4PSIzOSIgY3k9IjciIHI9IjMiIGZpbGw9IndoaXRlIi8+PGNpcmNsZSBjeD0iNTMiIGN5PSIyNCIgcj0iMi44IiBmaWxsPSJ3aGl0ZSIvPjxjaXJjbGUgY3g9IjQ3IiBjeT0iNDkiIHI9IjIuOCIgZmlsbD0id2hpdGUiLz48Y2lyY2xlIGN4PSIyMiIgY3k9IjU0IiByPSIyLjgiIGZpbGw9IndoaXRlIi8+PGNpcmNsZSBjeD0iMTIiIGN5PSIzMyIgcj0iMyIgZmlsbD0id2hpdGUiLz48Y2lyY2xlIGN4PSIzNiIgY3k9IjI4IiByPSIzLjIiIGZpbGw9IndoaXRlIi8+PC9zdmc+)](https://agenticraft.ai)
[![Python](https://img.shields.io/badge/Python-3.12+-3776AB?style=flat-square&logo=python&logoColor=white)](https://python.org)

---

</div>

## The Challenge

Most companies can build a prototype AI agent in days. Getting it to production — secure, reliable, compliant — takes months and often fails entirely.

88% of AI pilots fail to reach production ([IDC](https://www.cio.com/article/3850763/88-of-ai-pilots-fail-to-reach-production-but-thats-not-all-on-it.html)). 86% need tech stack upgrades for AI agents ([Tray.ai](https://www.architectureandgovernance.com/artificial-intelligence/new-research-uncovers-top-challenges-in-enterprise-ai-agent-adoption/)). 70-85% of GenAI deployments fail to meet ROI ([NTT Data](https://www.nttdata.com/global/en/insights/focus/2024/between-70-85p-of-genai-deployment-efforts-are-failing)).

**AgentiCraft bridges this gap** — providing both AI agent logic and enterprise infrastructure in one unified platform.

## What We Offer

- **200+ agent patterns** across reasoning, coordination, workflow, resilience, RAG, safety, and planning
- **40+ mesh services** with defined SLAs — security, canary deployment, agent marketplace, API gateway, and more
- **18 LLM providers** through one unified interface — switch models without changing code
- **Defense-in-depth security** with enterprise compliance controls
- **Open protocol support** — MCP (Model Context Protocol) and A2A (Agent-to-Agent) for tool integration and inter-agent communication
- **Built-in evaluation** with industry-standard benchmarks

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
claude_agent  = Craft.agent("Claude").model("claude-sonnet-4-5").create()
gemini_agent  = Craft.agent("Gemini").model("gemini-3-pro").create()
local_agent   = Craft.agent("Local").model("ollama/llama3").create()
```

### Multi-Agent Teams

```python
from agenticraft import Craft

team = (
    Craft.team("MarketResearch")
    .agents([
        Craft.analyst("Researcher").model("gpt-4o"),
        Craft.analyst("Validator").model("claude-sonnet-4-5"),
        Craft.writer("Synthesizer").model("gemini-3-pro"),
    ])
    .strategy("consensus")
    .create()
)

report = await team.run("Analyze Q4 market trends and provide recommendations")
```

## Contact

- **Website:** [agenticraft.ai](https://agenticraft.ai)
- **Email:** hello@agenticraft.ai
- **Security:** security@agenticraft.ai
