# Ethics and misuse prevention

**Stage:** Series A · **Category:** Trust & compliance · **[conditional]**

> Define what your product can and can't be used for before a viral misuse incident forces the answer — under pressure, with less time, and in public.

---

{% hint style="info" %}
**Conditional.** This milestone applies when your product can be used to harm people, facilitate illegal activity, spread false information, target vulnerable populations, or enable large-scale abuse. The threshold is lower than most founders expect. If users can use your product to send messages, publish content, process data about people, or automate decisions, this milestone applies.
{% endhint %}

## What you are aiming for

A set of documented acceptable use policies, a realistic view of the ways your product can be misused, and a response process that doesn't require a founder to triage every incident manually. Not a perfect solution — misuse can't be fully prevented — but a posture that makes systematic abuse difficult and gives you a credible, coherent answer when it happens anyway.

## What to focus on

- **Write the acceptable use policy before you need to enforce it** — a policy written the day after a misuse incident is written under duress and tends to be either too vague to enforce or too broad to be credible
- **Enumerate your threat model for your product specifically** — "spam, fraud, and abuse" is not a threat model; "our messaging feature could be used to send phishing emails at scale" is; enumerate the realistic ways your specific product could cause harm
- **Design friction into the highest-risk surfaces** — rate limits, verification requirements, review queues, and human-in-the-loop checkpoints are cheaper than incident response; place them where the risk is highest, not everywhere
- **Build a reporting path for users** — users who witness abuse will do nothing if there's no obvious place to report it; a report form takes one day to ship and dramatically improves detection
- **Name who responds and at what threshold** — a misuse incident at 10 AM on a Tuesday is different from one that goes viral at 11 PM on a Friday; the response process needs to account for both

## Deprioritize for now

- Automated content moderation at scale before you have the data to train it — false positive rates at low volume will create as many problems as they solve
- A dedicated Trust and Safety team — at Series A, this is a function that can be owned by an engineer and a policy lead, not a department
- Exhaustive edge case coverage in your policies — write for the 80% of cases you can anticipate clearly; reserve judgment for the rest and document how you'll handle novel cases

## The acceptable use policy (AUP)

Your AUP is a legal agreement between you and your users that defines what they can and can't do with your product. At minimum, it should prohibit:

- Using the product for illegal activity
- Impersonating individuals or organisations
- Distributing spam, malware, or phishing content
- Harvesting or scraping data in ways not sanctioned by you
- Using the product to harm, threaten, or harass individuals

Make the AUP a binding part of your Terms of Service. Without that linkage, it's unenforceable. Include specific consequences: warnings, suspension, termination.

## Common misuse scenarios by product type

| Product type | Common misuse vectors |
|-------------|----------------------|
| **Messaging / email** | Spam, phishing, harassment, coordinated inauthentic behaviour |
| **AI / generation tools** | Misinformation, deepfakes, automated fraud, impersonation |
| **Payments / fintech** | Money laundering, fraud rings, synthetic identity abuse |
| **Developer APIs** | Scraping, bot traffic, credential stuffing, DDoS amplification |
| **Marketplace / two-sided** | Counterfeit goods, fake reviews, payment fraud |
| **Data / analytics** | Unauthorised use of personal data, discriminatory profiling |

## The response process

When abuse is detected or reported:

1. **Triage** — is this a policy violation? how severe? how widespread?
2. **Contain** — disable the account, rate-limit the surface, or take down the content as appropriate
3. **Investigate** — understand the scope; was this one bad actor or a pattern?
4. **Remediate** — fix the underlying vector where possible
5. **Communicate** — notify affected users if warranted; document internally what happened and what changed

Define who makes the call at each step and what the escalation threshold is for founder or legal involvement.

## Proactive vs reactive controls

| Control type | Examples | When to use |
|-------------|---------|------------|
| **Preventive** | Rate limits, CAPTCHA, email verification, access tiers | High-risk surfaces; before launch |
| **Detective** | Usage anomaly monitoring, report queues, abuse signal scoring | After you have enough volume to set thresholds |
| **Corrective** | Account suspension, content removal, IP blocks | After detection; standardise the tooling |

Start with preventive controls on your highest-risk surfaces. Detective controls require volume to be meaningful. Corrective tooling should exist before you need it, not as you're responding to an active incident.

## Quality levels

| Level | What it looks like |
|-------|--------------------|
| **L0 — No policy** | No AUP; no reporting path; misuse handled reactively case-by-case |
| **L1 — Policy written** | AUP exists and is part of ToS; basic reporting path live; someone owns responses |
| **L2 — Threat model documented** | Misuse vectors enumerated for your specific product; preventive controls on highest-risk surfaces; response process written |
| **L3 — Proactive posture** | Anomaly detection running; report queue reviewed regularly; policies updated as new abuse patterns emerge; post-mortems written for significant incidents |

## How this connects to other goals

- **Security and privacy posture** — misuse prevention overlaps with security; [security and privacy posture](../security-and-privacy-posture/README.md) addresses the protection of your systems; this milestone addresses the protection of people who use or are affected by your product
- **Incident readiness** — a misuse incident is a type of incident; the response process in [incident readiness](../incident-readiness/README.md) should include trust and safety scenarios, not just infrastructure outages
- **Regulatory and industry rules** — certain industries (financial services, healthcare, AI) have regulatory requirements that overlap with ethics and misuse; [regulatory and industry rules](../regulatory-industry-rules/README.md) covers the compliance dimension

{% hint style="success" %}
**Done when:** Your acceptable use policy is live and part of your Terms of Service, your highest-risk product surfaces have at least one preventive control, there is a named owner for misuse reports, and you have a written response process for at least your three most likely misuse scenarios.
{% endhint %}

## Resources

- [Trust and Safety Professional Association (TSPA)](https://www.tspa.org) — the industry body for trust and safety practitioners; their framework documents are free and practical even for small teams
- [Stanford Internet Observatory: Research and guidance](https://io.stanford.edu) — the most rigorous public research on online misuse patterns; useful for understanding which threats are real and which are theoretical
- [Jigsaw (Google): Harassment and abuse tools](https://jigsaw.google.com) — open-source tools and research for reducing online harms; Perspective API for toxicity detection is free for low-volume use
