# Design context

Last reviewed: 2026-08-04

Design owns the Craig Mullin Design Language: principles, tokens, typography,
components, standards, and visual assets. On 2026-08-04, `design.git` was
verified to contain the exact local `develop` and `main` branch tips. The local
`origin` now points to `design.git`; the prior `mullin-design-language.git`
remote is retained as `legacy-mullin-design-language`.

The working tree also contains the CMDC React/Vite website and Firebase
configuration, so it currently has two responsibilities. Their later
separation must preserve history and avoid prematurely defining Design as a
runtime package. Lint and the production build passed on 2026-08-04. Firebase
project and Hosting site `craigmullin` were verified, with default URL
`https://craigmullin.web.app`. The `www.craigmullin.com` DNS CNAME and deployed
content confirm this is the current production target. A second project/site,
`craigmullin-com`, serves different content and remains unclassified. The
delivery mechanism to products remains undecided.
