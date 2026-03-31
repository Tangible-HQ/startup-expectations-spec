# Reliability and support

**Stage:** Seed · **Category:** Build & ship

> Define uptime targets, establish on-call coverage, and give customers a way to reach you — before an incident reveals you have none of these.

---

## What you are aiming for

A basic reliability and support setup appropriate to your current user base: monitoring that catches problems before customers report them, a defined on-call process, and a support channel that customers know how to use. Not enterprise-grade SLAs. Not a 24/7 support team. The minimum that makes you trustworthy to the customers you have.

## What to focus on

- **Monitoring before users** — set up uptime monitoring and error tracking before inviting your first beta users; customer-reported outages are worse than self-discovered ones
- **Define your uptime target honestly** — commit to what you can actually deliver; a 99.9% SLA you can't meet is worse than no SLA; start with what's achievable and raise it as infrastructure matures
- **On-call means someone is responsible** — not everyone is responsible (which means no one is); one person owns the pager at any given time, even if it's the CTO
- **Support channel must be visible** — customers should not have to hunt for how to contact you; one channel, clearly advertised, with a response time you can keep

## Deprioritize for now

- Formal SLA contracts with enterprise-grade uptime guarantees before you have the infrastructure to support them
- A dedicated support team — founders handle support at seed; it generates valuable product insight
- Status pages — useful at limited beta and above; overkill for a private cohort

## Monitoring stack

**Layer 1 — Uptime monitoring:**
- [Better Uptime](https://betteruptime.com), [UptimeRobot](https://uptimerobot.com), or [Checkly](https://www.checklyhq.com)
- Pings your endpoints every minute; alerts you (Slack, PagerDuty, SMS) when they go down
- Free tier is sufficient at early stage

**Layer 2 — Error tracking:**
- [Sentry](https://sentry.io) — catches and groups application errors; alerts on new or spiking errors
- Tells you what broke before a user reports it; essential from first beta user

**Layer 3 — Application performance:**
- [Datadog](https://www.datadoghq.com), [New Relic](https://newrelic.com), or cloud-native monitoring
- Response times, database query performance, memory and CPU usage
- Nice to have at seed; necessary at Series A

## On-call process

At seed, on-call is simple: one person carries the pager at all times and responds to alerts within a defined window.

**Minimum viable on-call:**
- Who is on call this week? (written down somewhere)
- What alerts route to them? (uptime + error spikes at minimum)
- What's the expected response time? (acknowledge within 15–30 minutes during business hours; 1 hour outside)
- What's the runbook for the most likely incidents? (even a one-page doc is enough)

**Rotation:** if there are 2+ engineers, rotate weekly; if the CTO is solo, they're always on call until the first engineering hire.

## Support channels

Pick one primary channel and commit to it:

| Channel | Best for | Response time commitment |
|---------|----------|--------------------------|
| Email (support@) | Most B2B products | Same business day |
| In-app chat (Intercom, Crisp) | Products with frequent user questions | Same business day; sub-hour when online |
| Slack shared channel | Design partners and enterprise pilots | Real-time during business hours |
| Community (Discord, Slack) | Developer tools, open-source | Best effort; community helps community |

**Don't offer all of them** — you can't maintain consistent response times across four channels with two people.

## Incident response basics

**When something breaks:**
1. Acknowledge — confirm you're aware of the issue (internal Slack, update status page if you have one)
2. Triage — is this affecting all users or a subset? Is it getting worse?
3. Fix or mitigate — fix if fast; roll back or disable the feature if it takes more than 30 minutes
4. Communicate — if customers are affected, tell them before they ask; a brief honest message beats silence
5. Post-mortem — for any incident affecting customers, write a one-page summary of what happened, why, and what changes

## Quality levels

| Level | What it looks like |
|-------|--------------------|
| **L0 — No setup** | No monitoring; no defined on-call; customers report outages by email or social media |
| **L1 — Basic monitoring** | Uptime monitoring and error tracking running; someone gets an alert when things break |
| **L2 — On-call defined** | Rotation documented; runbooks for common incidents; one support channel with a committed response time |
| **L3 — Mature practice** | Incidents trigger post-mortems; SLA defined and tracked; support metrics reviewed monthly; status page in place |

## How this connects to other goals

- **Technical foundation** — monitoring and deployments are built on top of the infrastructure from [technical foundation](../technical-foundation/README.md); get to L2 there before setting up reliability tooling
- **Beta and launch paths** — limited beta is when reliability expectations begin; have at least L1 in place before moving beyond a private cohort in [beta and launch paths](../beta-and-launch-paths/README.md)
- **Security and privacy posture** — incident response overlaps with security incident response; align the processes so you're not running two parallel playbooks
- **Customer and vendor contract templates** — SLAs in customer contracts should match what you can actually deliver; coordinate with [contract templates](../../operations-back-office/customer-vendor-contract-templates/README.md)

{% hint style="success" %}
**Done when:** You know about outages before your customers do, someone is always responsible for responding to them, and customers know how to reach you and what response time to expect.
{% endhint %}

## Resources

- [PagerDuty: Incident Response documentation](https://response.pagerduty.com) — free, open-source incident response guide; the on-call and post-mortem sections are directly applicable at this stage
- [Sentry getting started](https://docs.sentry.io) — the fastest way to get error tracking running; free tier is sufficient for most seed-stage products
- [Google SRE Book — Chapter 9: Being On-Call](https://sre.google/sre-book/being-on-call/) — the industry-standard reference for on-call practices; read the first half; the second half is for much larger teams
