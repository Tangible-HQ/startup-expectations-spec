# Contributing

## Next steps

| Step | Link |
|------|------|
| Report a gap or idea | [Open an issue](https://github.com/Subtext-labs/startup-expectations-spec/issues/new) |
| Propose an edit | [Open a pull request](https://github.com/Subtext-labs/startup-expectations-spec/compare) (fork → branch → PR from your fork) |
| See every milestone | [Full milestone catalog](spec/milestones/milestone-catalog.md) |

## What to read before you change structured content

- **Milestone goals** — [`spec/schema/goal.schema.json`](spec/schema/goal.schema.json) and each milestone’s `goal.yaml` under `spec/milestones/`
- **Roles** — [`spec/schema/role.schema.json`](spec/schema/role.schema.json) and files under `spec/shared/roles/` or `spec/industries/`
- **Indexes** — [`spec/manifest.yaml`](spec/manifest.yaml) (entry points and agent protocol), [`spec/goals/_registry.yaml`](spec/goals/_registry.yaml) (categories), [`spec/milestone-index.yaml`](spec/milestone-index.yaml) (flat list), [`spec/maturity/index.yaml`](spec/maturity/index.yaml) (milestones by stage)

Edits to indexes or schemas should stay consistent with each other; when in doubt, open an issue first.

## Plain pages (README milestones)

Many milestones are documented in `README.md` files next to `goal.yaml`. Wording-only improvements usually only need those files; adding a new milestone needs schema-valid `goal.yaml`, registry updates if applicable, and a row in the milestone catalog where appropriate.

**Content status** — [`spec/CONTENT_STATUS.md`](spec/CONTENT_STATUS.md) explains (1) **stub vs expanded** template (detectable with `rg`), and (2) **publication readiness**: pages with real content that are still **not** finalized for public readers—track those in the table there and/or with `<!-- publication-status: draft -->` at the top of a milestone `README.md`.

## Conduct

Participation is covered by the **[Code of Conduct](CODE_OF_CONDUCT.md)** and [GitHub Community Guidelines](https://docs.github.com/en/site-policy/github-terms/github-community-code-of-conduct).
