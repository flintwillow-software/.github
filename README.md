# flintwillow-software/.github

Organization-wide GitHub templates for `flintwillow-software`.

## Structure

Templates live in `.github/.github/ISSUE_TEMPLATE/` — the double `.github` is required for org-wide propagation.

### Available Templates

| Template | Label | Use For |
|----------|-------|---------|
| 🐛 Bug Report | `bug` | Reporting bugs with reproduction steps |
| ✨ Feature Request | `enhancement` | Proposing new features or enhancements |
| 📐 Epic | `epic` | Large initiatives spanning multiple issues/repos |
| 📋 Task | — | Discrete, actionable work items |

### Template Fields

All templates include:

- **Issue Type** — maps to your Projects v2 "Issue Type" field
- **Priority** — P0 (Critical) through P3 (Low)
- **Size** — XS through XL (effort estimate)
- **Component / Repo** — which repo or component is affected

### Adding New Templates

1. Create a new markdown file in `.github/ISSUE_TEMPLATE/`
2. Include the standard fields (`issue_type`, `priority`, `size`, `component`)
3. Add a `name` at the top of the file (this is what shows in the chooser)
4. Optionally add a `labels` field for auto-labeling
5. Commit and push — templates propagate automatically

### Propagation

Templates apply to all **public** repos in the org. Private repos inherit if the org `.github` repo is public.

To verify: create a "New issue" in any repo and check the template chooser.
