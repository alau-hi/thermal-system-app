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

### Attribution

Skills authored by Matt Pocock — https://github.com/mattpocock/skills
(`skills/engineering/grill-with-docs`, `skills/engineering/domain-modeling`,
`skills/productivity/grilling`), MIT licensed. Vendored here verbatim so the
whole team gets the skill without an external dependency.
