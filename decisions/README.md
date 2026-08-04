# Portfolio decisions

This directory holds approved decisions that affect more than one CMDC project
or define the portfolio operating model.

Use `templates/DECISION.md` for new records. Name records with a date and short
slug, for example `2026-08-04-eight-repository-model.md`.

## Decision index

| Date | Decision | Status |
|---|---|---|
| 2026-08-04 | Keep HQ plus seven independently bounded product/design repositories | Approved; recorded below |
| 2026-08-04 | [Separate CMDC and Design with shared history plus cleanup commits](2026-08-04-cmdc-design-separation.md) | Approved and implemented |

## 2026-08-04 — Eight-repository operating model

The HQ-managed ecosystem will keep eight repositories rather than form a monorepo:
HQ, CMDC, Budget, Wonky Zipper, Ledger, Stat, Design, and Chat.

HQ is the coordination layer and contains no application code. Repository
identities will be normalized in deliberate phases that preserve existing
history and uncommitted work. Conversation memory is not canonical; committed
repository documentation is.

## 2026-08-04 — Canonical portfolio naming

HQ is the distinct portfolio umbrella. CMDC refers only to `craigmullin.com`.
The canonical project names are Budget, Chat, Ledger, Stat, Design, CMDC, and
Wonky Zipper. Earlier names such as SpikeChat, SpikeStat, Spanner & Hide, and
Mullin Design Language may appear only when documenting legacy history or
external identifiers that have not yet been migrated.
