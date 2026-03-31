# Technical foundation

**Stage:** Pre-seed · **Category:** Build & ship

> Make the right stack and infrastructure choices for your stage — fast to ship, easy to change, secure enough not to create problems you'll regret.

---

## What you are aiming for

A working development setup that lets the team ship and iterate quickly, with enough structure to avoid the most expensive early mistakes — not a production-grade platform, not a proof of scale, just the minimum foundation that supports fast, safe development.

## What to focus on

- **Use what you know** — stack familiarity compounds; novelty costs time; pick tools your team can move fast with today
- **Separate environments from day one** — local, staging, and production should be distinct; deploying from a laptop to production is a risk not worth taking
- **Secrets management** — no credentials in code or `.env` files committed to version control; this mistake is expensive to clean up
- **Repeatable deploys** — if shipping requires manual steps only one person knows, you have a bus factor problem; automate from the start
- **Baseline security** — HTTPS everywhere, dependency scanning, basic access controls; these cost almost nothing to set up and almost everything to retrofit

## Deprioritize for now

- Microservices — a monolith is almost always the right starting point; split only when a specific scaling need justifies it
- Multi-region or high-availability infrastructure — you don't have enough users to need it
- Custom tooling — use managed services (databases, queues, auth) so you're building product, not platform
- Elaborate monitoring — basic uptime alerts and error tracking are sufficient; full observability comes later

## Key decisions to make

**Version control and CI**
- Git with GitHub, GitLab, or Bitbucket — pick one and use it for everything from day one
- A CI pipeline that runs tests and lints on every pull request; even a basic one catches regressions before they reach production

**Hosting and infrastructure**
- Managed cloud (AWS, GCP, Azure, Render, Fly.io, Railway) beats self-managed for everything at this stage
- A managed database (RDS, Cloud SQL, PlanetScale, Supabase) beats running your own Postgres server
- Choose based on what your team knows, not on what scales to 10M users

**Environments**
- Production: what real users see; no debug tools, no test data
- Staging: mirrors production as closely as possible; for testing before deploying
- Local: developer machines; can diverge from production on convenience grounds

**Secrets management**
- Never commit credentials, API keys, or passwords to version control
- Use environment variables managed via a secrets service (Doppler, AWS Secrets Manager, GitHub Actions secrets)
- Rotate any credentials that have ever been committed, even to a private repo

**Baseline security**
- HTTPS on all endpoints — managed certificates via Let's Encrypt or your cloud provider are free
- Dependency scanning — GitHub Dependabot or Snyk catches vulnerable packages automatically
- Basic access controls — who can deploy to production, who can access the database directly

## Quality levels

| Level | What it looks like |
|-------|--------------------|
| **L0 — No structure** | Code on one machine; no version control; deploying manually; no separation between dev and prod |
| **L1 — Repo and CI** | Version control in place; CI running on PRs; basic deployment process documented |
| **L2 — Environments separated** | Local, staging, and production are distinct; secrets not in code; HTTPS on all endpoints |
| **L3 — Repeatable and secure** | Automated deployments; dependency scanning running; access controls in place; another engineer can deploy without asking |

## How this connects to other goals

- **Defining MVP scope** — scope decisions directly affect infrastructure choices; finalise [MVP scope](../defining-mvp-scope/README.md) before committing to significant infrastructure decisions
- **Shipping your MVP** — the technical foundation is what you ship on top of; get it to L2 before inviting real users
- **Security and privacy posture** — baseline security here is the foundation that [security and privacy posture](../../trust-compliance/security-and-privacy-posture/README.md) builds on at seed; it's easier to start right than retrofit
- **Reliability and support** — monitoring and on-call build on top of the environment and deployment foundation set here

{% hint style="success" %}
**Done when:** Any engineer on the team can ship to production using a documented process, without asking the person who set it up — and no credentials live in version control.
{% endhint %}

## Resources

- [The Twelve-Factor App](https://12factor.net) — the canonical methodology for building portable, deployable software; configuration, backing services, and environment parity sections are directly applicable at this stage
- [GitHub Actions documentation](https://docs.github.com/en/actions) — the simplest way to set up CI/CD for most teams
- [Doppler](https://www.doppler.com) / [1Password Secrets Automation](https://1password.com/secrets) — managed secrets; easier than rolling your own from day one
