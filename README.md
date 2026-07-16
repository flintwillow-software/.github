# flintwillow-software/.github

Organization-wide GitHub templates for `flintwillow-software`.

## Structure

Issue forms live at `.github/ISSUE_TEMPLATE/*.yml`.

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

1. Create a new `.yml` issue form in `.github/ISSUE_TEMPLATE/`
2. Include structured form fields using GitHub's form schema: `dropdown`, `input`, `textarea`, `checkboxes`
3. Add a YAML frontmatter block at the top with `name:` and optional `labels:`
4. Commit and push — issue forms propagate to all org repos automatically

### Propagation

Templates apply to all **public** repos in the org. Private repos inherit if the org `.github` repo is public.

To verify: create a "New issue" in any repo and check the template chooser.
