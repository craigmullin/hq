# CMDC context

Last reviewed: 2026-08-04

CMDC owns the `craigmullin.com` React/Vite application. On 2026-08-04, the
complete 13-commit combined history was imported from Design and preserved in
CMDC. Ordinary cleanup commit `c7f7706` removed Design-owned source material
without rewriting history. CMDC `main` now contains the application runtime,
Firebase configuration, and a repository-specific README.

After separation, lint and the production build passed. The generated CSS and
JavaScript asset identities matched the deployed production page. The
`www.craigmullin.com` DNS CNAME points
to `craigmullin.web.app`, and their deployed content matched exactly on
2026-08-04. Firebase project/site `craigmullin` is therefore the verified
current production target. The user deleted project `craigmullin-com`, and its
absence from the accessible Firebase project list was verified on 2026-08-04.

The pre-cleanup imported tip is retained at
`backup/imported-design-history-2026-08-04`. Unknown: apex-domain behavior and
the application roadmap.
