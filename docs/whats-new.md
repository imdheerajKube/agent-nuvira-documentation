# What's new

A curated index of **feature** releases. Fix-level detail stays in the private repository:
those entries name the exact defect they repair, which is useful to an engineer and a target
list to anyone else.

## What the current line is about

- **The agent verifies its own work.** An edit that nothing checked can no longer be
  reported as done; an unverified edit is recorded and the agent gets one corrective nudge
  naming what would settle it.
- **Long unattended jobs finish, and account for themselves.** Per-batch cost and latency
  are reported on every completion path — including a request that arrived over a messaging
  channel, so a job run from WhatsApp is as measurable as one run from the terminal.
- **Every number means what it says.** A listing count is never presented as a capability,
  and a progress percentage means the deliverable exists rather than that a counter ran out.
- **Routing is consistent and honest.** The rationale, the decision and the ranked table
  always agree, and a provider/model pair that cannot work is retired and re-probed instead
  of costing a doomed round trip.
- **One engine behind every surface.** CLI, dashboard and all messaging channels share the
  same pipeline, tool surface and router.

## Feature releases

| Version | Headline |
|---|---|
| `v3.3.0` | An authored artifact lands on disk instead of in the reply, the loop engine leaves a reviewable trace, and a long unattended run accounts for what it cost |
| `v3.2.0` | The agent VERIFIES its own work, finishes long unattended jobs, and every number on the Models page means what it says |
| `v2.7.0` | Agentic capability assessment closure (engine routing, loop skill hints, DAG telemetry, model-level gates) |
| `v1.80.0` | Model-first routing, tiered failover, 1-token warmup, tool-level modality routing |
| `v1.78.0` | Contact-centric gateway messaging, Bedrock onboarding, Telegram auto-registration |
| `v1.77.0` | Dynamic model catalog, Bedrock provider, website refresh |
| `v1.76.1` | Model Discovery Timeline panel |
| `v1.76.0` | Improved folder browser, Telegram auto-learning, and Getting Started wizards |

## Versioning

Agent-Nuvira follows semantic versioning. The CLI reports its version with
`nuvira --version`.
