# Milestone content status

Two different questions get mixed together:

| Question | What it means |
|----------|----------------|
| **Template** | Is the page still the **short stub** (old sections only), or the **expanded** layout (`## What to focus on`, deprioritize, quality levels, …)? |
| **Publication** | Is the writing **ready for general readers** on GitBook and the open repo, or still **draft** (needs review, polish, legal pass, or internal-only nuance)? |

A page can be **expanded** and still **not public-ready**. Stubs are never public-ready in a meaningful sense, but some non-stub pages also stay in draft until you say otherwise.

---

## 1. Stub pages (structural — auto-detect)

These still use the placeholder sections (`## Focus on`, `## Worry less about (for this milestone)`, `## How this changes expectations`). They need a full rewrite into the expanded template.

| Category | Milestone folder |
|----------|------------------|
| Funding & runway | [`fundraising-runway/board-investor-reporting-rhythm`](milestones/fundraising-runway/board-investor-reporting-rhythm/README.md) |
| Funding & runway | [`fundraising-runway/wind-down-or-acqui-hire-optionality`](milestones/fundraising-runway/wind-down-or-acqui-hire-optionality/README.md) |
| Operations | [`operations-back-office/insurance-d-and-o-epli`](milestones/operations-back-office/insurance-d-and-o-epli/README.md) |
| Build & ship | [`product-delivery/deep-tech-r-and-d-milestones`](milestones/product-delivery/deep-tech-r-and-d-milestones/README.md) |
| Build & ship | [`product-delivery/product-surface-expansion`](milestones/product-delivery/product-surface-expansion/README.md) |
| Build & ship | [`product-delivery/pivot-or-scope-cut`](milestones/product-delivery/pivot-or-scope-cut/README.md) |
| Build & ship | [`product-delivery/hardware-and-physical-goods`](milestones/product-delivery/hardware-and-physical-goods/README.md) |
| Customers & revenue | [`revenue-gtm/international-expansion`](milestones/revenue-gtm/international-expansion/README.md) |
| Customers & revenue | [`revenue-gtm/community-or-open-source`](milestones/revenue-gtm/community-or-open-source/README.md) |
| Customers & revenue | [`revenue-gtm/early-gtm-motion`](milestones/revenue-gtm/early-gtm-motion/README.md) |
| Customers & revenue | [`revenue-gtm/partnerships-and-channels`](milestones/revenue-gtm/partnerships-and-channels/README.md) |
| Customers & revenue | [`revenue-gtm/first-case-studies`](milestones/revenue-gtm/first-case-studies/README.md) |
| Trust & compliance | [`trust-compliance/ethics-and-misuse`](milestones/trust-compliance/ethics-and-misuse/README.md) |
| Trust & compliance | [`trust-compliance/regulatory-industry-rules`](milestones/trust-compliance/regulatory-industry-rules/README.md) |
| Trust & compliance | [`trust-compliance/dual-mission-structure`](milestones/trust-compliance/dual-mission-structure/README.md) |
| Trust & compliance | [`trust-compliance/compliance-for-your-market`](milestones/trust-compliance/compliance-for-your-market/README.md) |
| Team & hiring | [`hiring-team/remote-and-global-hiring`](milestones/hiring-team/remote-and-global-hiring/README.md) |
| Team & hiring | [`hiring-team/advisors-versus-operators`](milestones/hiring-team/advisors-versus-operators/README.md) |
| Team & hiring | [`hiring-team/immigration-and-work-authorization`](milestones/hiring-team/immigration-and-work-authorization/README.md) |

**Refresh stub list:**

```bash
rg -l '## Worry less about \(for this milestone\)' spec/milestones
```

When a page is expanded, remove its row from this table (or rely on the command until the table is empty).

---

## 2. Draft — not for public consumption (editorial — you maintain)

These are pages that **already have real content** (they may or may not use the expanded template) but are **not** treated as finalized for public readers. Reasons vary: copy not reviewed, examples too company-specific, legal/compliance wording pending, or you want another editorial pass before promoting GitBook.

**How to track (pick one or combine):**

| Approach | When to use |
|----------|-------------|
| **A. This table** | Central list; good for planning and PM-style tracking. Add a row per path and a short note. Remove the row when the page is public-ready. |
| **B. Marker in the file** | Put the following as the **first line** of the milestone `README.md` (HTML comments do not render on GitBook/GitHub): `<!-- publication-status: draft -->`. Remove the line when the page is public-ready. **Find all drafts:** `rg 'publication-status: draft' spec/milestones` |
| **C. Visible banner** | If readers should see a warning on GitBook, add a GitBook hint under the title, e.g. `{% hint style="warning" %}**Draft** — Not finalized for general readers.{% endhint %}`. Remove when shipped. |

### Draft pages (add rows below)

| Path | Note |
|------|------|
| *— Add milestones here as you audit; or rely on `publication-status: draft` in files —* | |

---

## Other paths

- **`spec/goals/**/README.md`** — Some goals duplicate milestone text with the old stub shape; canonical narrative lives under **`spec/milestones/`**.
