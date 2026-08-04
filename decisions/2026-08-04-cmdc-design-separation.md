# Separate CMDC application from Design without rewriting history

- Date: 2026-08-04
- Status: proposed
- Scope: CMDC and Design
- Decision owner: unknown

## Context

The Design `develop` branch contains 13 commits. The first six establish design
documentation, `3f07ac2` adds reusable design assets, and `7baf5b4` introduces
both the CMDC React/Vite/Firebase application and more design assets. Later
commits update the application, with one also updating a design component.
Because the histories are interleaved, a path-filtered split would discard
relevant provenance from at least one repository.

CMDC's canonical repository is empty. Design and its legacy remote both retain
the complete combined history. Firebase project `craigmullin` is the verified
production target for `www.craigmullin.com`.

## Decision

Copy the complete combined Design history into CMDC, then separate ownership
with ordinary cleanup commits in both repositories. Do not rewrite, squash, or
force-push existing commits.

- CMDC keeps the application runtime: `.firebaserc`, `.gitignore`,
  `eslint.config.js`, `firebase.json`, `index.html`, `package*.json`, `public/`,
  `src/`, TypeScript configuration, and `vite.config.ts`.
- Design keeps the language and source material: principles, colors,
  typography, tokens, component specifications, references, questions,
  explorations, changelog, and repository documentation.
- Each repository receives a new README and a cleanup commit describing its
  boundary. CMDC may keep copied design files temporarily until its build and
  deployed behavior are verified; removal is the final cleanup step.
- Preserve the pre-separation tips under explicit backup refs and retain the
  legacy Design remote.

## Rationale

This preserves every commit identifier and makes the mixed commits available
in both repositories. Cleanup remains reviewable and reversible. It also avoids
making a reusable runtime package decision before product needs justify one.

## Consequences

- Both repositories retain some historical files outside their eventual scope.
- `git log --follow` and commit references remain intact.
- The repositories become independently developable after cleanup.
- The combined history remains available from Design and its retained legacy
  remote even after CMDC is verified.

## Alternatives considered

- Path-filtered history: rejected because mixed commits would lose provenance.
- Start CMDC with a new root commit: rejected because it would sever application
  history.
- Keep the combined repository: rejected because it conflicts with the approved
  eight-repository operating model.
- Publish Design as a package now: deferred until a real multi-product runtime
  dependency exists.

## Follow-up

1. Create dated local backup refs for the current Design tip and imported CMDC
   tip.
2. Fetch the Design history into CMDC and create a non-destructive separation
   branch from `e59fde9`.
3. Add the CMDC boundary cleanup and README, then run lint and build.
4. Create a Design separation branch from `e59fde9`; remove only application
   runtime files, update its README, and verify retained assets.
5. Push both separation branches for review. Do not change production hosting.
6. Merge only after verifying CMDC output against the current production site.
