# CTO — enterprise SaaS

Read [shared expectations](../../../../../../shared/roles/cto/responsibilities.md) first. This file adds what changes when your customers are businesses with security reviews, compliance requirements, and uptime expectations baked into contracts.

---

## At pre-seed

No additions to shared. Enterprise context isn't relevant until you have a customer or a clear enterprise ICP.

---

## At seed

**Security and compliance from the start**
- Enterprise buyers will ask about security practices before signing even a pilot agreement; know what you have and what you don't
- Basic security hygiene at seed: access controls, secrets management, audit logs, dependency scanning — these are table stakes, not advanced practice
- Begin tracking what you'd need for SOC 2 — not to complete it at seed, but so the work isn't a surprise later

**Multi-tenancy and data isolation**
- If you're building a shared platform, data isolation between customers is an architectural decision made early that's expensive to fix later
- Enterprise buyers will ask whether their data is separated from other customers'; have a clear answer

**Customer-facing reliability**
- Enterprise pilots come with implicit uptime expectations even when not in the contract
- Set up basic monitoring and have a process for communicating outages to affected customers

---

## At Series A

**Security program ownership**
- Own the engineering side of SOC 2 or equivalent: access controls, change management, incident response, vendor reviews
- Coordinate with whoever owns legal and infosec on audit timelines, pen test scheduling, and customer questionnaire responses
- Security is now a sales enablement function as much as a risk function — treat it that way

**Enterprise diligence**
- Lead technical diligence conversations during Series B fundraising and enterprise sales processes
- Be prepared to walk sophisticated buyers through architecture, data handling, and disaster recovery
- Maintain documentation that supports diligence without requiring the CTO to be present for every review

**Reliability at scale**
- Own SLA commitments to enterprise customers — know what you've promised and whether you can keep it
- Build incident response practices that include customer communication and post-mortem culture
