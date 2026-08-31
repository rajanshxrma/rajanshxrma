# Rajan Sharma

**CS @ Georgia State (2026)** — building on Apple Silicon: on-device AI/ML (Foundation Models, MLX, agentic systems) and iOS, backed by production systems engineering (Kubernetes, async services, concurrent data structures). Shipping software since 2020 — [reMemo](https://github.com/rajanshxrma/reMemo), a memo app on Amazon/Google Play/Samsung, built as a teenager learning to ship real software. Recent work includes a neural decoder that beats a classical baseline in quantum error correction, and open pull requests against Apple's own MLX inference framework.
Open to **Software Engineer roles in AI/ML and backend/infra** — internships and new-grad.

## Highlights

- **[maxwell](https://github.com/rajanshxrma/maxwell)** — a neural decoder for quantum error correction, trained and benchmarked entirely on-device in MLX on Apple Silicon. Beats the industry-standard matching decoder (PyMatching's MWPM) on logical error rate at every physical error rate tested, measured on data the model never trained on.
- **Open source on Apple's MLX** — [active pull requests](https://github.com/ml-explore/mlx-lm/pulls?q=is%3Apr+author%3Arajanshxrma) against `ml-explore/mlx-lm`: a quantization-loading fix, a KV-cache checkout/return API for memory safety, and a server crash fix — plus root-cause investigations, each with a reproducible test harness, into a quantized-attention memory regression and a speculative-decoding correctness edge case, both corroborated by other contributors on the thread.
- **[keep](https://github.com/rajanshxrma/keep)** — a private, fully on-device macOS assistant (Apple Foundation Models, Vision, Speech) that acts on your files, searches your machine, and describes your screen — zero network calls, nothing leaves the device. [Launched on Show HN](https://news.ycombinator.com/item?id=49415076).
- **[langchain-apple-foundation-models](https://github.com/rajanshxrma/langchain-apple-foundation-models)** — the first LangChain provider for Apple's on-device models, published on PyPI, verified against LangChain's own compliance test suite, with its integration docs merged into LangChain's official documentation.
- **[cobux-oss](https://github.com/rajanshxrma/cobux-oss)** — an iOS book-wisdom companion: AI chat that only cites your own highlights (the model self-declares real citations, not retrieval-inferred ones), FSRS-6 spaced-repetition review, full voice mode, Apple Watch companion.
- **[sisyphus-oss](https://github.com/rajanshxrma/sisyphus-oss)** — an autonomous AI job-application engine, open-sourced as a config-driven template: a scheduled Claude Code cloud routine discovers and classifies roles behind deterministic seniority/eligibility/ghost-posting filters, tailors one-page LaTeX resumes from a version-controlled knowledge base without inventing experience, and delivers everything to a zero-build kanban tracker with a ⌘K palette.
- **[sentinel](https://github.com/rajanshxrma/sentinel)** — a self-healing Kubernetes operator in Go: watches deployment health, triggers rate-limited rolling restarts, live-verified on a real cluster, backed by a three-layer test suite.

## What I build

Systems, infra & backend:

| Project | What it does | Stack |
|---|---|---|
| [sentinel](https://github.com/rajanshxrma/sentinel) | Self-healing Kubernetes operator — watches deployment health, triggers rate-limited rolling restarts before it just loops forever | Go · controller-runtime · CRDs · Helm |
| [ferroledger](https://github.com/rajanshxrma/ferroledger) | Async double-entry ledger service — hand-rolled optimistic concurrency control, append-only WAL-durable log | Rust · Axum · PostgreSQL |
| [corecache](https://github.com/rajanshxrma/corecache) | Header-only concurrent cache — real O(1) LRU plus a full Adaptive Replacement Cache, lock-free read path | C++20 |
| [packetpulse](https://github.com/rajanshxrma/packetpulse) | Low-latency market-data handler — kernel-aware UDP multicast fast path, nanosecond-resolution latency histograms under load | C++20 |
| [torchserve-sentinel](https://github.com/rajanshxrma/torchserve-sentinel) | Fine-tuned PII/sensitive-data token classifier behind a batched endpoint, with drift monitoring | Python · DistilBERT · FastAPI · Prometheus/Grafana |
| [spendtrack](https://github.com/rajanshxrma/spendtrack) | Native Android spend/receipt tracker, integer-cent accounting | Kotlin · Jetpack Compose · Room |

AI & on-device (Apple Foundation Models / MLX / MCP):

| Project | What it does | Stack |
|---|---|---|
| [keep](https://github.com/rajanshxrma/keep) | Private on-device macOS assistant — acts, searches your files, describes your screen, full voice in/out (merges private-agent, stacks, lantern into one app) | Apple Foundation Models · MLX · Vision · Speech · AppleScript |
| [maxwell](https://github.com/rajanshxrma/maxwell) | Neural surface-code decoder for quantum error correction — beats minimum-weight perfect matching, trained and benchmarked entirely on-device | MLX · stim · PyMatching · transformer |
| [langchain-apple-foundation-models](https://github.com/rajanshxrma/langchain-apple-foundation-models) | LangChain provider for Apple's on-device AI (PyPI); integration docs merged into langchain-ai/docs | Python · LangChain |
| [orchard](https://github.com/rajanshxrma/orchard) | On-device agentic workflow engine — YAML pipelines compiled to LangGraph | LangGraph · Apple Foundation Models · MLX |
| [cadence](https://github.com/rajanshxrma/cadence) | Local-first health engine — correlates WHOOP/Apple Health with git activity and AI usage, personal baselines, on-device narration, served via MCP. Listed in [awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers). | MCP · SQLite · OAuth 2.0 · Keychain · Apple Foundation Models |
| [cobux-oss](https://github.com/rajanshxrma/cobux-oss) | iOS book-wisdom companion — AI chat grounded only in your own highlights (model self-declares real citations, not inferred from retrieval), FSRS-6 spaced-repetition quiz, voice mode, Watch companion | SwiftUI · SwiftData · Claude API · FSRS-6 |
| [sisyphus-oss](https://github.com/rajanshxrma/sisyphus-oss) | Autonomous job-application engine — scheduled Claude Code routine discovers/filters/classifies roles, RAG-tailors one-page LaTeX resumes on demand, tracker dashboard with kanban + command palette | Claude Code routines · Python · LaTeX · Cloudflare Pages |
| [tensortrace](https://github.com/rajanshxrma/tensortrace) | Metal compute kernel profiling and optimization harness — real GPU kernels, real measured speedups | Metal · Apple Silicon |
| [preftune](https://github.com/rajanshxrma/preftune) | Local SFT-then-DPO LoRA fine-tuning — honest before/after preference-accuracy results, including a real degenerate-collapse finding | MLX · LoRA · Apple Silicon |

Applied engineering: a connected four-service backend suite over one domain (airport ops) — [aerolane](https://github.com/rajanshxrma/aerolane) (Spring Boot 3 · Keycloak SSO · PostgreSQL · Docker · K8s), [checkride](https://github.com/rajanshxrma/checkride) (its QA automation framework — REST Assured · Selenium · Testcontainers · Gatling), [tarmac](https://github.com/rajanshxrma/tarmac) (event-driven incident dispatch — Kafka retry/DLQ · MongoDB), and [conveyor](https://github.com/rajanshxrma/conveyor) (batch ETL — Spring Batch 5 · skip/retry + quarantine).

## Tools
**Languages:** Java, Python, Swift, Go, Rust, C++, Kotlin
**Backend:** Spring Boot 3, Spring Batch, REST, Kafka, Axum
**AI/On-device:** Apple Foundation Models, MLX, LangGraph, LangChain, MCP
**Data:** PostgreSQL, MongoDB, Flyway, Supabase/pgvector
**QA:** JUnit 5, REST Assured, Selenium, Testcontainers, Gatling, Allure
**DevOps:** Docker, Kubernetes, CI/CD, Git, Prometheus/Grafana
