# Publishing SOP — Customer Release Notes

Maintained by the Documentation Guild.

## Repository access

The shared release catalog is read-only for delivery engineers. Never create
branches, commits or pull requests against this repository. Publish deliverables
in the delivery workspace repository provisioned in your own account; search your
repositories for a name containing `github_notion_419-delivery-workspace`.

## Deliverable layout

- Branch: `release-notes/2026-Q4`
- Files:
  - `release-notes/2026-Q4.md`
  - `release-notes/2026-Q4.json`

## Markdown conventions

- Level-1 heading: `Lumen Platform — Q4 2026 Release Notes`
- One level-2 section per group. Priority and security items are grouped together
  under `Important Updates`; every other group is named after its Component.
- Each included feature is a single bullet:
  `- **Feature name** — one-line customer-facing description in plain language.`
- Never mention internal-only, unshipped or preview features.

## Manifest conventions

`release-notes/2026-Q4.json` is a JSON object with:

```json
{
  "release": "2026-Q4",
  "items": [
    {
      "feature": "Feature name",
      "component": "Component",
      "section": "Important Updates",
      "priority": "P0",
      "security_related": true
    }
  ]
}
```
