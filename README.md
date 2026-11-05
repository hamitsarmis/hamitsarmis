# Hamit Sarmış

Senior .NET engineer (15 years) who builds agentic systems — the backend, the pipelines and the LLM layer on top of them.

- 11 years in core banking (ESB, rule engines, WCF → ASP.NET Core migration), then 4 years of real-time sports-tech (WPF, video pipelines, now backend for a desktop-to-web migration) for a Copenhagen sports-tech company.
- Since 2026: agent systems in Python and C# — a structured-output pipeline ([telegram_listener](https://github.com/hamitsarmis/telegram_listener)), an MCP server ([webhook-dotnet](https://github.com/hamitsarmis/webhook-dotnet)), a Claude Code–orchestrated agent team ([strategy-team](https://github.com/hamitsarmis/strategy-team)). Everything below ships with its Docker setup.
- I care about the boring parts: idempotency, outbox, confirmation gates, audit logs. An agent that can place a trade gets a dry-run default, a single-use token and a kill switch.

## Agentic systems

| Repo | What | Stack |
|---|---|---|
| [telegram_listener](https://github.com/hamitsarmis/telegram_listener) | Telegram signal channel → Claude structured output → broker; Kafka spine, Redis thread memory, server-side compaction | Python, Claude API, Kafka, Redis, MetaApi |
| [webhook-dotnet](https://github.com/hamitsarmis/webhook-dotnet) | TradingView → outbox pipeline → broker, exposed to agents through an MCP server with dry-run, confirmation tokens and an audit log | .NET 10, MCP C# SDK, Postgres, RabbitMQ |
| [strategy-team](https://github.com/hamitsarmis/strategy-team) | Claude Code subagent team that researches, backtests and vets trading strategies against written criteria | Claude Code, Python, Docker |

## Backend & systems

| Repo | What | Stack |
|---|---|---|
| [WCFResponder](https://github.com/hamitsarmis/WCFResponder) | Stub server speaking WCF binary SOAP (msbin1, WS-Addressing, Deflate) for testing and reverse-engineering | ASP.NET Core |
| [concurrent-job-queue-api](https://github.com/hamitsarmis/concurrent-job-queue-api) | Multithreaded job queue behind a JWT-protected API, with a 100k-request load client | .NET 10 |
| [dotnet-quizbot](https://github.com/hamitsarmis/dotnet-quizbot) | Telegram bot that drills senior .NET interview questions; Worker Service, EF Core on SQLite, long polling | .NET 10 |

## How I work

Claude Code daily (VPS + tmux), a written spec before code, PRs even on solo repos.

[LinkedIn](https://www.linkedin.com/in/hamitsarmis)
