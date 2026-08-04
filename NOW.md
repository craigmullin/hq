# Current state

Last reviewed: 2026-08-04
Owner: unknown

## Objective

Establish HQ as the trustworthy, lightweight command center for the eight-repo
CMDC ecosystem before any product repository is normalized.

## Current focus

Phase 3: continue verified, history-preserving repository identity
reconciliation.

## Next three actions

1. Prepare the history-preserving Design/CMDC source separation now that the
   production target is verified.
2. Baseline Chat after reviewing its protected uncommitted work.
3. Clarify Wonky Zipper's production status without changing its deployment.

## Blockers

- Production URLs and hosting details are not verified for most projects.

## Recently completed

- Completed a read-only audit of all eight intended repositories.
- Approved the eight-repository operating model and four-phase normalization
  sequence.
- Pointed the active HQ task at `C:\Users\cmullin\code\hq`.
- Scaffolded the HQ control-plane documents without modifying product repos.
- Committed and pushed the HQ baseline to `hq.git`.
- Verified `chat.git` and `design.git` contain the exact developed branch tips.
- Protected Chat's three-file dirty state in
  `backup/pre-normalization-work-2026-08-04` without changing the worktree.
- Made `chat.git` and `design.git` the local `origin` remotes while retaining
  the legacy repositories as named remotes.
- Passed Chat lint, 12 tests, and production build; passed the combined
  Design/CMDC lint and production build.
- Verified Firebase ownership and Hosting sites for `spikechat-e682a`,
  `craigmullin`, and `craigmullin-com` without changing them.
- Verified all eight saved Codex projects point to their canonical
  `C:\Users\cmullin\code\<project>` repositories; no old directory was deleted.
- Verified `www.craigmullin.com` points to `craigmullin.web.app` and serves the
  same deployed content; `craigmullin-com` remains untouched and unclassified.

## Open questions

- Who should be recorded as portfolio owner?
- Which production URLs and hosting projects are canonical?
- Is the current Wonky Zipper site production, a placeholder, or historical?
- What are the desired initial outcomes and priorities for Budget, Ledger, and
  Stat?
