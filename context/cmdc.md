# CMDC context

Last reviewed: 2026-08-04

CMDC owns the `craigmullin.com` application. Its intended repository is empty.
The current React/Vite website implementation, package identity, and Firebase
configuration were found inside the Design working tree. A later phase must
separate these roles while preserving history. The combined source passed lint
and a production build on 2026-08-04. The `www.craigmullin.com` DNS CNAME points
to `craigmullin.web.app`, and their deployed content matched exactly on
2026-08-04. Firebase project/site `craigmullin` is therefore the verified
current production target. The user deleted project `craigmullin-com`, and its
absence from the accessible Firebase project list was verified on 2026-08-04.

A proposed history-preserving separation plan is recorded in
`decisions/2026-08-04-cmdc-design-separation.md`. Unknown: apex-domain behavior
and the application roadmap.
