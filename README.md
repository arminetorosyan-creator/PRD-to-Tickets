# PRD to Tickets

A Claude Code skill that turns a PRD/spec into Jira-ready Epics and Stories
with acceptance criteria, delivered as a Word (`.docx`) draft for a product
owner to review and amend — nothing is ever written to Jira directly.

## Layout

- **`.claude/skills/prd-to-tickets/SKILL.md`** — the reusable skill.
  Attach this repo (or copy the skill folder) into any Claude Code session
  and it triggers automatically when you provide a PRD and ask for it to be
  broken down into tickets.
- **`sources/`** — the original PRD/spec documents that were run through
  the skill, one subfolder per project, kept for traceability.
- **`deliverables/`** — the generated Epics/Tickets `.docx` drafts, one
  subfolder per project, mirroring `sources/`.

## Current projects

| Project | Source | Deliverable |
|---|---|---|
| Sanctions Module | [`sources/sanctions-module/Sanctions_Module_PRD_v3.0.docx`](sources/sanctions-module/Sanctions_Module_PRD_v3.0.docx) | [`deliverables/sanctions-module/Sanctions_Module_Epics_Tickets_Draft.docx`](deliverables/sanctions-module/Sanctions_Module_Epics_Tickets_Draft.docx) |

## How it works

See [`.claude/skills/prd-to-tickets/SKILL.md`](.claude/skills/prd-to-tickets/SKILL.md)
for the full process: gathering the source PRD, clarifying only real
scope blockers, deriving Epics and INVEST-quality Stories, writing
Given/When/Then acceptance criteria, and assembling the Word draft with a
summary table and an Assumptions & Open Questions section.
