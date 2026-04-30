# Startup Expectations

A plain-language guide to what "good" looks like at each stage of building a company — written for founders and operators, not HR departments.

[![GitHub Stars](https://img.shields.io/github/stars/Subtext-labs/startup-expectations-spec?style=social)](https://github.com/Subtext-labs/startup-expectations-spec)
[![GitHub Forks](https://img.shields.io/github/forks/Subtext-labs/startup-expectations-spec?style=social)](https://github.com/Subtext-labs/startup-expectations-spec/fork)
[![License](https://img.shields.io/badge/license-Apache%202.0-blue)](LICENSE)
[![Last commit](https://img.shields.io/github/last-commit/Subtext-labs/startup-expectations-spec)](https://github.com/Subtext-labs/startup-expectations-spec/commits/main)

**[Read on GitBook →](https://subtext-2.gitbook.io/startup-expectations-specifications)** · **[Star on GitHub](https://github.com/Subtext-labs/startup-expectations-spec)** · Built by [Amandeep Singh](https://github.com/adsingh)

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

Read it on [GitBook](https://subtext-2.gitbook.io/startup-expectations-specifications). Start with your stage guide, follow the phase table, and click through to individual milestone pages. Each milestone page explains what you are aiming for, what to focus on, and common ways it goes wrong — in plain language, without assumed knowledge.

### For AI agents and copilots

The spec includes a structured machine-readable layer designed for agent navigation:

1. **Start at [`spec/manifest.yaml`](spec/manifest.yaml)** — defines all entry points, schema locations, and an `agent_protocol` with explicit traversal steps
2. **Navigate by stage** via [`spec/maturity/index.yaml`](spec/maturity/index.yaml) — ordered `milestone_ids` per stage
3. **Navigate by category** via [`spec/goals/_registry.yaml`](spec/goals/_registry.yaml) — six categories with goal paths
4. **Load each milestone** via its `goal.yaml` — structured outcome data, signals, and load order
5. **Read context** via each milestone's `README.md` — human-language guidance written to be unambiguous for language models

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
- **What to deprioritize** — what does not belong in this milestone
- **Quality levels** — L0 through L3 so you know where you stand
- **How this connects** — cross-links to related milestones

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

The full license text is in [`LICENSE`](LICENSE).

**Attribution format for derivatives or redistributions:**

```
Based on Startup Expectations (https://github.com/Subtext-labs/startup-expectations-spec)
Licensed under Apache 2.0
```

---

## Contributing

Contributions help this spec stay grounded in how real teams build. For **next steps**—where to open issues and PRs, which schemas and indexes to read, and how milestone pages fit together—see **[CONTRIBUTING.md](CONTRIBUTING.md)**.

Quick links: [new issue](https://github.com/Subtext-labs/startup-expectations-spec/issues/new) · [new pull request](https://github.com/Subtext-labs/startup-expectations-spec/compare) · [goal schema](spec/schema/goal.schema.json) · [milestone catalog](spec/milestones/milestone-catalog.md)

If you find a gap — a stage, role, or scenario that's missing — open an issue describing it. Even a one-line description of what felt missing is useful.

By participating in issues, pull requests, or discussions, you agree to follow this repository’s **[Code of Conduct](CODE_OF_CONDUCT.md)** and GitHub’s [Community Guidelines](https://docs.github.com/en/site-policy/github-terms/github-community-code-of-conduct).

---

## Community and moderation

Participation here is covered by GitHub’s platform rules and by our **[Contributor Covenant Code of Conduct](CODE_OF_CONDUCT.md)** (harassment-free, professional discussion; enforcement steps are described in that file).

Maintainers may label, request changes on, close, or lock issues and pull requests; remove or reject contributions that break the CoC or derail work; and restrict repository access when needed. Reports of unacceptable behavior go through the contact path in [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md); use [GitHub’s abuse reporting](https://docs.github.com/en/communities/maintaining-your-safety-on-github/reporting-abuse-or-spam) for account or safety concerns on GitHub itself.

---

## Support this project

If **Startup Expectations Specifications** is useful to you, you can help without writing code:

- **[Star the repository](https://github.com/Subtext-labs/startup-expectations-spec)** on GitHub so more people discover it
- **Share** this README or the [GitBook](https://subtext-2.gitbook.io/startup-expectations-specifications) with founders, operators, or teams building on the spec
- **Fork** and adapt the content under Apache 2.0 for your own playbooks or products
- **Open issues and pull requests** with fixes, gaps, or industry-specific nuance (see Contributing)

Visibility and feedback keep the spec honest and widely useful.

---

*Built by [Amandeep Singh](https://github.com/adsingh) · [GitHub](https://github.com/Subtext-labs/startup-expectations-spec) · [GitBook](https://subtext-2.gitbook.io/startup-expectations-specifications) · [Code of Conduct](CODE_OF_CONDUCT.md) · Apache 2.0*
