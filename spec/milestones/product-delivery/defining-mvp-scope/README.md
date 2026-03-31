# Defining MVP scope

**Stage:** Pre-seed · **Category:** Build & ship

> Decide what to cut so you can ship something real, testable, and fast — not a smaller version of your full vision.

---

{% hint style="warning" %}
**Do this before writing code.** Scope without a written hypothesis is just a feature list. A feature list without cuts is a roadmap. A roadmap is not an MVP.
{% endhint %}

## What you are aiming for

A written scope — with an explicit hypothesis, a single primary job-to-be-done, and a documented non-goals list — that a small team can ship in 6–10 weeks. The scope is done when you can explain what you're testing, not just what you're building.

## What to focus on

- **Write the hypothesis first** — "We believe [ICP] will [do X] because [reason]"; if you can't write it, you're not ready to scope; everything in the MVP must serve observing whether this is true
- **One job-to-be-done** — the MVP delivers exactly one thing for exactly one customer type; scope that serves two ICPs or two jobs is twice as hard to ship and half as useful for learning
- **Cut by asking "does this help us learn?"** — not "is this useful?" or "would users want this?"; useful features that don't test the hypothesis belong on the roadmap, not the MVP
- **Write the non-goals list** — explicit decisions about what you're not building are as valuable as the scope itself; they prevent the conversations that slow you down mid-build
- **Time-box the scope** — if a pre-seed team can't ship it in 6–10 weeks, the scope is too large; cut more

## Deprioritize for now

- Nice-to-have features that don't affect whether the hypothesis is true or false
- Multiple user types or use cases — pick the ICP you validated and build for them only
- Production-grade reliability, scale, or polish — that comes after the hypothesis is confirmed
- Admin tooling, settings pages, and account management — manual ops are fine at this stage

## How to scope an MVP

**Step 1 — Restate the hypothesis from your discovery interviews:**
> "We believe [specific ICP from ICP and wedge] will [complete this job] because [reason from PSV interviews]. We'll know we're right if [observable signal]."

**Step 2 — Identify the minimum product that produces the observable signal:**
Ask: what is the smallest thing a user must be able to do for you to observe whether the hypothesis is right or wrong? That's your scope.

**Step 3 — Cut everything else:**
Go through every feature on your list. For each one, ask: "If we don't build this, can we still observe the signal?" If yes, cut it. If no, keep it.

**Step 4 — Write the non-goals:**
List at least five things you are explicitly not building in this version. If you can't name five, you haven't cut enough.

**Step 5 — Gut-check the timeline:**
Can your current team ship this in 6–10 weeks? If not, go back to step 3.

## Quality levels

| Level | What it looks like |
|-------|--------------------|
| **L0 — No scope** | Building whatever feels right; no written hypothesis; no explicit cuts |
| **L1 — Feature list** | Features identified but no hypothesis; no non-goals; scope likely too large |
| **L2 — Scoped** | Hypothesis written; one primary JTBD; non-goals documented; fits within team capacity |
| **L3 — Validated scope** | Scope tested against ICP feedback; team aligned; build started with clear ship criteria |

## How this connects to other goals

- **ICP and wedge** — the wedge defines the one job the MVP must deliver; if [ICP and wedge](../../revenue-gtm/icp-and-wedge/README.md) isn't done, you don't have a hypothesis to scope around
- **Problem–solution validation** — your discovery interviews are the cut list; features your target customers didn't mention are candidates to remove; don't scope before you have interview data from [PSV](../../revenue-gtm/problem-solution-validation/README.md)
- **Technical foundation** — scope decisions directly affect stack and infrastructure choices; a narrower scope often means simpler infrastructure; finalize scope before committing to technical decisions
- **Shipping your MVP** — this milestone produces the scope document that [shipping your MVP](../shipping-mvp/README.md) executes against; the ship milestone is about quality and learning, not re-litigating scope

## Team impact

The hardest part of scope definition is not deciding what to build — it's defending the cuts. Every stakeholder, advisor, and early user will suggest additions. The job of whoever owns scope is to say no clearly and repeatedly, with the hypothesis as the reason. "That's not what we're testing in this version" is a complete answer.

{% hint style="success" %}
**Done when:** You can fill in this template completely: "We're building [one specific thing] for [specific ICP] that lets them [one primary job]. We'll know it worked if [observable signal]. We are explicitly not building [at least 5 things] in this version." If any blank is vague, the scope is not done.
{% endhint %}

## Resources

- [The Lean Startup — Eric Ries](https://theleanstartup.com) — the original framing of MVP as a learning vehicle, not a product; chapters 3–5 are directly applicable to scope definition
- [Intercom on Starting Up](https://www.intercom.com/resources/books) — practical essays on scope decisions at early-stage; particularly strong on the cost of building features before validating them
- [Shape Up — Basecamp](https://basecamp.com/shapeup) — a detailed methodology for scoping and pitching work; useful once you have a team; the appetite concept (time-boxing scope) is directly applicable at MVP stage
- [Y Combinator: How to Build an MVP](https://www.startupschool.org) — Michael Seibel's YC Startup School lecture is the most direct talk on MVP scope decisions; search "how to build an MVP"
