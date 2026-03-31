# Beta and launch paths

**Stage:** Pre-seed → Seed · **Category:** Build & ship

> Sequence your release phases with explicit criteria between them — not a single big launch you're not ready for.

---

## What you are aiming for

A staged release path from private beta through public launch, with a defined criterion for moving between each phase and a plan for what happens if something goes wrong. The goal is to expand your user base in proportion to your ability to support and learn from them.

## What to focus on

- **Gate phases with criteria, not dates** — moving from private to public beta because "it's been 6 weeks" is not a criterion; moving because "10 private users completed the core job without hand-holding" is
- **Grow the user base slower than you think you should** — inviting 500 users when you can support 50 doesn't accelerate learning; it creates noise and support burden
- **Have a rollback plan** — know how you'll take the product offline or limit access if something breaks; the plan is most useful when you need it immediately
- **Prepare customer communication before you need it** — draft the email you'll send if there's an outage before launch, not during

## Deprioritize for now

- A perfect launch — a quiet release to 20 users who give honest feedback beats a big launch to 500 users who churn silently
- Press and PR at private beta — save media attention for when the product is ready for it
- Public metrics dashboards — wait until you have numbers worth showing

## The phases

**Private beta (invited users only)**
- 10–50 users maximum; people you can email directly
- Goal: confirm the core job works without hand-holding; find the critical path failures
- Exit criteria: a meaningful percentage of invited users complete the core job; you understand why the rest didn't

**Limited beta (controlled expansion)**
- 50–500 users; may include a waitlist or referral mechanism
- Goal: test reliability under real load; validate that learning from private beta translated into improvements
- Exit criteria: reliability is acceptable for the user population; support volume is manageable; you know your activation rate

**Public launch**
- Open access; may include a Product Hunt or Hacker News launch
- Goal: validate acquisition channels; generate initial awareness; stress-test onboarding
- Exit criteria: not applicable — public launch is a marketing event, not a product gate

## Waitlists and early access

A waitlist is a tool for managing demand and building anticipation — not a validation signal. Thousands of waitlist signups with no one completing the core job after launch is not success.

**When a waitlist makes sense:** when you genuinely cannot onboard everyone at once and want to sequence who gets access. **When it doesn't:** as a vanity metric or a substitute for actually talking to users.

## Launch channels

| Channel | Best for | What to prepare |
|---------|----------|-----------------|
| Product Hunt | Developer tools, consumer products, design-focused products | Demo video, tagline, hunter relationship, day-of presence |
| Hacker News Show HN | Technical products, developer tools, anything unusual | Clear explanation of what it does and why you built it |
| Direct outreach | B2B, niche markets | 50 personalised emails beats a mass blast |
| Community posts | Niche verticals (Slack groups, subreddits, forums) | Context-specific framing; don't cross-post identically |

## Quality levels

| Level | What it looks like |
|-------|--------------------|
| **L0 — No plan** | Building toward an undefined "launch"; no phasing; no rollback plan |
| **L1 — Private cohort identified** | First 10–20 users selected; invitations sent; feedback process in place |
| **L2 — Private beta running** | Users active; exit criteria defined for moving to limited beta; support process in place |
| **L3 — Public launch executed** | Limited beta completed with exit criteria met; public launch executed; acquisition channels tested |

## How this connects to other goals

- **Shipping your MVP** — beta phases build directly on the [MVP ship levels](../shipping-mvp/README.md); L1 private beta maps to L1 private cohort in the ship framework
- **Feedback loop and metrics** — each beta phase produces data; [feedback loop and metrics](../../revenue-gtm/feedback-loop-metrics/README.md) should be instrumented before inviting private beta users
- **Reliability and support** — limited beta is when reliability expectations start to matter; have [reliability and support](../reliability-support-ops/README.md) at a basic level before expanding beyond private beta
- **Positioning and story** — public launch requires a clear one-liner and website; [positioning and story](../../revenue-gtm/positioning-and-story/README.md) should be done before any public-facing launch

{% hint style="success" %}
**Done when:** You have moved through at least private beta with a defined cohort, learned something that changed the product, and have a documented criterion for when you're ready to expand access.
{% endhint %}

## Resources

- [Do Things That Don't Scale — Paul Graham](http://paulgraham.com/ds.html) — the canonical argument for starting with a tiny, hand-held private beta rather than optimising for scale from launch
- [Lenny's Newsletter: How to launch on Product Hunt](https://www.lennysnewsletter.com) — search "Product Hunt" for a practitioner breakdown of what actually drives successful launches
