# Feedback loop and metrics

**Stage:** Seed · **Category:** Customers & revenue

> Instrument your product and run a regular cadence of customer contact so learning is continuous, not episodic.

---

## What you are aiming for

A setup where product usage data, customer feedback, and churn signals flow into a regular review, and that review drives product decisions. Not a dashboard nobody reads. Not customer interviews that happen once and get forgotten. A consistent practice that makes the team smarter every week.

## What to focus on

- **Instrument before you invite users** — if you launch without analytics, you'll spend the first month guessing what users actually did; set up event tracking before the first private beta invite
- **Pick 2–3 metrics that matter** — activation rate, retention at 30 days, and weekly active users cover most early products; avoid the vanity metrics (total signups, page views) that look good and tell you nothing
- **Talk to customers on a cadence, not just when something breaks** — a standing call with 3–5 active users every two weeks generates more signal than a survey sent to everyone once a quarter
- **Treat churn as a signal, not a failure** — every customer who cancels or stops using the product has a reason; find out what it is before their memory fades

## Deprioritize for now

- A comprehensive analytics platform with 50 tracked events — start with 5–10 events that cover the critical path
- NPS surveys at pre-seed — NPS is a lagging indicator and meaningless with fewer than 30 respondents
- Automated churn prediction models — you don't have enough data; talk to churned customers directly

## What to instrument

**The critical path:** the sequence of actions a user must complete to get value from the product. Track every step.

| Event type | Examples | Why it matters |
|------------|----------|----------------|
| Activation | "Completed first task", "Invited first teammate" | Are users reaching value? |
| Engagement | "Used feature X", "Returned after 7 days" | Are users finding the core value? |
| Friction | "Abandoned at step 3", "Error on page X" | Where are users getting stuck? |
| Revenue | "Upgraded plan", "Cancelled subscription" | Is the business working? |

**Tools worth knowing:**
- [Mixpanel](https://mixpanel.com) or [Amplitude](https://amplitude.com) — event-based product analytics; pick one, set up the critical path events, nothing else initially
- [PostHog](https://posthog.com) — open-source alternative; self-hostable if data residency matters
- [Sentry](https://sentry.io) — error tracking; catches what users experience but don't report

## The feedback cadence

**Weekly:**
- Review the key metrics from the previous week
- Check for error spikes, unusual drop-offs, or usage pattern changes
- One standing question: "What do users keep failing to do?"

**Bi-weekly:**
- One call with an active customer; not a support call — a learning call
- One asynchronous check-in with churned or inactive users
- Update the product decision log with what you learned

**Monthly:**
- Review retention cohorts — are month-2 users retaining at the same rate as month-1 users?
- Review the pattern of cancellation reasons — is there a theme?
- Decide what changes based on data from this month

## Reading churn signals

| Signal | What to investigate |
|--------|-------------------|
| User never activates after signup | Onboarding failure; the critical path has a step they can't complete |
| User activates then goes quiet | Core value not delivered; they tried it, it didn't work for them |
| User active then suddenly cancels | Something changed — in the product, in their situation, or in a competitor's offer |
| User pays then downgrade or cancels | Pricing or value mismatch; what they expected and what they got diverged |

## Quality levels

| Level | What it looks like |
|-------|--------------------|
| **L0 — No instrumentation** | No analytics; no customer contact cadence; decisions made by gut |
| **L1 — Basic analytics** | Critical path events tracked; team can see activation and retention data |
| **L2 — Regular cadence** | Weekly metrics review; bi-weekly customer calls; churn reasons documented |
| **L3 — Metrics driving decisions** | Product decisions traced to specific data points; retention improving measurably quarter over quarter |

## How this connects to other goals

- **Shipping your MVP** — instrument before shipping to [private beta](../../../product-delivery/shipping-mvp/README.md); you can't learn from users you can't observe
- **First paying users** — first customers are the source of the earliest signal; the feedback loop should be running before [first paying users](../first-paying-users-design-partners/README.md) are onboarded
- **Pricing and packaging** — usage data tells you which features drive retention; that drives which features to put in which tier in [pricing and packaging](../pricing-and-packaging/README.md)
- **Milestones that unlock the next round** — Series A investors will ask for retention data; this practice produces it

{% hint style="success" %}
**Done when:** You can answer "what percentage of users who signed up last month are still active today and why?" — and that answer is informing what the team builds next.
{% endhint %}

## Resources

- [Mixpanel guides](https://mixpanel.com/blog) — practical guides on event tracking setup and interpreting retention data
- [Reforge: Retention](https://www.reforge.com) — the most rigorous curriculum on product retention; expensive but the free content (blog, podcast) is worth reading at this stage
- [Lenny's Newsletter: Metrics](https://www.lennysnewsletter.com) — search "retention" and "activation" for practitioner breakdowns of what metrics matter at each stage
