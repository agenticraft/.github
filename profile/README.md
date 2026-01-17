# AgentiCraft

  **Enterprise-grade agentic AI platform with production-ready infrastructure**

  From pilot to production in weeks, not months.

  ## What is AgentiCraft?

  AgentiCraft is an enterprise framework for creating production-ready AI agents. It features a 6-tier SLA-driven mesh architecture with 45 integrated services, 245+ battle-tested patterns across 22 categories, and support for 18 LLM providers.

  ## Key Features

  ### 18 LLM Providers
  - **Core**: OpenAI, Anthropic, Google, Mistral
  - **Performance**: Groq, Together, Fireworks, Cerebras
  - **Enterprise**: Azure OpenAI, AWS Bedrock
  - **Specialized**: Cohere, Perplexity, DeepSeek, xAI
  - **Local/Router**: Ollama, OpenRouter, Nebius

  ### 245+ Agent Patterns (22 Categories)
  - **Cognitive (39)**: Chain-of-Thought, Tree-of-Thoughts, ReAct, Reflection
  - **Coordination (51)**: Consensus, Voting, Swarm, Debate, Team
  - **Resilience (15)**: Circuit Breaker, Fallback, Retry, Bulkhead
  - **Workflow (14)**: DAG, Saga, State Machine, Event-Driven

  ### 6-Tier Mesh Architecture (45 Services)
  - **Critical Tier** (<100ms SLA): Security, Discovery, Observability
  - **Core Tier** (<200ms SLA): Agents, Events, Orchestration
  - **Platform Tier** (<500ms SLA): LLM, Data, Health
  - **Standard Tier** (<1s SLA): A2A, MCP, ANP, Streaming
  - **Background Tier**: Metrics, Evaluation, Cost
  - **Utility Tier**: Governance, HITL, Compliance

  ### Enterprise Infrastructure
  - 9-layer security (OAuth, RBAC, AES-256-GCM, SPIFFE)
  - MCP, A2A, and ANP protocol support
  - 48 REST API modules
  - OpenTelemetry distributed tracing
  - SOC2, GDPR, HIPAA, ISO27001 ready

  ## Quick Start

  ```python
  from agenticraft import Craft

  # Fluent builder API
  agent = (
      Craft.agent("Assistant")
      .model("gpt-4o")
      .memory(enabled=True)
      .tools(["web_search", "calculator"])
      .create()
  )

  response = await agent.generate("Hello, world!")

  # Or use presets
  analyst = Craft.analyst("DataBot").create()

  Repositories
  ┌────────────────────────────────────────────┬──────────────────────────┐
  │                 Repository                 │       Description        │
  ├────────────────────────────────────────────┼──────────────────────────┤
  │ https://github.com/agenticraft/agenticraft │ Core framework (1M+ LOC) │
  ├────────────────────────────────────────────┼──────────────────────────┤
  │ https://github.com/agenticraft/docs        │ Documentation            │
  ├────────────────────────────────────────────┼──────────────────────────┤
  │ https://github.com/agenticraft/examples    │ Example implementations  │
  └────────────────────────────────────────────┴──────────────────────────┘
  Get Involved

  - https://github.com/agenticraft/agenticraft/issues - Report bugs & request features
  - https://github.com/agenticraft/agenticraft/discussions - Ask questions
  - https://github.com/agenticraft/agenticraft/blob/master/CONTRIBUTING.md - Contribution guide

  License

  Business Source License 1.1 (BSL) - Free for development and internal use. Enterprise licenses available for production. Converts to Apache 2.0 after 4 years.
