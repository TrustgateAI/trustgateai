# Trustgate AI

**The self-hosted trust plane for agentic AI.**

Trustgate AI is a self-hosted AI security gateway that inspects and governs every
surface of your AI agents, with zero data egress.

It runs inside your own VPC. No prompt, no document, no tool call and no response
ever leaves your infrastructure.

---

## Your agent has six doors. Most tools watch one.

| # | Surface | What gets through it |
|---|---------|----------------------|
| 1 | **Prompt** | Instructions hidden in user input |
| 2 | **RAG / retrieval** | Instructions hidden in documents the agent reads |
| 3 | **Tool / MCP calls** | Actions the agent is tricked into taking |
| 4 | **Session / memory** | Planted content that persists in agent memory |
| 5 | **Agent-to-agent** | Work and permissions handed between agents |
| 6 | **Response / egress** | Sensitive data leaving in the output |

A prompt firewall watches door one. An output filter watches door six. The four in
between are where real incidents happen — and where most of the 2026 breach reports
land.

---

## What it does

**Defend** — Inspect every surface. Scrutiny escalates with threat.

**SHASHU**, the detection engine, learns what normal looks like for each agent and
raises its own scrutiny when something looks hostile: NORMAL to ELEVATED to STRICT,
then back down once the threat clears. **Cedar** sits underneath it as a
deterministic, default-deny policy layer, evaluated per tool — so a detection miss
still hits a closed door.

**Prove** — Real-time posture, cryptographic audit trail.

Every decision is written to a hash-chained log with daily seals. You can show an
auditor what the agent was allowed to do, what it tried, and what was stopped.

**Control** — Per-agent budgets, real-time throttle.

**Contain** — Runs in your VPC. Zero data egress.

---

## Reference material we maintain

These are vendor-neutral and free to use, cite, or fork:

- **[Agentic AI incident log](https://github.com/trustgateai/agentic-ai-incidents)** —
  a dated, sourced record of real-world attacks carried out by or through AI agents,
  with a stated confidence level on every entry.
- **[Agentic AI attack surface](https://github.com/trustgateai/agentic-ai-attack-surface)** —
  the six surfaces, what an attack looks like at each one, and why perimeter tooling
  misses four of them.

---

## See it work

There is a guided product tour at **[trustgateai.io/demo](https://www.trustgateai.io/demo)**.
It walks a real attack through a hospital running four AI agents and shows what the
gateway does at each surface. The first chapter needs no sign-up.

---

**Website** — [trustgateai.io](https://www.trustgateai.io)
**LinkedIn** — [linkedin.com/company/trustgateai](https://www.linkedin.com/company/trustgateai/)
**Contact** — founder@trustgateai.io

Built in Cary, North Carolina.
