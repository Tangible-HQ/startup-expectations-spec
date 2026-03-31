# CTO — shared expectations

Owns the technical direction of the company and the engineering team that executes it. At pre-seed the CTO is almost always a co-founder writing most of the code. By Series A the role has shifted almost entirely to leadership, strategy, and external credibility. The transition between these modes is one of the hardest personal changes a founding CTO makes.

---

## At pre-seed

The CTO at pre-seed is the builder. Speed and learning matter more than anything else.

**Building**
- Write most or all of the production code; this is expected and correct at this stage
- Make all technical decisions: stack, infrastructure, architecture — optimize for speed and the ability to change direction, not for scale
- Ship the MVP and iterate fast; the cost of the wrong technical decision is low when you can rewrite in a week

**Technical judgment**
- Choose tools and platforms you know well, not the most interesting ones — familiarity compounds; novelty costs time
- Avoid premature abstraction and over-engineering; the code that matters is the code that tests the hypothesis
- Keep infrastructure simple: a managed database, a single cloud provider, no custom tooling until the need is proven

**Co-founder dynamic**
- Be the co-founder who translates between what's technically possible and what the business needs
- Make technical tradeoffs visible to the CEO — timeline, cost, and risk should be legible to your co-founder
- Set the earliest technical norms: code organization, deployment process, basic security hygiene

**What to skip:** formal architecture reviews, technical roadmaps, documentation beyond what you need to work, hiring processes.

---

## At seed

The CTO at seed is transitioning from sole builder to technical lead — still writing code, but now also hiring, reviewing, and setting the bar for others.

**Building and reviewing**
- Shift from writing all code to writing the hardest code and reviewing the rest
- Own the architecture decisions that will be expensive to undo: data model, API design, service boundaries
- Set up the basics of engineering practice: code review, CI/CD, basic monitoring, on-call coverage

**Hiring**
- Define what "good engineering" looks like at this company before the first interview
- Evaluate technical candidates directly — the CTO owns the engineering bar at seed
- Make the first 2–4 engineering hires; these people set the culture for everyone who follows

**Technical direction**
- Identify the technical risks that could threaten the business and have a plan for each
- Begin the infrastructure decisions that will matter at 10x current scale — not building for it yet, but knowing the path
- Own the security and data handling posture as enterprise customers begin to ask about it

**What to skip:** formal engineering management processes, career ladders, full-time platform engineering — these are seed-extension or Series A problems.

---

## At Series A

The CTO at Series A is a leader and strategist. Most production code is written by others. The CTO's leverage is in the decisions that are expensive to undo and the team that makes everything else possible.

**Technical strategy**
- Own the multi-year technical direction: build vs. buy decisions, platform bets, architectural evolution
- Manage technical debt as a business risk — prioritize it, staff it, and communicate it to the board in terms they understand
- Set the engineering team's relationship to reliability, security, and compliance

**Engineering leadership**
- Manage engineering managers directly or through a VP Eng; either way, own the culture and bar of the org
- Drive the engineering hiring plan in partnership with the CEO and finance
- Build a path for engineers to grow; retention at Series A depends on people believing they have a future

**External credibility**
- Represent the technical vision to investors, enterprise customers, and strategic partners
- Lead technical diligence conversations during fundraising and enterprise sales
- Own the company's security posture externally — sign off on security reviews, pen test results, and compliance programs

**The CTO-to-VP-Eng question**
- Many companies hire a VP Engineering to manage the engineering org so the CTO can focus on strategy and architecture
- This is a healthy evolution, not a demotion — the decision should be made based on where the CTO adds most value, not ego
- If you hire a VP Eng, define the split clearly: who owns the team, who owns the technical direction, and how disagreements are resolved
