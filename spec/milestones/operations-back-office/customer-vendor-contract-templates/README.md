# Customer and vendor contract templates

**Stage:** Seed · **Category:** Operations

> Stage-appropriate contract templates protect you in customer deals and vendor relationships without creating the legal overhead of a company ten times your size.

---

## What you are aiming for

A small library of reusable contract templates — a customer Master Service Agreement (MSA), an order form, a Data Processing Agreement (DPA), and a vendor Statement of Work (SOW) — that your lawyer approves once and you use for every deal thereafter. Not bespoke contracts for every customer. Consistent templates that are fast to execute and defensible in a dispute.

## What to focus on

- **One approved template beats ten bespoke contracts** — custom contracts for every customer create legal overhead and inconsistent terms; a standard MSA with an order form is the right default for B2B SaaS
- **Start with your paper, not theirs** — whenever possible, send your contract first; negotiating from a customer's standard form almost always results in worse terms for you
- **Get lawyer approval once, use forever** — paying a lawyer to review your MSA template is a one-time cost; paying a lawyer to review every customer's redlines is a recurring cost that scales with deal volume
- **A DPA is not optional if you process EU data** — GDPR requires a DPA between you and your customers if you process their data; having a standard one ready removes a common deal blocker
- **Know what you're signing for vendors** — vendor contracts have auto-renewal clauses, data processing terms, and liability caps; understand each before signing

## Deprioritize for now

- Highly negotiated enterprise terms — at seed, most customers will sign a clean standard form; enterprise procurement with redlines is a Series A problem
- Intellectual property indemnification clauses in detail — understand the basics, but extensive IP indemnity negotiation happens at enterprise deal sizes
- Custom SLA terms per customer — use one SLA standard and put it in your MSA; per-customer SLAs create operational and legal complexity

## The minimum contract library

**Customer-facing documents:**

**MSA (Master Service Agreement)**
The governing contract for the customer relationship. Covers:
- License grant (what the customer can do with your product)
- Payment terms (net 30 standard; net 60 for enterprise)
- Limitation of liability (cap your liability; this is the most important clause)
- Indemnification (each party indemnifies the other for their own breach)
- Term and termination
- Governing law and dispute resolution

**Order form**
Attached to the MSA for each deal. Covers:
- Subscription tier, seats, or usage volume
- Pricing and payment schedule
- Contract start and end dates
- Renewal terms (auto-renew with notice period is standard)

**DPA (Data Processing Agreement)**
Required under GDPR when you process EU personal data on behalf of customers. Covers:
- What personal data you process and for what purpose
- Your obligations as data processor
- Sub-processor list (your own vendors)
- Security measures
- Data subject request handling

**Vendor-facing documents:**

**Vendor SOW (Statement of Work)**
For contractors, agencies, and professional services. Covers:
- Scope of work and deliverables
- Timeline and milestones
- Payment terms
- Intellectual property ownership (ensure all work product is assigned to the company)
- Confidentiality

## Getting templates

At seed stage, you have several options:

- **Lawyer-drafted templates** — the highest quality; one-time cost of $1,500–$3,000 for a startup lawyer to draft an MSA + order form + DPA
- **YC's standard documents** — YC makes its standard SAFE and some other documents public; not a full contract library but a starting point
- **Clerky or Stripe Atlas** — these services often include basic commercial contract templates for their customers
- **Online templates** — use with caution; free templates are often missing key clauses or use unfavorable defaults; always have a lawyer review before using in a deal

## Common mistakes

- **No limitation of liability clause** — without this, you could be liable for consequential damages far exceeding the contract value; always cap liability at 12 months of fees
- **No IP assignment in vendor contracts** — a vendor who writes code for you without an IP assignment clause retains ownership; get it in writing
- **Auto-renewing vendor contracts you've forgotten about** — audit vendor contracts annually; identify auto-renewal dates and set calendar reminders 60 days in advance
- **Signing customer paper without reading it** — customers sometimes send their own MSA; read it before signing; their contract is written for their benefit, not yours

## Quality levels

| Level | What it looks like |
|-------|--------------------|
| **L0 — No templates** | Each deal uses ad hoc documents or verbal agreements; terms inconsistent |
| **L1 — Basic MSA** | A standard MSA exists and is used for customer deals; lawyer has reviewed it |
| **L2 — Full library** | MSA, order form, DPA, and vendor SOW exist; used consistently; lawyer-approved |
| **L3 — Operational** | Templates updated annually; deal cycle shortened by standard terms; legal overhead per deal is minimal |

## How this connects to other goals

- **Cap table hygiene** — vendor IP assignment is part of the cap table story; investors in diligence will ask whether all IP is properly owned; [cap table hygiene](../cap-table-hygiene/README.md)
- **Security and privacy posture** — DPAs are part of both your security posture and your contract library; [security and privacy posture](../../trust-compliance/security-and-privacy-posture/README.md) determines what the DPA needs to say
- **Investor pipeline and diligence** — investors will review your standard contracts in diligence; well-drafted templates signal operational maturity

{% hint style="success" %}
**Done when:** You have a lawyer-approved MSA, order form, DPA, and vendor SOW — and every customer and vendor deal uses one of these templates rather than a bespoke document.
{% endhint %}

## Resources

- [Bonterms: Open-source commercial contracts](https://bonterms.com) — free, lawyer-drafted open-source commercial contract templates; the Cloud Terms are widely used in B2B SaaS and a good starting point for your MSA
- [Clerky: Legal documents for startups](https://www.clerky.com) — plain-English guides to commercial contract basics; useful for understanding what clauses mean before negotiating them
- [Stripe Atlas: Legal resources](https://stripe.com/atlas) — Atlas customers get access to a library of startup legal documents; GDPR DPA template is particularly useful
