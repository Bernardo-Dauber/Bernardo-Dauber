# Hi, I'm Bernardo 👋

**Software Engineer / AI Engineer** from southern Brazil — I build things with LLMs, mostly in Python and TypeScript on AWS.

By day I work on generative AI that has to survive production: multi-agent systems, RAG over knowledge bases, document extraction, streaming chat, and all the unglamorous plumbing — prompt versions, tracing, cost and latency telemetry, Terraform. What I like most is the seam between the model and the user: the contract that makes an agent feel predictable instead of magical.

---

## 🌙 What I build for myself

- **`organizer`** — a self-hosted organizer for my own life (gym, finances, calendar on one date spine). Go + SQLite backend, React/TypeScript front, and a written spec and architecture decision record for every screen before I write code.
- **`harness`** — one repo that configures all my coding agents (Claude Code, Hermes, Codex, opencode, Cursor and friends): shared skills, hooks and config, plus per-run telemetry so I can see where the agents actually save me time — and where they cost me rework.
- **`workflow-orquestracao`** — my day planned by agents: it gathers my open PRs and the sprint's tickets, implements only the tasks I mark, opens draft PRs and never merges.
- **RAG, MCP and memory experiments** — including [chat-agentcore](https://github.com/Bernardo-Dauber/chat-agentcore), a single-endpoint agent with retrieval over S3, an MCP server and short + long-term memory.

## 🎓 What I'm studying

My undergraduate thesis is about **uncertainty**: when an LLM says it's *80% confident* about a Brazilian financial fact, is it right 80% of the time? I measure that with proper scoring rules (Brier, log score, ECE), conformal prediction and VaR backtesting as a coverage test — with a side branch on whether generative models reproduce **tail risk** or quietly smooth it out exactly where it matters most.

Outside of that: markets and personal finance (I automate my own portfolio reporting), a lot of probability and risk, Linux as a daily driver, and occasionally a routing lab just for fun.

## 🛠️ Tools I reach for

**Python · TypeScript · Go · Java** — AWS (Bedrock, AgentCore, Lambda, Step Functions, S3, DynamoDB, Terraform) · Strands Agents, LangChain, LangGraph, OpenAI Agents · RAG, MCP, knowledge bases · FastAPI, NestJS, Next.js, React · PostgreSQL, SQLite, MongoDB, Prisma · Docker.

## 📫 Say hi

- [LinkedIn](https://www.linkedin.com/in/bernardo-dauber/)
- Email: be.daubervieira@gmail.com

<details>
<summary>🇧🇷 Em português</summary>

**Software Engineer / AI Engineer** do sul do Brasil — construo coisas com LLMs, principalmente em Python e TypeScript na AWS.

De dia trabalho com IA generativa que precisa sobreviver à produção: sistemas multiagente, RAG sobre bases de conhecimento, extração de documentos, chat com streaming e toda a parte pouco glamourosa — versões de prompt, tracing, telemetria de custo e latência, Terraform. O que mais gosto é a costura entre o modelo e quem usa: o contrato que faz o agente parecer previsível em vez de mágico.

**O que construo para mim** — `organizer` (organizador pessoal auto-hospedado: academia, finanças e calendário numa mesma espinha de datas; Go + SQLite no backend, React/TypeScript no front), `harness` (um repositório que configura todos os meus agentes de código, com telemetria por execução), `workflow-orquestracao` (meu dia planejado por agentes: PRs e tickets, implementação em worktrees, PRs em draft, nunca merge) e experimentos de RAG, MCP e memória.

**TCC** — incerteza: quando um LLM diz que tem 80% de certeza sobre um fato financeiro brasileiro, ele acerta 80% das vezes? Brier, log score, ECE, predição conformal, backtesting de VaR e uma verificação de se modelos generativos reproduzem risco de cauda ou suavizam justamente onde mais importa.

Fora disso: mercado e finanças pessoais (automatizo meus próprios relatórios), probabilidade e risco, Linux no dia a dia e, de vez em quando, um lab de roteamento por diversão.

</details>
