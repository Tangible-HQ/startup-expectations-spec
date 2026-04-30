# Compliance for your market

**Stage:** Series A · **Category:** Trust & compliance

> Compliance is a revenue question, not just a risk question — SOC 2 or HIPAA opens enterprise deals, but only if you pursue the right certification at the right time and don't treat it as a checkbox.

---

## What you are aiming for

The specific compliance certifications and programmes your customers and contracts require — in place before a deal stalls waiting for them, and maintained as a functioning programme rather than a one-time audit. Not compliance across every possible framework — that's unachievable and wasteful at this stage — but the one or two certifications that directly unblock revenue.

## What to focus on

- **Let customers tell you what they need** — the fastest way to identify which compliance frameworks matter is to lose a deal to one, or have a customer's legal team send you a security questionnaire; track these across your pipeline before committing to a certification programme
- **SOC 2 is the default for B2B SaaS** — if you sell to enterprise software buyers, SOC 2 Type II will eventually be a requirement; start the readiness process before a customer asks, not the week they ask
- **Type I vs Type II — understand the difference** — SOC 2 Type I certifies that your controls are designed correctly at a point in time; Type II certifies that they operated effectively over a period (usually 6–12 months); customers with sophisticated security teams will ask for Type II
- **Compliance automation tools cut the time and cost significantly** — platforms like Vanta, Drata, or Secureframe reduce the time to SOC 2 readiness from 12+ months to 4–6 months and cut costs by 30–50%
- **HIPAA is not a certification — it's a programme** — there is no official HIPAA certification body; you sign a Business Associate Agreement (BAA) with covered entities and you demonstrate compliance through documented policies, controls, and risk assessments; the obligation is ongoing, not one-time

## Deprioritize for now

- Pursuing ISO 27001 before SOC 2 — SOC 2 is faster, cheaper, and more directly useful for US enterprise sales; ISO 27001 is worth pursuing when you have significant European enterprise customers or government contracts
- Starting a FedRAMP authorisation before you have a federal customer with budget — FedRAMP takes 12–18 months and $500,000–$1,000,000+; only pursue it when there is a funded government contract that requires it
- Compliance-washing — a SOC 2 report issued by a lenient auditor that doesn't reflect real controls will create more risk than no certification when a sophisticated customer reviews it

## SOC 2

**What it is:** An attestation report (not a certification) issued by a licensed CPA firm covering five Trust Services Criteria: Security, Availability, Processing Integrity, Confidentiality, and Privacy. Most customers ask for Security only.

**Type I vs Type II:**
- **Type I:** Controls designed appropriately at a specific date; takes 2–4 months to achieve; useful as an interim signal; some customers accept it
- **Type II:** Controls operated effectively over an audit period (minimum 6 months, usually 12); the version enterprise customers require; total timeline 9–15 months from starting readiness

**Timeline and cost:**
| Phase | Duration | Cost (estimate) |
|-------|----------|----------------|
| Readiness (with automation platform) | 3–5 months | $10,000–$30,000 platform + internal time |
| Type I audit | 1–2 months | $10,000–$25,000 |
| Type II observation period | 6–12 months | Running controls; no incremental cost |
| Type II audit | 1–2 months | $15,000–$40,000 |

**With compliance automation (Vanta, Drata, Secureframe):**
- Annual SaaS fee: $8,000–$30,000 depending on company size and scope
- Reduces manual readiness work by 50–70%
- Provides continuous control monitoring; makes annual renewal significantly faster

**Common SOC 2 controls:**
- Access control and multi-factor authentication
- Change management and code review process
- Logging and monitoring
- Vendor risk management
- Incident response plan (tested)
- Employee security training
- Business continuity and disaster recovery

## HIPAA

**What it is:** A US federal law (Health Insurance Portability and Accountability Act) that governs how protected health information (PHI) is handled. If you receive, store, or transmit PHI on behalf of a covered entity (hospital, insurer, healthcare provider), you are a Business Associate and must comply with HIPAA.

