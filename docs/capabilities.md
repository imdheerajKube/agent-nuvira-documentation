# Capabilities

What Agent-Nuvira can do beyond "write a file". Every count here is produced by a command
you can run yourself.

| Surface | Size | Command |
|---|---|---|
| Agent tools | **110** | `nuvira tools list` |
| CLI command entries | **289** across **48** groups | see [Full Command Surface](reference/commands-surface.md) |
| Inference providers | **22** | `nuvira provider list` |
| Messaging platforms | **22** | `nuvira gateway status` |
| Skills | **155** on disk | `nuvira skills list` |
| Workflow templates | **10** built in | `nuvira workflow list` |
| Dashboard pages | **22** | see the [User Manual](user-manual.md#5-the-dashboard) |

## Coding

Plan, implement, review, test and publish. `nuvira execute` runs a multi-agent pipeline;
`nuvira workflow run` runs a fixed one; `nuvira chat` is the interactive surface. Every
mode shares one tool surface and one router.

## Beyond coding

- **Browser automation** — drive a real page: open, click, type, extract, screenshot.
- **Vision** — describe screenshots, diagrams and photos via a local Ollama model or a free
  vision tier.
- **Image and video generation** — from a prompt, saved to the artifact directory.
- **Voice in both directions** — synthesize speech and transcribe audio locally.
- **Desktop control** — screenshot, mouse and keyboard without stealing focus.
- **Sandboxed code execution** — run code under time and resource limits.
- **Document extraction** — PDF, DOCX, XLSX, PPTX, HTML, CSV.
- **Assessment of other repositories** — shallow-clone a repo into an ephemeral cache and
  work on it without touching your own workspace.
- **Integrations** — Docker, Microsoft Graph (mail/calendar/OneDrive), Home Assistant,
  Discord, Feishu docs and drive, kanban boards.
- **Scheduling and supervision** — cron jobs and long-lived daemons under the agent's
  control.
- **Sub-agents** — delegate a focused subtask to a fresh, isolated context and get the
  summary back.

## Messaging

Twenty-two platforms, from Telegram and Slack to SMS, IRC and Home Assistant. Inbound
messages are dispatched through the **same pipeline** as the CLI, and progress plus the
final result are sent back to the channel. Two independent permission lists govern who may
*trigger* the agent and who may direct it to *send* to other people.

## Knowledge and memory

Trajectory memory, fact memory, coding-pattern extraction and failure lessons. Vector
retrieval keeps long contexts affordable — the reference machine measured **142,493 tokens
saved at a 65.6% average reduction** across 64 calls.

## Extension

- **Skills** — reusable, parameterised execution plans.
- **Workflows** — fixed pipelines you can search, install, publish.
- **MCP** — connect external tool servers, or expose the agent's own tools *as* an MCP server.
- **Plugins** — providers, agents and workflow templates.
- **SDK** — build custom agents.
- **Federation** — connect remote agent instances, including A2A.

## Verification and governance

Per-step traces, an evaluation framework, model benchmarks, a CycloneDX software bill of
materials, security scanning for injection and PII, an admin governance policy (allow/deny
providers and models, hard cost cap, privacy floor), and RBAC.

## Try it without spending a token

```bash
nuvira doctor                              # full environment diagnosis
nuvira tools list                          # the 110 tools, with descriptions
nuvira skills search docker                # find a skill by need
nuvira skill run security-audit --dry-run  # print the plan, run nothing
nuvira workflow list                       # the ten built-in pipelines
nuvira intent resolve "stop the dashboard" # plain English -> exact command
nuvira code-map src                        # symbol map of a directory
nuvira retrieval stats                     # measured token savings
```
