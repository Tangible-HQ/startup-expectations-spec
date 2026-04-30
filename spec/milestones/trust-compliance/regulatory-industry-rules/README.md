# Regulatory and industry rules

**Stage:** Series A · **Category:** Trust & compliance

> Most founders discover sector-specific regulations the first time a customer's legal team sends a vendor questionnaire — map your regulatory landscape before that moment, not during a deal.

---

## What you are aiming for

A documented view of which sector-specific regulations apply to your business, what they require, and what the consequences of non-compliance are. Not full compliance across every possible regulation — that's usually impossible to achieve pre-revenue — but clarity on which rules are license-to-operate requirements, which are customer-driven, and which you can address on a timeline.

## What to focus on

- **Map what applies before you need to comply** — regulations vary by industry, jurisdiction, and business model; the first step is a clear inventory of which rules touch your product, your customers, and your data
- **Distinguish license-to-operate from aspirational** — some regulations are gates: you can't operate without them (e.g. a money transmitter license to process payments); others are competitive differentiators or customer requirements (e.g. SOC 2); others are background obligations you must maintain (e.g. GDPR); know which is which
- **Customer requirements are often the practical driver** — regulated customers (hospitals, banks, insurers, government agencies) have their own compliance obligations and will push them down to you via vendor questionnaires and contract terms; map your customer base's industry before mapping your own obligations
- **Get a specialist, not a generalist** — a startup lawyer who does IP and employment is not the right person for HIPAA or broker-dealer regulations; one conversation with a specialist in your industry's regulatory framework is worth more than 10 with a generalist
- **Track ongoing obligations, not just one-time filings** — most regulations create continuing obligations: annual audits, recurring disclosures, reportable events; build these into your ops calendar

## Deprioritize for now

- Seeking certification or licensure in every jurisdiction simultaneously — sequence by where your customers are and where regulations are most restrictive
- Building your own compliance programme before you've hired or contracted someone with the relevant expertise — build on existing frameworks and professional guidance, not from scratch
- Over-indexing on future regulations that haven't taken effect — monitor them, but don't build compliance programmes for rules that aren't law yet

## Industry regulatory map

### Financial services (fintech, payments, lending, insurance)

| If you... | Regulation / license |
|-----------|---------------------|
| Transmit money between parties | Money Transmitter License (MTL) — required in most US states; the Nationwide Multistate Licensing System (NMLS) tracks these |
| Provide investment advice | Registered Investment Adviser (RIA) registration — SEC or state-level |
| Originate or broker loans | State lending licenses; CFPB oversight for consumer lending |
| Underwrite or sell insurance | Insurance producer license by state |
| Operate in the EU with financial data | PSD2, MiCA (for crypto), local central bank registration |

**Rule of thumb:** If money moves through your product, assume you need a license. Getting this wrong is expensive.

### Healthcare and life sciences

| If you... | Regulation |
|-----------|-----------|
| Handle Protected Health Information (PHI) | HIPAA — Business Associate Agreement (BAA) required with covered entities; Security Rule compliance required |
| Provide clinical decision support or diagnostic tools | FDA Software as Medical Device (SaMD) classification may apply |
| Conduct or support clinical research | IRB (Institutional Review Board) oversight; FDA 21 CFR Part 11 for electronic records |
| Operate in the EU with health data | GDPR special category data rules; CE marking for medical devices |

**Rule of thumb:** If a doctor or patient uses your product and health data flows through it, get a healthcare regulatory attorney on a call before you sign a hospital contract.

### Education

| If you... | Regulation |
|-----------|-----------|
| Handle student records at K-12 schools | FERPA — educational records may not be shared without consent |
| Collect data from children under 13 | COPPA — requires verifiable parental consent in the US |
| Work with EU students | GDPR, potentially with additional national education data rules |

### Government and public sector

| Requirement | Description |
|-------------|------------|
| FedRAMP | Cloud services used by US federal agencies require FedRAMP authorisation — a 12–18 month process minimum |
| ITAR / EAR | Defense-related technology or exports may trigger ITAR (International Traffic in Arms) or EAR (Export Administration Regulations) obligations |
| StateRAMP | Some US states have their own cloud security requirements for vendors |

### Horizontal regulations (apply across industries)

| Regulation | Applies when |
|-----------|-------------|
| GDPR | You have users or process data of EU residents |
| CCPA / CPRA | California users; revenue > $25M or large volumes of personal data |
| SOC 2 | Enterprise customers require it; not a regulation but treated as one in B2B sales |
| ADA / WCAG | Web accessibility; WCAG 2.1 AA is effectively required for government customers and increasingly for enterprise |

## How to build your regulatory inventory

1. **List your industries** — what sector do your customers operate in? what sector do you operate in?
2. **Map the data you handle** — financial data, health data, personal data, children's data, education records
3. **Map your geographies** — where are your customers? where are your users? where do you process data?
4. **Identify license-to-operate requirements** — regulations without which you simply cannot operate legally in your market
5. **Get specialist review** — one call per regulatory domain; document what you learn

## Quality levels

| Level | What it looks like |
|-------|--------------------|
| **L0 — Unknown** | No view of which regulations apply; reacting to customer questionnaires and vendor reviews without a framework |
| **L1 — Inventory done** | Written list of which regulations apply, which are license-to-operate, and which are ongoing obligations |
| **L2 — Compliant on gates** | License-to-operate requirements met; customer-driven compliance addressed; obligations on an ops calendar |
| **L3 — Proactive programme** | Regulatory changes tracked; annual review of obligations; specialist counsel on retainer for the two or three most material regulatory domains |

## How this connects to other goals

- **Compliance for your market** — [compliance for your market](../compliance-for-your-market/README.md) is where HIPAA, SOC 2, and ISO certifications live; this milestone is about mapping the full regulatory landscape; the two are complementary
- **Security and privacy posture** — data regulations (GDPR, HIPAA, CCPA) overlap with security requirements; [security and privacy posture](../security-and-privacy-posture/README.md) builds the controls; this milestone maps the legal obligations
- **Customer and vendor contract templates** — regulated customers will require compliance representations in contracts; [customer and vendor contract templates](../../operations-back-office/customer-vendor-contract-templates/README.md) is where those representations should be standardised

{% hint style="success" %}
**Done when:** You have a written inventory of which regulations apply to your business, have confirmed which are license-to-operate requirements, and have a named plan (or active compliance) for each one — reviewed with at least one specialist attorney in the relevant domain.
{% endhint %}

## Resources

- [Stripe Atlas: Regulatory compliance guide](https://stripe.com/atlas/guides) — Stripe's plain-English guides to financial regulation for startups; one of the most accessible starting points for fintech regulation
- [IAPP: Privacy law reference](https://iapp.org) — the International Association of Privacy Professionals maintains a jurisdiction-by-jurisdiction map of privacy regulations; free to access
- [HHS: HIPAA for businesses](https://www.hhs.gov/hipaa) — the US Department of Health and Human Services' own guidance for HIPAA compliance; start here before engaging a healthcare regulatory attorney
- [NMLS Resource Center](https://www.nmlsconsumeraccess.org) — state licensing requirements for money services businesses; searchable by state and license type
