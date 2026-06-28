# Cao Ngoc Tau (Tàu) — Software Engineer · AI-Governed Systems

📍 Hue City, Vietnam
🌐 Portfolio: <https://taucao-ruby.github.io/my-portfolio/>

---

## About Me

I'm a **software engineer** who applies AI-agent governance workflows to control, audit, and enforce engineering quality across the systems I build.

Self-taught since 2016 (grade 10), I graduated from **Passerelles Numériques Vietnam** in Software Engineering, interned at **Unitech** (Da Nang Software Park) and **Softworld Vietnam**, and after years of rebuilding from the ground up, returned to engineering in 2025 and have been building the **Soleil Hostel** booking system — under an AI-governed workflow — ever since.

---

## What I Do

I don't just write code. I build **AI-governed engineering systems** where every change is audited, every agent is constrained, and quality is enforced automatically — not manually reviewed.

### AI Harness Governance

I designed and operationalized a full multi-agent governance framework applied end-to-end to the Soleil Hostel project:

- **Constitutional hierarchy** — CLAUDE.md → ARCHITECTURE_FACTS → CONTRACT → 17 skill files → 6 slash commands
- **MCP safety constraints** — allowlisted tools, denylist enforcement, size limits
- **Structured audit logging** — JSONL hook events for every agent action
- **Self-learning gates** — AGENT_LEARNINGS with human verification before adoption
- **4 specialist subagents** — security-reviewer, db-investigator, docs-sync, frontend-reviewer
- **Replayable verification** — `verify-control-plane.sh` proves harness health on any machine
- **30+ AI batch sessions** with zero regressions

### Backend Engineering

- Laravel 12 + React 19 TypeScript monorepo
- 1,789 backend tests (5,740 assertions) + 545 frontend tests; PHPStan Level 5 / 0 errors / 0 baseline ignores; Psalm clean (~90% inferred)
- Deadlock-aware retry with SQLSTATE classification
- Dual payments: Stripe Cashier (payment-hold + durable refund-event idempotency, TOCTOU eliminated) **and** MoMo e-wallet (in-app QR, IPN sign/verify, `(order_id, trans_id)`-UNIQUE idempotency ledger)
- PostgreSQL `no_overlapping_bookings` exclusion constraint as a database-level safety net
- Booking state machine with explicit transition validation + immutable actor snapshots
- 179/179 audit findings resolved across four audit rounds (v1–v4)

### In-Product AI Assistant (AI Harness)

- 7 `/v1/ai/*` endpoints with a 7-layer safety pipeline, kill switch, and canary routing
- Durable AI proposal lifecycle with human confirmation (proposer-binding, drift detection)
- Prompt-injection defense (AI-001), PII hard-block, and HMAC-signed audit trail
- `php artisan ai:eval` regression gate run nightly in CI — blocks deploy on failure

### Quality Enforcement

- Pre-commit hooks + `ship.sh` gate — no bypass possible
- CI pipeline: 6 parallelized jobs, booking stress test, 95% coverage gate
- Multi-stage Docker (4-stage frontend), Caddy with HSTS/CSP hardening
- Tag-based production deploy with pre-deployment gate

### Code Intelligence (Open Source)

- Forked and extended **GitNexus** — an open-source knowledge-graph engine that indexes codebases for AI agents (rebranded *soleil-ai-review-engine* in my fork)
- Contributed PHP call-graph resolution (`$this->prop->method()` edges), web server-mode agent init + OpenRouter model guard, Claude Code hook fixes, and CI/test infrastructure
- Integrated it as the code-intelligence layer (MCP tools, impact analysis, knowledge-graph queries) for graph-aware, low-risk changes on Soleil Hostel

> Built on the work of [GitNexus](https://github.com/abhigyanpatwari/GitNexus) and its contributors — my role here is fork, extension, and integration, not original authorship.

---

## Engineering Philosophy

> Code without governance is a liability. AI without constraints is a risk.
> I build systems where **the harness enforces correctness** — not hope.

I care deeply about:

- Concurrency correctness and transactional integrity
- Defense-in-depth security at every layer
- Evidence-gated quality (tests, static analysis, audit logs)
- Governance that survives team scaling and time

---

## Work History

| Period | Role | Organization |
|--------|------|--------------|
| 2025 – Present | Lead Engineer | Soleil Hostel — Booking & AI Governance System |
| 2022 – Present | Self-Directed Engineer | Independent — Backend & AI Systems |
| 2021 | Software Engineer Intern | Softworld Vietnam |
| 2021 | Software Engineer Intern | Unitech, Da Nang Software Park |

**Education:** Passerelles Numériques Vietnam — Software Engineering (2018–2021)
**Course:** KMS Technology — Spectre Module: Automation Testing (2020–2021)

---

## Contact

If you're interested in AI harness engineering, backend architecture, or the Soleil Hostel system, reach out:

👉 <https://taucao-ruby.github.io/my-portfolio/>
📧 ngoctaucao@gmail.com

---

> _"The harness enforces correctness — not hope."_
