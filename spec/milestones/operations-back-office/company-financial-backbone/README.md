# Company financial backbone

Before you raise money, hire anyone, or sign a customer contract, you need a legal entity and a functional financial setup. This is not exciting work, but skipping or deferring it creates problems that are expensive to fix later — messy cap tables, personal tax liability, or contracts that can't be enforced.

## What you are aiming for

A legal entity, a business bank account, a basic bookkeeping system, and a payroll setup — all in place before you spend meaningful money or take on meaningful obligations.

## Step 1: Legal entity

For most venture-backed startups in the US, the right entity is a **Delaware C Corporation**. This is not the only option, but it is the default that investors expect, lawyers know, and conversion from other structures is painful.

| Entity type | When it fits | When it doesn't |
|-------------|-------------|-----------------|
| Delaware C Corp | Raising venture capital, issuing equity to employees, planning to IPO or be acquired | Sole operator, no investors, no employees |
| LLC | Simple businesses, single-founder consulting, no equity grants | Issuing equity to employees or investors — LLCs can't issue stock options in the normal sense |
| S Corp | Tax efficiency for profitable small businesses | Foreign founders or investors (S Corps have ownership restrictions) |

**Practical steps:**
- Use [Stripe Atlas](https://stripe.com/atlas), [Clerky](https://www.clerky.com), or a startup lawyer for Delaware incorporation — cost is typically $500–$2,000 all-in
- File for an EIN (Employer Identification Number) immediately after — free, takes 10 minutes at irs.gov
- Register as a foreign entity in your home state if you're incorporated in Delaware but operating elsewhere

## Step 2: Business bank account

Open a dedicated business bank account immediately. Do not commingle personal and business funds — it creates legal liability and makes bookkeeping a nightmare.

Options used by most early-stage startups:
- **Mercury** — built for startups, no fees, API access, good for teams
- **Brex** — banking plus corporate cards, popular at YC-backed companies
- **Silicon Valley Bank** (now part of First Citizens) — traditional option, good for VC-backed companies
- **Chase Business** — works if you prefer a traditional bank

Get a business debit or corporate card immediately so all company expenses are automatically separated from personal.

## Step 3: Bookkeeping

You need your books closed monthly from day one. "We'll sort it out at tax time" turns a $500 problem into a $5,000 problem.

**At pre-seed:** a simple setup is sufficient.
- Use **QuickBooks Online** or **Xero** for accounting software
- Categorize every transaction as it happens — don't let it pile up
- Reconcile your bank account monthly
- Most founders handle this themselves initially; consider a part-time bookkeeper ($200–$500/month) once you have more than ~20 transactions per month

**What investors will ask to see:** a P&L (profit and loss statement), burn rate, and bank balance. These should be producible in under 5 minutes if your books are current.

## Step 4: Payroll

If any founder is taking a salary — even a nominal one — you need a payroll provider. Paying yourself via bank transfer and filing it manually is a compliance problem.

- **Gusto** — most common among early-stage startups; handles federal and state payroll tax filings automatically
- **Rippling** — more feature-rich, better for teams that will scale quickly
- **Deel** — if you have international contractors or employees from day one

Even if founders are not taking salaries yet, set up payroll before your first external hire.

## Step 5: Basic financial hygiene

A few practices to establish from day one:

- **Separate email for financial accounts** — use a role-based address (finance@yourcompany.com) rather than a personal address for all banking, payroll, and accounting logins
- **Two-factor authentication** on all financial accounts
- **Expense policy** — even informally, agree what counts as a company expense before someone buys something questionable
- **Monthly financial review** — 30 minutes once a month to review your P&L, bank balance, and burn rate; don't fly blind

## Common gotchas

- **Using a personal account for business expenses** — creates piercing of the corporate veil risk (personal liability) and makes bookkeeping retroactively painful
- **Incorporating in your home state instead of Delaware** — you'll likely need to reincorporate before raising a Series A; do it right the first time
- **Not getting an EIN immediately** — you need this for banking, payroll, and any contractor payments
- **Paying contractors without a W-9 or signed agreement** — creates tax filing problems and IP assignment gaps
- **No one owning the books** — if both founders assume the other is handling finances, the books won't get done; assign ownership explicitly

## Resources

- [Stripe Atlas: Starting a company](https://stripe.com/atlas/guides) — the most accessible plain-English guide to entity formation, EINs, banking, and the first 90 days of company operations
- [Clerky guides](https://www.clerky.com/features) — detailed walkthroughs of Delaware incorporation, founder stock, and IP assignment; used by many YC companies
- [Pilot: Startup accounting guide](https://pilot.com/blog) — Pilot is a bookkeeping service for startups; their blog has practical guides on what financial systems to set up at each stage
- [Mercury startup banking](https://mercury.com) — beyond the product, Mercury's resources section has plain-English guides on opening accounts, understanding burn, and financial basics for first-time founders
