# Rajan Sharma

CS student at Georgia State University (Dec 2026). I build systems that keep running after I close the laptop.

**Flagship:** [autonomous-application-engine-public](https://github.com/rajanshxrma/autonomous-application-engine-public) — a pipeline that applies to jobs for me twice a day. n8n orchestration, GPT-4o tailoring from a version-controlled knowledge base, LaTeX compilation, application-ready PDFs in my inbox. A hard budget fence keeps it under $5/month. **[Live demo →](https://rajanshxrma.github.io/autonomous-application-engine-public/)**

## what's live

| repo | what it does |
|---|---|
| [aerolane](https://github.com/rajanshxrma/aerolane) | airport screening ops tracker — Spring Boot 3, three-role RBAC enforced server-side (not just hidden in the UI), Keycloak SSO, Postgres + Flyway, Docker, k8s |
| [checkride](https://github.com/rajanshxrma/checkride) | QA framework that black-box tests aerolane from the outside, the way a QA team would — REST Assured, Selenium, Testcontainers, Gatling load tests, Allure reports |
| [conveyor](https://github.com/rajanshxrma/conveyor) | batch ETL for hourly passenger data — Spring Batch 5; bad rows get quarantined with a reason instead of killing the job |
| [tarmac](https://github.com/rajanshxrma/tarmac) | event-driven incident dispatch — two Spring Boot services over Kafka, retry/backoff into a queryable dead-letter topic, MongoDB |

All four CI-green on GitHub Actions.

**In progress:** payledger — a payments API built on double-entry bookkeeping: idempotent transfers, money as integer cents (never floats), Spring Boot + Postgres, with Terraform/EC2 and Kubernetes deployment infra alongside.

## stack

Java · Spring Boot · JUnit 5 · Selenium · REST Assured · Kafka · Postgres · Docker · Kubernetes · Terraform · n8n · Python

📫 rajansharma9218@gmail.com
