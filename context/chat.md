# Chat context

Last reviewed: 2026-08-04

Chat owns SpikeChat. The local working tree is a mature React/Vite PWA with 39
commits, Firebase Hosting configuration, browser persistence, Vitest coverage,
PWA functionality, public legal/product pages, and a substantial handoff.

On 2026-08-04, `chat.git` was verified to contain the exact local `develop` and
`main` branch tips. The local `origin` now points to `chat.git`; the prior
`spikechat.git` remote is retained as `legacy-spikechat`. Three local files
remain modified:

- `src/App.css`
- `src/features/snapchat/SnapchatEditorPage.tsx`
- `src/pages/AboutPage.tsx`

Their exact dirty snapshot is protected by local ref
`backup/pre-normalization-work-2026-08-04`, and the working tree was not
altered. Lint, all 12 tests, and the production build passed on 2026-08-04.
Firebase ownership and Hosting site `spikechat-e682a` were verified, with
default URL `https://spikechat-e682a.web.app`. Browser PWA and deployed-content
verification remain required before considering the legacy repository archival.
