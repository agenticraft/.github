  # AgentiCraft

  **Enterprise-grade agentic AI platform with multi-provider LLM support**

  Building powerful AI agents shouldn't be complicated.

  ## What is AgentiCraft?

  AgentiCraft is an open-source framework for creating production-ready AI agents with enterprise capabilities. It combines a
  modular architecture with 116 battle-tested patterns for cognitive reasoning, coordination, resilience, and workflows.

  ## Key Features

  ### Multi-Provider LLM Support
  - OpenAI, Anthropic, Google, Together, Groq, Mistral, Ollama
  - Unified API across all providers
  - Automatic fallback and load balancing

  ### 116 Agent Patterns
  - **Cognitive**: Chain-of-thought, ReAct, reflection
  - **Coordination**: Supervisor, swarm, hierarchical
  - **Resilience**: Circuit breaker, retry, bulkhead
  - **Workflow**: DAG, saga, state machine

  ### Enterprise Infrastructure
  - 19 mesh services with 9-layer security
  - MCP and A2A protocol integration
  - gRPC and WebSocket transports
  - OpenTelemetry distributed tracing
  - Vector memory (ChromaDB, FAISS, Qdrant, Weaviate)

  ## Quick Start

  ```python
  from agenticraft import craft

  agent = craft.agent("assistant").with_provider("openai").build()
  response = await agent.run("Hello, world!")

  Repositories

  | Repository                                 | Description             |
  |--------------------------------------------|-------------------------|
  | https://github.com/agenticraft/agenticraft | Core framework          |
  | https://github.com/agenticraft/docs        | Documentation           |
  | https://github.com/agenticraft/examples    | Example implementations |

  Get Involved

  - https://github.com/agenticraft/agenticraft/issues - Report bugs & request features
  - https://github.com/agenticraft/agenticraft/discussions - Ask questions
  - https://github.com/agenticraft/agenticraft/blob/master/CONTRIBUTING.md

  License

  Business Source License 1.1 (BSL) - Free for non-production use, converts to Apache 2.0 after 4 years.
