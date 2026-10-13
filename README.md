# Bernardo Dauber Vieira

**Software Engineer** building end-to-end **Generative AI** products — mostly Python and TypeScript on AWS, turning "the agent works in the demo" into multi-agent systems that are fast, scalable and production-ready.

My work has a theme: making an agent behave predictably outside the notebook. One contract between client and backend, one place for the agent's configuration, one source of truth for its tools and telemetry — so nothing has to be rewritten when the backend changes.

Currently a **Software Engineer** (full-time, remote) in a team that turns GenAI ideas into real products, and a **Ciência da Computação** student at **Unisinos** (RS, Brazil).

---

## 🔭 What I build at work

Products across **legal tech, real estate, education, media and e-commerce** — from PoC to production.

- **Automated legal document generation** — a multi-agent system that produces structured legal petitions in **under 30 seconds** using parallel specialist agents. *(AWS Bedrock AgentCore · LangChain · LangGraph · Strands Agents)*
- **Conversational AI for US real estate investors** — assistant that consolidates portfolio data and financial forecasts through a multi-agent architecture. *(OpenAI Agents & Tools · function calling · Python · AWS)*
- **AI lesson-plan generator** — plans aligned with Brazil's national curriculum (BNCC), saving teachers hours of weekly planning. *(AWS Bedrock · Step Functions · Lambda · Docker · Python)*
- **AI-powered video clip generation** — pipeline that finds and cuts highlight moments from long-form video based on emotion and storytelling. *(AWS Transcribe · Langflow · prompt engineering)*

And the ground under it: RAG over knowledge bases, document extraction, streaming chat contracts, usage/cost telemetry, Terraform-managed AWS.

## 🧰 Personal projects

- `harness` — single-source configuration for my coding agents: **8 harnesses** (Claude Code, pi, Hermes, opencode, Codex, Copilot, Cursor, Windsurf) driven from one repo — skills, agents, hooks and extensions as symlinks, app-rewritten configs as copies — plus per-run **telemetry** and a rework/cost/success report. `git clone` + `./install.sh` reproduces the whole setup.
- `workflow-orquestracao` — daily task orchestration with agents: collects my open PRs and the current sprint's Jira tickets into a *plano do dia* issue, implements only the marked items in `git worktree`, opens **draft PRs** (never merges), then reports rework, success rate, cost and time from `telemetry/runs.jsonl`.
- `organizer` — a self-hosted, single-user life organizer (**gym**, **finance**, **calendar** on a shared date spine): **Go + SQLite** backend, React/TypeScript frontend. Architecture docs, ADRs and a spec per screen before the first line of code.
- `chat-template-aws-harness` — chat template whose agent backend is an **AgentCore Harness invoked directly by the Next.js server**: no container, no ECR image, deploy is a single `terraform apply`, SSE contract with the frontend untouched.
- [chat-agentcore](https://github.com/Bernardo-Dauber/chat-agentcore) — PoC of a single-endpoint conversational agent with **RAG over S3 + Knowledge Base**, an **MCP server** and short/long-term **memory**.
- [trabalho-ga-roteamento-ip](https://github.com/Bernardo-Dauber/trabalho-ga-roteamento-ip) — Containerlab/FRR lab with **5 routers** running RIPv2 and OSPFv2, plus **LARP**, a protocol of my own for active-latency routing metrics.

## 🎓 Undergraduate thesis (TCC)

**Uncertainty and calibration of LLMs in financial text.** If a language model says it is *80% confident* about a Brazilian financial fact, is it right 80% of the time? Proper scoring rules (Brier, log score, ECE, reliability diagrams), conformal prediction for guaranteed coverage, VaR backtesting as a coverage test — plus a branch on **synthetic generation and tail risk** (GAN/diffusion vs. GARCH, block bootstrap, EVT), judged by tail properties instead of accuracy.

## 🛠️ Technical stack

| | |
|---|---|
| **Languages** | Python · TypeScript · JavaScript · Go · Java · SQL |
| **GenAI / agents** | AWS Bedrock (AgentCore, Knowledge Bases) · Strands Agents · LangChain · LangGraph · OpenAI Agents & Tools · MCP · RAG · prompt engineering |
| **Cloud / Backend** | AWS Lambda · Step Functions · DynamoDB · S3 · Amplify · Cognito · Terraform · FastAPI · NestJS · Node.js · Spring Boot |
| **Frontend** | React · Next.js · TypeScript |
| **Data** | PostgreSQL · MongoDB · SQLite · Prisma |
| **Practices** | system design, ADRs and written specs, streaming (SSE) contracts, agent-run telemetry, Docker, GitHub Actions |

## 📫 How to reach me

- [LinkedIn](https://www.linkedin.com/in/bernardo-dauber/)
- Email: be.daubervieira@gmail.com

<details>
<summary>🇧🇷 Versão em português</summary>

**Software Engineer** construindo produtos de **IA generativa** de ponta a ponta — principalmente Python e TypeScript na AWS, transformando "o agente funciona no demo" em sistemas multiagente rápidos, escaláveis e prontos para produção.

No trabalho, produtos em **legal tech, imobiliário, educação, mídia e e-commerce**:
- Geração automatizada de documentos jurídicos — sistema multiagente que produz petições estruturadas em menos de 30 segundos com agentes especialistas em paralelo (AWS Bedrock AgentCore · LangChain · LangGraph · Strands Agents).
- IA conversacional para investidores imobiliários nos EUA — consolida dados de carteira e projeções financeiras em arquitetura multiagente (OpenAI Agents & Tools · function calling · Python · AWS).
- Gerador de planos de aula alinhados à BNCC (AWS Bedrock · Step Functions · Lambda · Docker · Python).
- Geração de cortes de vídeo por emoção e narrativa (AWS Transcribe · Langflow · prompt engineering).

**Projetos pessoais** — `harness` (configuração em fonte única para 8 harnesses de código, com telemetria por execução), `workflow-orquestracao` (plano do dia a partir de PRs e Jira, implementação em worktrees, PRs em draft), `organizer` (organizador pessoal auto-hospedado: academia, finanças e calendário; Go + SQLite no backend, React/TypeScript no front) e o PoC `chat-agentcore` (RAG em S3/Knowledge Base, servidor MCP e memória).

**TCC** — incerteza e calibração de LLMs em textos financeiros (Brier, log score, ECE, predição conformal, backtesting de VaR) e geração sintética de risco de cauda.

</details>
