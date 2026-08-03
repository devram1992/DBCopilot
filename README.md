#DBCopilot
Enterprise AI Assistant for Database Operations

## Overview
DBCopilot is an internal AI-powered assistant designed to support Database Operations teams by providing a unified interface for documentation search, incident analysis, infrastructure monitoring, log analysis, capacity planning, and operational intelligence.
Built entirely on open source technologies, DBCopilot leverages Retrieval-Augmented Generation (RAG), AI agents, and enterprise integrations to help engineers troubleshoot issues faster, access operational knowledge, and improve incident resolution.

## Vision
To provide a single intelligent platform that enables database engineers to interact with enterprise knowledge, monitoring systems, logs, incidents, and operational data using natural language.

## Documentation

| Doc | What |
|---|---|
| `RUN_GUIDE.md` | Complete run guide — local, EC2, Jenkins, demos |
| `docs/RAGOPS_COMPLETE.md` | What RAGOps is, architecture, V1→V2→V3 |
| `docs/V2_ARCHITECTURE.md` | Three worlds, flow diagrams, decision matrix |
| `docs/V3_PLAN.md` | Future roadmap (auto-eval, canary, drift, ES) |
| `docs/RUNBOOK.md` | 16 test flows with expected results |
| `docs/RAGOPS_WALKTHROUGH.ipynb` | Framework walkthrough notebook |
| `docs/RAGOPS_CODE_STRUCTURE.ipynb` | Code patterns notebook |
| `docs/EC2_JENKINS_SETUP.ipynb` | EC2 + Jenkins setup notebook |

## Tech Stack

| Concern | Choice |
|---|---|
| Backend | FastAPI + SQLAlchemy 2.0 |
| Frontend | Next.js 14 App Router |
| Database | PostgreSQL 16 |
| Vector Store | Qdrant |
| Cache | Redis (RedisStack with RediSearch) |
| LLM | Ollama (local) / Groq (cloud) |
| Eval | Ragas + Ollama judge |
| Observability | Langfuse + JSONL fallback |
| CI/CD | GitHub Actions + Jenkins (Jenkinsfile) |
| Container | Docker Compose |


