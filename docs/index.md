![Agent-Nuvira](assets/logo.svg){ width="76" }

# Agent-Nuvira — Documentation

Agent-Nuvira is a **multi-agent AI coding CLI**. It plans, writes, reviews, tests and
publishes code using local models (Ollama) or cloud APIs, and it is reachable from a
terminal, a web dashboard, or any of 22 messaging platforms.

> **This repository is documentation only.** The source code lives in a private repository.
> Everything here is written to be runnable and checkable against a published build.

## Start here

- **[User Manual](user-manual.md)** — install, configure, and use every surface in depth.
- **[Capabilities](capabilities.md)** — what it can do beyond writing code.
- **[Command Reference](commands.md)** — curated commands with examples.
- **[Full Command Surface](reference/commands-surface.md)** — all 289 command entries,
  generated from the live CLI tree.
- **[Architecture](architecture.md)** — how the execution engine is put together.
- **[What's New](whats-new.md)** — the 3.x release index.

## The shape of it

| Surface | Size |
|---|---|
| Agent tools | **110** |
| CLI command entries | **289** across **48** groups |
| Inference providers | **22** |
| Messaging platforms | **22** |
| Skills | **155** |
| Built-in workflow templates | **10** |
| Dashboard pages | **22** |

## Design commitments

1. **Verify before claiming.** The agent may not report work it has not checked.
2. **No telemetry.** Requests go to the model providers you configure and nowhere else.
3. **Local-first.** Ollama and local models are a first-class path, not a fallback.
4. **One engine, every surface.** The CLI, the dashboard and every messaging channel share
   the same pipeline, tools and router.

## Install

```bash
npm install -g agent-nuvira
nuvira doctor
nuvira chat "explain what this project does"
```

Requires Node **>= 18.18.0**.

- This repository: [github.com/imdheerajKube/agent-nuvira-documentation](https://github.com/imdheerajKube/agent-nuvira-documentation)

> There is no public source repository. The site and this page are the published surface;
> issues and corrections are welcome here.
