# Chat context

Last reviewed: 2026-08-04

Chat owns SpikeChat. The local working tree is a mature React/Vite PWA with 39
commits, Firebase Hosting configuration, browser persistence, Vitest coverage,
PWA functionality, public legal/product pages, and a substantial handoff.

The working tree points to `spikechat.git`, while `chat.git` is the intended
canonical repository and currently has only an initial README and `.gitignore`
remotely. Three local files were modified at audit time:

- `src/App.css`
- `src/features/snapchat/SnapchatEditorPage.tsx`
- `src/pages/AboutPage.tsx`

Protect those changes before any history or remote normalization. Verify lint,
tests, build, PWA behavior, and Firebase configuration before considering the
legacy repository archival.
