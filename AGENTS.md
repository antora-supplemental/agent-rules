# antora-supplemental org overlay

Shared rules and Cursor skills live in **dev-centr/agent-rules**. This repo is the org overlay only - it does not vendor a snapshot.

When assembling context for this org's repos, resolve:

- `AGENT_RULES_PATH` = `$CODE_ROOT/github.com/dev-centr/agent-rules`
- Org overlay = this `AGENTS.md`

Shared changes: PR `dev-centr/agent-rules`. Org-only: commit here.

## Rewrite era (default stack)

Unless the user or task explicitly names **antora-solidstart**, **antora-next** (deprecated alias), **SolidStart docs shell**, **content manifest**, or **asciidoctor-d engine**, assume **Antora 3 static generate** — `@antora/site-generator`, Handlebars UI bundles, facto-stack, site-rebuild v1/v2, SoftNav on static HTML.

When antora-solidstart triggers match, load dev-centr skill **`antora-solidstart`** first; do not default to Antora 3 extension wiring or `antora-org-site` hub steps. Implementation repo: https://github.com/antora-supplemental/antora-solidstart[antora-solidstart^].

Canonical proposal (Pattern C split artifact): https://docs.antora-supplemental.org/docs/ROOT/proposals/antora-next-shell.html — source `docs/modules/ROOT/pages/proposals/antora-next-shell.adoc` in repo `antora-supplemental/docs`.