**What compliance requires:**
- **Business Associate Agreement (BAA)** with every covered entity customer; this is a legal prerequisite to handling their PHI — if you don't have a BAA and you're handling PHI, you're in violation
- **Security Rule:** Administrative, physical, and technical safeguards for electronic PHI
- **Privacy Rule:** Policies governing use and disclosure of PHI; minimum necessary standard; patient rights
- **Breach Notification Rule:** If a breach occurs, covered entities must be notified within 60 days; HHS may also need to be notified

**Common healthcare-specific controls:**
- Audit logging for all access to PHI
- Encryption at rest and in transit for PHI (required under Security Rule)
- Role-based access to PHI with minimum necessary principle
- Annual HIPAA risk assessment
- Workforce training on PHI handling
- BAA template reviewed by a HIPAA-specialist attorney

## PCI DSS (payment card data)

**What it is:** The Payment Card Industry Data Security Standard; required if you store, process, or transmit cardholder data.

**The fastest path:** Don't store card data. Use Stripe, Braintree, or another PCI-compliant processor that handles cardholder data and gives you a token; this reduces your PCI scope to SAQ-A or SAQ-A-EP, the two simplest compliance levels.

If you must store card data (rare): engage a Qualified Security Assessor (QSA) for a formal assessment; budget $50,000–$200,000+ and 12+ months.

## ISO 27001

**What it is:** An international standard for information security management systems (ISMS); widely recognised in Europe, the UK, and the public sector.

**When it matters:** When selling to European enterprises, UK government, or markets where ISO 27001 is a vendor requirement. US enterprise buyers generally prefer SOC 2.

**Timeline and cost:** 12–18 months; $40,000–$100,000 for initial certification including consulting and audit.

## Quality levels

| Level | What it looks like |
|-------|--------------------|
| **L0 — No programme** | No certifications; reacting to customer requests without a compliance strategy |
| **L1 — Requirements mapped** | Written list of which certifications your pipeline requires; roadmap exists for the top priority |
| **L2 — In progress** | Compliance automation platform set up; SOC 2 or HIPAA programme actively running; BAAs in place for health data customers |
| **L3 — Certifications active** | SOC 2 Type II report current; HIPAA programme documented and audited; certifications included in sales process proactively |

## How this connects to other goals

- **Security and privacy posture** — the controls in your security posture are the foundation of SOC 2 and HIPAA compliance; [security and privacy posture](../security-and-privacy-posture/README.md) should be built first; compliance programmes systematise and audit those controls
- **Regulatory and industry rules** — [regulatory and industry rules](../regulatory-industry-rules/README.md) covers the full landscape of sector-specific regulations; this milestone goes deeper on the specific certifications and programmes that require active ongoing management
- **Customer and vendor contract templates** — HIPAA BAAs, SOC 2 report sharing terms, and security representations in MSAs need to be standardised; [customer and vendor contract templates](../../operations-back-office/customer-vendor-contract-templates/README.md) is where those templates live

{% hint style="success" %}
**Done when:** You have identified the one or two compliance frameworks that gate your largest revenue opportunities, have an active programme in place for each, and can provide a current report or programme documentation to any customer who asks — without a 4-week scramble.
{% endhint %}

## Resources

- [Vanta: SOC 2 guide for startups](https://www.vanta.com/resources) — the most practical free guide to SOC 2 readiness; includes timeline, cost benchmarks, and control checklists; relevant even if you use a different automation platform
- [HHS: HIPAA for covered entities and business associates](https://www.hhs.gov/hipaa) — the authoritative source for HIPAA requirements; start with the Security Rule summary before engaging a HIPAA attorney
- [PCI Security Standards Council](https://www.pcisecuritystandards.org) — the authoritative source for PCI DSS requirements; the self-assessment questionnaires (SAQs) are free and show you exactly which controls apply to your card data scope
- [AICPA: SOC 2 overview](https://www.aicpa.org) — the accounting body that governs SOC 2; their overview of Trust Services Criteria is the definitive description of what auditors actually assess
