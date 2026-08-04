# Portfolio decisions

This directory holds approved decisions that affect more than one CMDC project
or define the portfolio operating model.

Use `templates/DECISION.md` for new records. Name records with a date and short
slug, for example `2026-08-04-eight-repository-model.md`.

## Decision index

| Date | Decision | Status |
|---|---|---|
| 2026-08-04 | Keep HQ plus seven independently bounded product/design repositories | Approved; recorded below |

## 2026-08-04 — Eight-repository operating model

The CMDC ecosystem will keep eight repositories rather than form a monorepo:
HQ, CMDC, Budget, Wonky Zipper, Ledger, Stat, Design, and Chat.

HQ is the coordination layer and contains no application code. Repository
identities will be normalized in deliberate phases that preserve existing
history and uncommitted work. Conversation memory is not canonical; committed
repository documentation is.
