# Development workflow and product sequence

Date: 2026-08-04

Status: approved

## Decision

Use `main` as the protected, production-ready branch and `develop` as the
shared integration/staging branch in each portfolio repository. Do feature and
fix work on short-lived branches, merge those into `develop`, and promote a
tested release from `develop` to `main`. Production deploys come only from
`main`; preview or staging deploys may come from pull requests or `develop`.

This is a pragmatic hybrid for the current portfolio. Trunk-based development
with short-lived branches into `main` is the more common modern default, but a
separate integration branch fits the explicit need to accumulate substantial
redesign work without changing production.

The approved product sequence is:

1. Refactor CMDC (`craigmullin.com`) to the updated design language.
2. Refactor SpikeChat to the updated design language.
3. Rebuild Ledger from scratch to the updated design system.
4. Rewrite SpikeStat in the canonical `spikestat` repository, preserve and
   study the legacy app/backend, then add the product to `craigmullin.com`.
5. Refactor Design to the updated design language.
6. Create Wonky Zipper as a standalone flagship project.

Budget remains empty and outside this sequence.

## Safety constraints

- Preserve repository history and uncommitted work.
- Do not delete legacy repositories, placeholder history, or Firebase projects
  until their replacements and migrations are verified.
- Treat `spikestat-pwa-epsilon` as a read-only legacy source until its Firestore
  contract and uncommitted work are protected.
- Do not begin visual refactoring until the updated design-language guidance is
  available.
