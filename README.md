# Bernardo Dauber Vieira

**Ciência da Computação** student at **Unisinos** (RS, Brazil) working mostly as a **backend developer for AI products** — Python and TypeScript on AWS, building LLM agents that actually ship: streaming chat, retrieval, tool use, memory, and cost/latency telemetry.

My work has a theme: making an agent behave predictably outside the demo. One contract between client and backend, one place for the agent's configuration, no silent rewrite of the client when the backend changes.

---

## 🔭 What I'm working on now

**AI agents on AWS Bedrock AgentCore**
- `chat-template-aws-harness` — a chat template whose agent backend is an **AgentCore Harness invoked directly by the Next.js server** — no container, no ECR image, deploy is a single `terraform apply`, and the SSE contract with the frontend is untouched. The ADR in the repo explains why I dropped the older Runtime + Docker design.
- [chat-agentcore](https://github.com/Bernardo-Dauber/chat-agentcore) — PoC of a single-endpoint conversational agent with **RAG over S3 + Knowledge Base**, an **MCP server**, and short- and long-term **memory**.

**Agentic engineering tooling** (what I use to build the above)
- `harness` — single-source configuration for my coding agents: **8 harnesses** (Claude Code, pi, Hermes, opencode, Codex, Copilot, Cursor, Windsurf) driven from one repo, where skills, agents, hooks and extensions are symlinks and app-rewritten configs are copies, plus per-run **telemetry** and a rework/cost/success report. `git clone` + `./install.sh` reproduces the whole setup.
- `workflow-orquestracao` — daily task orchestration with agents: collects my open PRs and the current sprint's Jira tickets into a *plano do dia* issue, implements only the marked items inside `git worktree`, opens **draft PRs** (never merges), then reports rework, success rate, cost and time from `telemetry/runs.jsonl`.

**Backend & product**
- `organizer` — a self-hosted, single-user life organizer (**gym**, **finance**, **calendar** on a shared date spine), **Go + SQLite** backend, React/TypeScript frontend. Currently at specification stage: architecture docs, ADRs and a spec per screen before the first line of code.
- `personal-finance-dashboard` — full-stack finance app: NestJS + Prisma + PostgreSQL, Next.js + React + shadcn/ui.

**Networking**
- [trabalho-ga-roteamento-ip](https://github.com/Bernardo-Dauber/trabalho-ga-roteamento-ip) — Containerlab/FRR lab with **5 routers** running RIPv2 and OSPFv2, plus **LARP**, a protocol of my own for active-latency routing metrics.

**Coursework I still like**
- [Car-Rental-Management-System](https://github.com/Bernardo-Dauber/Car-Rental-Management-System), [Pool-of-Process](https://github.com/Bernardo-Dauber/Pool-of-Process), [TrabalhoGB2](https://github.com/Bernardo-Dauber/TrabalhoGB2), [ProjectEmail](https://github.com/Bernardo-Dauber/ProjectEmail), [trabalho-gb-algoritmos](https://github.com/Bernardo-Dauber/trabalho-gb-algoritmos).

## 🎓 Undergraduate thesis (TCC)

**Uncertainty and calibration of LLMs in financial text.** If a language model says it is *80% confident* about a Brazilian financial fact, is it right 80% of the time? Worked with proper scoring rules (Brier, log score, ECE, reliability diagrams), conformal prediction for guaranteed coverage, and VaR backtesting as a coverage test — plus a branch on **synthetic generation and tail risk** (GAN/diffusion vs. GARCH, block bootstrap and EVT), judged by tail properties instead of accuracy.

## 🛠️ Technologies

| | |
|---|---|
| **Languages** | Python · TypeScript/JavaScript · Go · Java · SQL · Shell |
| **AI / Cloud** | AWS (Bedrock, AgentCore Harness & Runtime, S3, Knowledge Bases) · RAG · MCP · tool use & memory · Strands Agents |
| **Backend** | FastAPI · NestJS · Spring Boot · PostgreSQL · SQLite · MongoDB · Prisma · Docker · Terraform |
| **Practices** | git worktrees, ADRs and written specs, GitHub Actions, telemetry on agent runs |

## 📫 How to reach me

- [LinkedIn](https://www.linkedin.com/in/bernardo-dauber/)
- Email: be.daubervieira@gmail.com

<details>
<summary>🇧🇷 Versão em português</summary>

Estudante de **Ciência da Computação** (Unisinos). Trabalho principalmente como **desenvolvedor backend de produtos com IA** — Python e TypeScript na AWS, construindo agentes que saem do demo: chat com streaming, recuperação de informação, uso de ferramentas, memória e telemetria de custo/latência.

- **Agentes na AWS Bedrock AgentCore** — template de chat com o backend do agente em um AgentCore Harness chamado direto pelo servidor Next.js (sem container, sem ECR) e PoC de agente com RAG em S3/Knowledge Base, servidor MCP e memória curta + longa.
- **Ferramental de engenharia com agentes** — `harness` (configuração em fonte única para 8 harnesses de código, com telemetria por execução) e `workflow-orquestracao` (plano do dia a partir de PRs e Jira, implementação em worktrees, PRs em draft, relatório de retrabalho/custo).
- **Backend e produto** — `organizer` (organizador pessoal auto-hospedado: gym, finanças e calendário; backend Go + SQLite, front React/TypeScript) e o dashboard financeiro em NestJS/Prisma/PostgreSQL + Next.js.
- **Redes** — lab Containerlab/FRR com 5 roteadores (RIPv2, OSPFv2) e um protocolo próprio de métrica ativa de latência.
- **TCC** — incerteza e calibração de LLMs em textos financeiros (Brier, log score, ECE, predição conformal, backtesting de VaR) e geração sintética de risco de cauda.

</details>
