# Ecosystem roadmap

Last reviewed: 2026-08-04

This roadmap records the approved normalization sequence. Phase boundaries are
safety boundaries: later work must not be folded into an earlier phase without
explicit approval.

## Phase 1 — Establish HQ safely

Status: complete

- Use `C:\Users\cmullin\code\hq` as the HQ repository.
- Scaffold the operating documents and project registry.
- Record observed repository facts and explicit unknowns.
- Commit the first HQ baseline.
- Do not modify product repositories.

## Phase 2 — Correct saved Codex project paths

Status: complete

- Point each saved project to its matching directory under
  `C:\Users\cmullin\code`.
- Verify that no saved project remains attached to an empty `Documents`
  repository or nonexistent path.
- Do not delete old directories until task history and overlooked files have
  been checked.

## Phase 3 — Reconcile repository identities

Status: in progress

- Chat's uncommitted work is protected and its full SpikeChat history is
  verified in `chat.git`; retain `spikechat.git` until application and deploy
  verification is complete.
- Design and CMDC now preserve the shared history in their intended canonical
  homes and use ordinary cleanup commits to enforce their boundaries.
- Preserve Wonky Zipper history and clarify its production status.

## Phase 4 — Baseline each project

Status: pending

- Add project-local operating documents without redesigning products.
- Record maturity, setup, deployment, environment expectations, and production
  URLs.
- Run available validation and add lightweight automation where useful.
- Pin supported runtimes and replace fragile dependency declarations when
  justified by project-specific review.
