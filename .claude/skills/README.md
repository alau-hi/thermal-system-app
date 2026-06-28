# Claude Code Skills

## grill-with-docs

A relentless interview skill that stress-tests a plan or design against the
project's own documentation, capturing the results as a domain glossary
(`CONTEXT.md`) and Architecture Decision Records (`docs/adr/`) as you go.

Invoke it with `/grill-with-docs` before starting a substantial piece of work.

### Components

- `grill-with-docs/` — entry point; runs a grilling session backed by domain modeling.
- `grilling/` — the relentless one-question-at-a-time interview.
- `domain-modeling/` — maintains the glossary and ADRs (`ADR-FORMAT.md`, `CONTEXT-FORMAT.md`).

### Updating with the skills.sh installer

These skills are tracked in [`skills-lock.json`](../../skills-lock.json) at the
repo root, sourced from `mattpocock/skills` via [skills.sh](https://skills.sh).

The skill files are committed (vendored) so they work out of the box and with no
network access. To refresh them from upstream, run from the repo root:

```bash
npx skills@latest update                 # update to latest upstream versions
# or restore exactly what the lock pins:
npx skills@latest experimental_install
```

Note: pulling/updating requires unrestricted GitHub access. Claude Code's web
sandbox scopes Git to this repo only, so run the installer from a local machine.

### Attribution

Skills authored by Matt Pocock — https://github.com/mattpocock/skills
(`skills/engineering/grill-with-docs`, `skills/engineering/domain-modeling`,
`skills/productivity/grilling`), MIT licensed. Vendored here verbatim so the
whole team gets the skill without an external dependency.
