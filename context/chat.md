# Chat context

Last reviewed: 2026-08-04

Chat is the canonical product name. The local working tree, historically named
SpikeChat, is a mature React/Vite PWA with 39
commits, Firebase Hosting configuration, browser persistence, Vitest coverage,
PWA functionality, public legal/product pages, and a substantial handoff.

On 2026-08-04, `chat.git` was verified to contain the exact local `develop` and
`main` branch tips. The local `origin` now points to `chat.git`; the prior
`spikechat.git` remote is retained as `legacy-spikechat`. Three local files were
modified at audit:

- `src/App.css`
- `src/features/snapchat/SnapchatEditorPage.tsx`
- `src/pages/AboutPage.tsx`

Their exact dirty snapshot remains protected by local ref
`backup/pre-normalization-work-2026-08-04`. The changes were reviewed as one
coherent experimental-tools update. Cross-input and keyboard caption-position
support was restored before commit `0646b97` was published to `develop`.

Project-local `AGENTS.md`, `NOW.md`, canonical repository/hosting details, and
the corrected public GitHub link were committed in baseline `98da936`. Lint,
all 12 tests, the production build, PWA generation, rendered About-to-Snapchat
flow, and console passed on 2026-08-04.
Firebase ownership and Hosting site `spikechat-e682a` were verified, with
default URL `https://spikechat-e682a.web.app`. Browser PWA and deployed-content
verification remain required before considering the legacy repository archival.
