# Unit economics experiments

**Stage:** Seed · **Category:** Funding & runway

> Measure CAC, LTV, and payback period early — even when the numbers aren't pretty — so you know whether the business model works before scaling it.

---

## What you are aiming for

A basic understanding of what it costs to acquire a customer, how much revenue that customer generates over their lifetime, and how long it takes to recoup the acquisition cost — grounded in real data from your first customers, not assumptions. Not a perfect model. Honest early numbers you can improve.

## What to focus on

- **Measure early, even if it's ugly** — a CAC payback of 36 months is not a reason to stop measuring; it's a reason to understand what's driving it and how to improve it
- **Use real data, not modelled assumptions** — blended averages across your first 10 customers are more useful than a perfect theoretical model with no real data behind it
- **CAC must include all costs** — marketing spend, sales time at an hourly rate, tools, and outreach costs; a CAC that only counts ad spend is a fiction
- **Track cohorts, not aggregates** — customers acquired in month 1 behave differently from customers acquired in month 6; cohort analysis reveals trends that averages hide
- **Share the numbers honestly** — Series A investors will calculate these themselves; sharing honest numbers with clear improvement plans is better than optimistic numbers that don't hold up

## Deprioritize for now

- Sophisticated multi-touch attribution models — too early; too much complexity for the data you have
- Lifetime value projections beyond 24 months — you don't have enough retention data to project beyond what you've observed

## Key metrics

**Customer Acquisition Cost (CAC):**
> Total sales and marketing spend in period ÷ new customers acquired in period

Include: paid ads, sales salaries (time allocated to new customer acquisition), outreach tools, events, content creation costs.

**Customer Lifetime Value (LTV):**
> Average revenue per customer per month × average customer lifetime in months × gross margin

Average customer lifetime = 1 ÷ monthly churn rate. If monthly churn is 5%, average lifetime is 20 months.

**CAC Payback Period:**
> CAC ÷ (average monthly revenue per customer × gross margin)

This is the number of months to recoup acquisition cost. Below 12 months is good for most SaaS. Below 18 months is acceptable. Above 24 months means either CAC is too high or revenue per customer is too low.

**LTV:CAC ratio:**
> LTV ÷ CAC

Above 3:1 is the commonly cited benchmark for healthy SaaS unit economics. Below 1:1 means you lose money on every customer.

**Gross margin:**
> (Revenue – cost of goods sold) ÷ Revenue

For SaaS, COGS includes hosting, customer success time, and third-party tools that scale with customers. Target: 60–80% for most SaaS products.

## Cohort analysis basics

A cohort is a group of customers who started at the same time. Tracking cohorts separately reveals:

- **Retention curves:** what percentage of month-1 customers are still active in month 3, 6, 12?
- **Revenue expansion:** are later cohorts paying more than earlier ones?
- **CAC efficiency:** are customers acquired in later months cheaper to acquire than early ones?

A simple cohort table in a spreadsheet — customers by acquisition month, revenue by month — is sufficient at seed stage.

## Quality levels

| Level | What it looks like |
|-------|--------------------|
| **L0 — No metrics** | No CAC or LTV calculated; business model health unknown |
| **L1 — First calculations** | CAC and LTV estimated from real data, even if rough; payback period known |
| **L2 — Cohort data** | Customers tracked by acquisition month; retention curve visible; gross margin calculated |
| **L3 — Driving decisions** | Unit economics improving measurably; pricing, acquisition channel, and customer success decisions traceable to unit economics data |

## How this connects to other goals

- **Next-round unlock milestones** — CAC payback and LTV:CAC are commonly cited Series A unlock metrics; start measuring them early enough to show improvement, not just a snapshot
- **Feedback loop and metrics** — the retention data in your [feedback loop](../../revenue-gtm/feedback-loop-metrics/README.md) is the raw material for LTV calculations; the systems should be built together
- **Pricing and packaging** — improving LTV is often about pricing; unit economics data tells you whether you're underpricing in [pricing and packaging](../../revenue-gtm/pricing-and-packaging/README.md)
- **Runway dashboard and burn reviews** — CAC is a cost; LTV is a revenue driver; both should appear in your burn review alongside cash position

{% hint style="success" %}
**Done when:** You can state CAC, LTV, CAC payback period, and gross margin with real data behind each number — and you can explain what you're doing to improve the weakest one.
{% endhint %}

## Resources

- [Andreessen Horowitz: 16 startup metrics](https://a16z.com/16-metrics) — the canonical list of metrics investors use to evaluate SaaS businesses; directly applicable for understanding what to track and why
- [OpenView: SaaS benchmarks report](https://openviewpartners.com/saas-benchmarks-report) — annual data on CAC, LTV, and payback across different SaaS categories; useful for calibrating whether your numbers are competitive
- [Reforge: Growth series](https://www.reforge.com) — the most rigorous treatment of retention and unit economics available; start with the free blog content
