# Current state

Last reviewed: 2026-08-04
Owner: unknown

## Objective

Maintain HQ as the trustworthy, lightweight command center for the eight-repo
portfolio while product repositories are normalized and modernized.

## Current focus

Apply the normalized portfolio identity and shared design guidance across
product refactors while preserving each product's data and history.

## Next three actions

1. Connect the intended `stat.craigmullin.com` custom domain after DNS is ready.
2. Plan the next product redesign against the approved Design guidance.
3. Verify remaining production URLs and hosting projects.

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
  same deployed content.
- Verified the user-deleted `craigmullin-com` project is absent from the
  accessible Firebase project list.
- Mapped the interleaved Design/CMDC history and proposed a no-rewrite,
  shared-history separation plan.
- Implemented the approved Design/CMDC separation with full ancestry preserved,
  dated backup refs, and ordinary cleanup commits.
- Published CMDC `main` at `c7f7706` and Design `develop` at `5ba934b`; retained
  both remote review branches and changed no production deployment.
- Reviewed and committed Chat's protected experimental-tools work at `0646b97`,
  restoring pointer and keyboard caption-position support.
- Established Chat's project-local operating baseline at `98da936`; lint, 12
  tests, build, PWA generation, browser flow, console, and Hosting URL passed.
- Established canonical naming: HQ is distinct, and CMDC refers only to
  `craigmullin.com`.
- Incorporated Heidi's shared design guidance and M.* product-family rules.
- Prepared project-local canonical-state baselines for every repository.
- Imported all locally known Stat history and Bitbucket branch tips without
  changing the legacy working directory.
- Replaced Stat's broken Vue 2 client with a legacy-compatible React,
  TypeScript, and Vite runtime; lint, build, signed-out browser flow, Firebase
  ownership, Firestore database, Hosting, and dependency audit passed.
- Published Stat modernization commit `52337f9` and all 15 legacy branch tips
  to `stat.git`.
- Promoted Stat release `7c56a18` to `main` and deployed it to Firebase
  Hosting with a one-time legacy service-worker cleanup.
- Deployed Stat password recovery release `f9b0590` for legacy users who no
  longer know their Firebase password.
- Replaced Stat's transitional password flow with Google sign-in in release
  `1c2a08b`; enabled the Firebase provider and deployed owner-only Firestore
  rules for verified account `cmlmullin@gmail.com`.
- Approved Playfair Display and Inter as the shared primary typography and
  published Design commit `86d1f64`.
- Published and deployed Stat release `07193be` with a public synthetic-data
  demo and a separate private Google-authenticated owner workspace.

## Open questions

- Who should be recorded as portfolio owner?
- Which production URLs and hosting projects are canonical?
- Is the current Wonky Zipper site production, a placeholder, or historical?
- What is Budget's desired initial outcome and priority?
- Which existing or temporary Firebase account should be used for Stat's
  authenticated Firestore flow validation?
