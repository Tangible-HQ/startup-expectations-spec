# Incident readiness

**Stage:** Seed · **Category:** Trust & compliance

> When something breaks in production — and it will — you need a response plan ready before it happens, not improvised in the middle of an outage.

---

## What you are aiming for

A documented, practised incident response process: who gets called, how the team coordinates during an outage, how customers are communicated with, and how you learn from the incident so it doesn't happen the same way twice. At seed, this is lightweight — but it needs to exist before you have paying customers depending on your uptime.

## What to focus on

- **Define "incident" before you have one** — any event that degrades service for customers qualifies; data loss, extended downtime, and security breaches are incidents regardless of root cause
- **One person is on-call at all times** — even a team of two can rotate; the first responder should be able to triage without waking up the whole team
- **A status page is a trust signal** — customers checking a status page during an outage are less likely to call; a public status page shifts the communication burden from reactive to proactive
- **Post-mortems are how you improve** — a blameless post-mortem after every significant incident produces the institutional learning that prevents the next one; skip it and you'll replay the incident
- **Customer communication is part of incident response** — an outage your customers notice without a message from you damages trust more than the outage itself

## Deprioritize for now

- PagerDuty or OpsGenie — appropriate when on-call rotation involves more than 3 people or incidents are frequent
- Automated incident management platforms — a Slack channel and a runbook are sufficient at seed
- SLA-driven incident classification with SLO tracking — important at Series A; at seed, the classification is "is the product working for customers, yes or no?"

## The minimum incident response plan

**Step 1 — Detection**
How do you find out before a customer tells you?
- Uptime monitoring: [Better Uptime](https://betteruptime.com), [UptimeRobot](https://uptimerobot.com), or Datadog synthetic monitoring
- Error rate alerting: alert when error rate exceeds baseline by 3x
- On-call rotation: one engineer primary, one secondary; rotates weekly

**Step 2 — Triage**
The on-call responder:
- Confirms whether customers are affected (yes/no)
- Estimates severity: cosmetic bug, degraded performance, complete outage, data issue
- Decides whether to escalate to the founding team

**Step 3 — Communicate**
- Update the status page within 15 minutes of confirmed customer impact
- For paying customers with known impact: personal email or Slack within 30 minutes
- Tone: factual, specific, and avoid guessing at resolution time

**Step 4 — Resolve**
- Document actions taken in a shared incident Slack channel or doc as you go
- If the fix requires a deployment: follow your change management process; don't rush and compound the issue
- Update the status page when resolved

**Step 5 — Post-mortem (within 48 hours)**
- What happened, when, and who was affected?
- What caused it? (technical root cause, not human blame)
- What would have caught this earlier?
- What changes are we making?

## Status page setup

A status page takes 30 minutes to set up and is one of the highest-trust signals to enterprise buyers. Options:

- [Atlassian Statuspage](https://www.atlassian.com/software/statuspage) — the most common; free tier is sufficient at seed
- [Better Uptime](https://betteruptime.com) — includes monitoring + status page in one tool
- [Instatus](https://instatus.com) — lightweight, fast to set up, generous free tier

Keep it public. Customers should be able to check it without logging in.

## Customer communication templates

Prepare these before you need them. Adapt to the specific incident.

**Acknowledgement (send within 15–30 minutes of confirmed impact):**
> We're aware of an issue affecting [feature/service]. We're investigating and will provide an update within [time]. We're sorry for the disruption.

**Update (send every 30–60 minutes during extended outage):**
> Update on the [feature] issue: [current status]. Our team is working to resolve this. Next update by [time].

**Resolution:**
> The [feature] issue has been resolved as of [time]. All systems are operating normally. We'll share a full post-mortem within 48 hours.

## Quality levels

| Level | What it looks like |
|-------|--------------------|
| **L0 — Reactive** | No on-call; outages discovered by customers; no status page; no post-mortem |
| **L1 — Basic coverage** | On-call rotation running; uptime monitoring in place; status page live |
| **L2 — Documented process** | Incident playbook written; customer communication templates ready; post-mortems running |
| **L3 — Learning system** | Every incident produces a post-mortem; action items tracked and closed; MTTD and MTTR improving over time |

## How this connects to other goals

- **Technical foundation** — the observability built in [technical foundation](../../product-delivery/technical-foundation/README.md) is what enables detection; alerting and logging are prerequisites for incident response
- **Reliability and support ops** — [reliability and support ops](../../product-delivery/reliability-support-ops/README.md) sets uptime and support SLAs; incident readiness is how you meet those SLAs when things go wrong
- **Security and privacy posture** — security incidents (data breach, unauthorised access) are a specific category of incident; the [security posture](../security-and-privacy-posture/README.md) determines the likelihood; this milestone determines the response

{% hint style="success" %}
**Done when:** You have an on-call rotation, a public status page, written customer communication templates, and you've run at least one blameless post-mortem on a real or simulated incident.
{% endhint %}

## Resources

- [PagerDuty: Incident response guide](https://response.pagerduty.com) — the most comprehensive free incident response guide available; the core process applies even if you don't use PagerDuty
- [Google SRE Book: Incident management](https://sre.google/sre-book/managing-incidents/) — Google's Site Reliability Engineering book is free online; the incident management chapter is the canonical reference for post-mortems and on-call design
- [Atlassian: Incident management for high-velocity teams](https://www.atlassian.com/incident-management) — Atlassian's free guide is practical and startup-appropriate; their post-mortem template is widely used
