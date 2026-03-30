# Startup Expectations

A plain-language guide to what "good" looks like at each stage of building a company — written for founders and operators, not HR departments.

Open source under Apache 2.0. Free to read, fork, embed, and build on.

---

## Start with your stage

The fastest path is to pick your current stage and work through the ordered guide.

| Stage | What it proves | Guide |
|-------|---------------|-------|
| **Pre-seed** | Problem and team are credible; first build and first learning | [Pre-seed guide →](spec/maturity/pre-seed.md) |
| **Seed** | Real traction or strong de-risking; seed round raised, early GTM | [Seed guide →](spec/maturity/seed.md) |
| **Series A** | Repeatable motion; raising to scale what already works | [Series A guide →](spec/maturity/series-a.md) |

Each guide tells you the job of the stage, what order to tackle things, what kills companies at that stage, and how to know when you're ready for the next one.

---

## Browse by topic

If you know the area you are working on, go directly to the goal.

| Topic | What it covers |
|-------|---------------|
| [Funding & runway](spec/milestones/fundraising-runway/) | Raising money, modeling burn, investor relationships |
| [Build & ship](spec/milestones/product-delivery/) | MVP scope, shipping, technical foundation, reliability |
| [Customers & revenue](spec/milestones/revenue-gtm/) | ICP, validation, pricing, GTM motion, case studies |
| [Team & hiring](spec/milestones/hiring-team/) | Founders, first hires, interview bar, operating rhythm |
| [Trust & compliance](spec/milestones/trust-compliance/) | Security, privacy, IP, compliance, incident readiness |
| [Operations](spec/milestones/operations-back-office/) | Entity, cap table, payroll, contracts, insurance |

Or see [all milestones at a glance →](spec/milestones/milestone-catalog.md)

---

## How to consume this spec

This project is designed to be readable and usable in three distinct ways.

### For humans

Read it on GitBook. Start with your stage guide, follow the phase table, and click through to individual milestone pages. Each milestone page explains what you are aiming for, what to focus on, and common ways it goes wrong — in plain language, without assumed knowledge.

### For AI agents and copilots

The spec includes a structured machine-readable layer designed for agent navigation:

1. **Start at [`spec/manifest.yaml`](spec/manifest.yaml)** — defines all entry points, schema locations, and an `agent_protocol` with explicit traversal steps
2. **Navigate by stage** via [`spec/maturity/index.yaml`](spec/maturity/index.yaml) — ordered `milestone_ids` per stage
3. **Navigate by category** via [`spec/goals/_registry.yaml`](spec/goals/_registry.yaml) — six categories with goal paths
4. **Load each milestone** via its `goal.yaml` — structured outcome data, signals, and load order
5. **Read context** via each milestone's `agent-context.md` — human-language guidance written to be unambiguous for language models

The `agent_protocol` block in `manifest.yaml` spells out the exact traversal sequence. Agents should start there rather than crawling the directory tree.

### For software and professional tools

The spec is schema-backed and index-driven. Everything a tool needs to consume it programmatically:

| File | What it provides |
|------|-----------------|
| [`spec/manifest.yaml`](spec/manifest.yaml) | Top-level entry points, schema refs, agent protocol |
| [`spec/maturity/index.yaml`](spec/maturity/index.yaml) | Ordered milestone IDs per stage, stage proof statements |
| [`spec/milestone-index.yaml`](spec/milestone-index.yaml) | Flat index of all milestones with metadata |
| [`spec/goals/_registry.yaml`](spec/goals/_registry.yaml) | Category registry with goal paths |
| `spec/milestones/<category>/<id>/goal.yaml` | Per-milestone structured data: outcomes, signals, stage tags |
| `spec/schema/goal.schema.json` | JSON Schema for validating goal files |

The YAML files are stable and versioned (`version: "1.0.0"` in manifest). If you build tooling on top of this spec, pin to a release tag rather than main to avoid unexpected changes.

---

## What each goal page includes

Every goal has a short page covering:

- **What you are aiming for** — the outcome in plain language
- **What to focus on** — the 2–3 things that move the needle at this stage
- **What to worry less about** — what does not belong in this milestone
- **How expectations change** — what this milestone means for your team and role

---

## License — Apache 2.0

This project is licensed under the [Apache License, Version 2.0](LICENSE).

**What that means in plain language:**

| You can | You must | You cannot |
|---------|----------|------------|
| Use this freely — commercially or otherwise | Include a copy of the Apache 2.0 license with any distribution | Use this project's name or marks to endorse your product |
| Modify and build derivative works | State clearly which files you changed | Hold contributors liable for damages |
| Distribute copies or derivatives | Retain all existing copyright and attribution notices | — |
| Sublicense and sell | — | — |
| Use in AI training, agent systems, or embedded tooling | Attribute the source if you distribute the output | — |

The full license text is in [`LICENSE`](LICENSE). The [Apache 2.0 FAQ](https://www.apache.org/licenses/LICENSE-2.0) covers edge cases.

**Attribution format for derivatives or redistributions:**

```
Based on Startup Expectations (https://github.com/adsingh/startup-expectations-spec-1)
Licensed under Apache 2.0
```

---

## Contributing

To add or improve a milestone, see the [schema reference](spec/schema/goal.schema.json) and open a pull request. Machine-readable indexes live in `spec/goals/_registry.yaml` and `spec/milestone-index.yaml`.
