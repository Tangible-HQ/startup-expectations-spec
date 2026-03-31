# Cap table hygiene

**Stage:** Pre-seed → Seed · **Category:** Operations

> Keep your ownership structure clean, understandable, and free of surprises — so founders, employees, and investors all know what they own.

---

## What you are aiming for

A cap table that any founder, lawyer, or investor can read in 10 minutes and understand completely — no mystery shares, no missing vesting schedules, no SAFEs with unclear conversion terms. Clean from the start; maintained as you grow.

## What to focus on

- **Use dedicated software from day one** — spreadsheets break under the complexity of SAFEs, conversions, and option grants; [Carta](https://carta.com) or [Pulley](https://pulley.com) cost less than the legal bill to fix a spreadsheet error
- **Get vesting right before the first raise** — missing or incorrect founder vesting is the most common cap table problem that delays or kills early funding conversations
- **Model dilution before issuing anything** — run a fully diluted model before issuing SAFEs or options; surprises at conversion are founder errors, not investor tricks
- **Keep the option pool honest** — over-promising equity to recruits is a cap table disaster waiting to happen; know how many shares exist before making offers

## Deprioritize for now

- Complex liquidation preference analysis — understand it, but you don't need to model it at pre-seed
- Secondary transactions and employee liquidity programs — those are Series B+ problems

## Key concepts

**Fully diluted shares:** total shares outstanding plus all options, warrants, and convertible instruments as if they had all converted or exercised. This is the number that matters for ownership percentage calculations.

**Option pool:** shares reserved for employee equity grants. Investors often require a specific option pool size before closing a priced round — usually 10–20% of the post-money fully diluted cap table. Understand the dilutive impact before agreeing to a pool size.

**SAFE conversion:** a SAFE converts into equity at the next priced round. The conversion price depends on the valuation cap and discount. Multiple SAFEs at different caps create a conversion waterfall — model it before your seed round closes, not during.

**409A valuation:** an independent appraisal of the fair market value of common stock, required before issuing stock options. Issuing options without a 409A creates tax liability for employees. A 409A typically costs $1,500–$3,000 and is valid for 12 months or until a material event.

## What to track

Every instrument on the cap table should be documented with:

| Instrument | What to record |
|------------|---------------|
| Founder shares | Number of shares, issue price, vesting schedule, cliff date, acceleration provisions |
| SAFEs | Amount invested, valuation cap, discount, MFN clause, investor name |
| Options | Grant date, number of shares, exercise price, vesting schedule, expiry date, grantee |
| Convertible notes | Principal, interest rate, maturity date, conversion terms, investor name |

## Common errors to fix now

- **No vesting on founder shares** — fix before any financing; investors will require it
- **Shares issued before incorporation** — not legally valid; re-issue after incorporating
- **Options issued without a 409A** — creates tax problems for employees; get a 409A before the next option grant
- **SAFE terms not modelled at conversion** — run the conversion math before signing a SAFE; understand what each investor will own at your likely Series A valuation
- **Option grants made verbally** — all equity must be documented in writing and signed; verbal promises are not enforceable and create conflict

## Quality levels

| Level | What it looks like |
|-------|--------------------|
| **L0 — Untracked** | No dedicated software; shares issued informally; no vesting documentation |
| **L1 — Tracked** | Cap table software in use; founder shares documented with vesting schedules |
| **L2 — Clean** | All instruments recorded; option pool set; 409A current; SAFE conversions modelled |
| **L3 — Audit-ready** | Any investor or lawyer can review the cap table and find no errors or missing documents; fully diluted model current |

## How this connects to other goals

- **Company financial backbone** — the legal entity from [company financial backbone](../company-financial-backbone/README.md) is a prerequisite; you can't issue shares without a legal entity
- **Co-founder alignment** — equity splits and vesting schedules should be decided in [co-founder alignment](../../hiring-team/co-founder-alignment/README.md) before the cap table is set up
- **Early financing rounds** — SAFEs and convertible notes add to the cap table with each financing; model conversions in [early financing rounds](../../fundraising-runway/early-financing-rounds/README.md) before signing
- **Investor pipeline and diligence** — cap table is one of the first documents investors review in diligence; surprises here delay or kill closings

{% hint style="success" %}
**Done when:** Your cap table is in dedicated software, every instrument has complete documentation, founder vesting is in place, and you can run a fully diluted ownership calculation in under five minutes.
{% endhint %}

## Resources

- [Carta: Cap table education](https://carta.com/learn) — the most comprehensive free library on cap tables, option pools, SAFEs, and dilution; practical and specific
- [Clerky: Equity basics](https://www.clerky.com) — plain-English guides to equity issuance, vesting, and 409A requirements
- [YC SAFE primer](https://www.ycombinator.com/documents) — covers SAFE conversion mechanics including the conversion waterfall in detail
