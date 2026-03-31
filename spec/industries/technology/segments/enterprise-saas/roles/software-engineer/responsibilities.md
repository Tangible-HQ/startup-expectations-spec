# Software engineer — enterprise SaaS

Read [shared expectations](../../../../../../shared/roles/software-engineer/responsibilities.md) first. This file adds what changes when your software is sold to businesses with security reviews, compliance requirements, and uptime expectations.

---

## At pre-seed

No additions to shared. Enterprise context isn't relevant until you have a customer.

---

## At seed

**Security as a baseline practice**
- Treat security hygiene as part of the definition of done: no secrets in code, proper access controls, input validation
- Enterprise buyers will eventually audit what was built early; habits set now are cheaper than fixes later

**Multi-tenancy awareness**
- If building a shared platform, understand the data isolation model and apply it consistently
- Mistakes in tenant isolation are the most damaging class of bug in enterprise SaaS — understand the architecture before building on top of it

---

## At Series A

**Compliance and audit support**
- Understand which parts of the system you own are in scope for SOC 2 or equivalent; implement and maintain the relevant controls
- Write code and configuration that is auditable — changes tracked, access logged, behavior observable

**Enterprise customer expectations**
- Features that affect enterprise customers (permissions, audit logs, SSO, data export) are higher stakes than they appear; test them rigorously
- Reliability in your ownership area is a customer commitment, not just a team preference; treat on-call and incident response as part of the job
