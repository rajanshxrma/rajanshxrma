# Rajan Sharma

**CS @ Georgia State (2026)** — Software Engineer building on-device AI/ML on Apple's platform: Keep (on-device macOS assistant), orchard (agentic workflow engine), cadence (my first MCP server), maxwell (a neural quantum error-correction decoder in MLX that beats the standard matching decoder), langchain-apple-foundation-models (first LangChain provider for Apple's on-device models), and 3 merged fixes in Apple's MLX inference framework. Also build reliable, well-tested backend systems in Java & Python.
Open to **Software Engineer roles focused on AI/ML**.

## What I build
A connected suite of production-style backend services (aviation-ops domain):

| Project | What it does | Stack |
|---|---|---|
| [aerolane](https://github.com/rajanshxrma/aerolane) | Airport screening ops tracker | Spring Boot 3 · Keycloak SSO · PostgreSQL · Flyway · Docker · K8s |
| [checkride](https://github.com/rajanshxrma/checkride) | QA automation framework for aerolane | REST Assured · Selenium · Testcontainers · Gatling · JUnit 5 · Allure |
| [tarmac](https://github.com/rajanshxrma/tarmac) | Event-driven incident dispatch | 2 Spring Boot services · Kafka (retry/backoff + DLQ) · MongoDB · Docker |
| [conveyor](https://github.com/rajanshxrma/conveyor) | Batch ETL for airport throughput | Spring Batch 5 · skip/retry + quarantine · PostgreSQL · Flyway · Docker |

AI / RAG:

| Project | What it does | Stack |
|---|---|---|
| [switchboard-ai](https://github.com/rajanshxrma/switchboard-ai) | Voice-AI for sales/claims calls | Twilio Media Streams · GPT-4o agents · ML analytics · Azure K8s |
| [finance-rag](https://github.com/rajanshxrma/finance-rag) | Query bank statements in plain English | RAG · OpenAI · Supabase pgvector |

On-device & local-first AI (Apple Foundation Models / MLX / MCP):

| Project | What it does | Stack |
|---|---|---|
| [keep](https://github.com/rajanshxrma/keep) | Private on-device macOS assistant — acts, searches your files, describes your screen, full voice in/out (merges private-agent, stacks, lantern into one app) | Apple Foundation Models · MLX · Vision · Speech · AppleScript |
| [orchard](https://github.com/rajanshxrma/orchard) | On-device agentic workflow engine — YAML pipelines compiled to LangGraph | LangGraph · Apple Foundation Models · MLX |
| [langchain-apple-foundation-models](https://github.com/rajanshxrma/langchain-apple-foundation-models) | LangChain provider for Apple's on-device AI (PyPI) | Python · LangChain |
| [cadence](https://github.com/rajanshxrma/cadence) | Local-first health engine — correlates WHOOP/Apple Health with git activity and AI usage, personal baselines, on-device narration, served via MCP | MCP · SQLite · OAuth 2.0 · Keychain · Apple Foundation Models |
| [maxwell](https://github.com/rajanshxrma/maxwell) | Neural surface-code decoder for quantum error correction — beats minimum-weight perfect matching, trained and benchmarked entirely on-device | MLX · stim · PyMatching · transformer |

Also contribute directly to Apple's [MLX inference framework](https://github.com/ml-explore/mlx-lm) — a quantization load-fix, a KV-cache memory-safety fix, and a server reliability fix.

## Tools
**Languages:** Java, Python, Swift
**Backend:** Spring Boot 3, Spring Batch, REST, Kafka
**AI/On-device:** Apple Foundation Models, MLX, LangGraph, LangChain, MCP
**Data:** PostgreSQL, MongoDB, Flyway, Supabase/pgvector
**QA:** JUnit 5, REST Assured, Selenium, Testcontainers, Gatling, Allure
**DevOps:** Docker, Kubernetes, CI/CD, Git

## Open to
Software Engineer roles focused on AI/ML, internships and new-grad.
