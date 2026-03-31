# Security and privacy posture

**Stage:** Seed · **Category:** Trust & compliance

> Enterprise customers will ask about your security before they sign — build a defensible posture before the first big deal, not after you lose one.

---

## What you are aiming for

A documented, practised security posture that protects customer data, gives you honest answers to enterprise security questionnaires, and doesn't require a dedicated security team to maintain. Not SOC 2 compliance (that comes later) — but the controls and practices that make SOC 2 achievable without starting from scratch.

## What to focus on

- **Know what data you hold** — you can't protect data you haven't mapped; a simple data inventory (what data, where stored, who has access, how long retained) is the foundation of everything else
- **Access control before tools** — principle of least privilege from day one costs nothing and prevents most insider risk and account takeover scenarios
- **Vendor risk is your risk** — every SaaS tool that touches customer data is your responsibility; know which vendors are sub-processors and what their security posture is
- **Write a privacy policy that's accurate** — a template privacy policy that doesn't match how you actually handle data creates legal exposure; make sure the policy reflects reality
- **Incidents will happen; prepare before they do** — see [incident readiness](../incident-readiness/README.md); the two milestones are designed to be built together

## Deprioritize for now

- SOC 2 Type II certification — pursue after Series A or when a large customer requires it
- Penetration testing — appropriate at seed only if your product handles particularly sensitive data (health, finance, identity)
- A dedicated security hire — a security-minded engineer or an outsourced fractional CISO is sufficient at seed

## The minimum viable security posture

**Identity and access:**
- SSO (Google Workspace or Okta) for all company tools; no shared passwords
- MFA required for all accounts that touch production or customer data
- Access provisioned on hire, deprovisioned on termination — same day
- Production access restricted to the minimum number of people who need it

**Data protection:**
- Data encrypted at rest (most cloud providers handle this by default — verify it's enabled)
- Data encrypted in transit (TLS 1.2+ for all endpoints)
- Customer data not stored in local developer machines or personal Dropbox/Google Drive accounts

**Vendor management:**
- List of vendors with access to customer data (your sub-processors)
- Each vendor has a DPA (Data Processing Agreement) in place — most SaaS vendors offer a standard one on request
- Vendors are reviewed annually or when a new vendor is added

**Policy basics:**
- Password manager required for all team members (1Password or Bitwarden)
- Acceptable use policy: what team members can and can't do with company data and systems
- Privacy policy on the website that accurately describes data collection and use

## Answering the enterprise security questionnaire

Most enterprise customers send a security questionnaire before signing. At seed, the honest answer for many questions is "we do X but don't have formal documentation of it yet." That is acceptable. What is not acceptable:

- Claiming controls you don't have
- Claiming certifications you haven't earned
- Leaving questions blank

A well-prepared security posture means you can answer 80%+ of a standard CAIQ or SIG questionnaire honestly and affirmatively. The remaining 20% (formal ISMS, SOC 2, pen test results) can typically be addressed with a compensating control narrative or a roadmap commitment.

## GDPR and data privacy basics

If you have customers or users in the EU, GDPR applies. The minimum:

- Privacy policy that discloses: data you collect, why, how long, who you share it with, and user rights
- A process for handling data subject requests (e.g. deletion requests)
- DPAs with all sub-processors
- Don't transfer EU data to non-EU processors without appropriate safeguards (Privacy Shield successor or Standard Contractual Clauses)

CCPA applies if you have California users and meet revenue/data thresholds — likely not relevant at early seed but worth knowing.

## Quality levels

| Level | What it looks like |
|-------|--------------------|
| **L0 — Uncontrolled** | No data inventory; shared passwords; no vendor list; no privacy policy |
| **L1 — Basic controls** | SSO and MFA in place; data inventory exists; privacy policy live |
| **L2 — Documented posture** | Sub-processor list maintained; DPAs in place; access review running; acceptable use policy shared |
| **L3 — Defensible** | Can answer an enterprise security questionnaire honestly; incident plan tested; SOC 2 readiness assessment done |

## How this connects to other goals

- **Incident readiness** — security posture and incident response are built together; [incident readiness](../incident-readiness/README.md) is what you do when the controls in this milestone fail
- **Customer and vendor contract templates** — DPAs, data processing terms, and security representations in contracts flow from this posture; [customer and vendor contract templates](../../operations-back-office/customer-vendor-contract-templates/README.md)
- **IP and trademarks basics** — intellectual property protection and data protection are related; [IP and trademarks](../ip-trademarks-basics/README.md) addresses ownership of what you build; this addresses protection of what you hold

{% hint style="success" %}
**Done when:** You have a data inventory, SSO and MFA enforced, a vendor list with DPAs in place, an accurate privacy policy, and you can answer an enterprise security questionnaire without fabricating controls.
{% endhint %}

## Resources

- [Vanta: SOC 2 guide for startups](https://www.vanta.com) — Vanta's free guide to preparing for SOC 2; even if you're not ready for certification, the control list is the best checklist for building your security posture
- [CAIQ Lite (CSA)](https://cloudsecurityalliance.org) — the standard questionnaire enterprise customers send; reading through it reveals exactly what controls matter to buyers
- [IAPP: GDPR overview](https://iapp.org) — the International Association of Privacy Professionals maintains the most reliable free GDPR guidance; start with their GDPR overview for startups
