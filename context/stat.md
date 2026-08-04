# Stat context

Last reviewed: 2026-08-04

Stat is the volleyball statistics tracking application and M.S product. The
legacy Vue 2 application's complete selected ancestry and all 15 locally known
Bitbucket branch tips are preserved in `stat.git`; the latter use `legacy/*`
branch names. The prior untracked `Delete.vue` is archived outside the runtime.

Canonical modernization commit `52337f9` replaces the broken client with a React,
TypeScript, Vite, and Firebase implementation that preserves the `matches` and
embedded `games` Firestore contract. Firebase project/site
`spikestat-pwa-epsilon`, its default Firestore database, and Hosting URL were
verified. Lint, build, signed-out browser flow, and the production dependency
audit pass. Authenticated Firestore reads and writes remain to be tested before
deployment. Production release `7c56a18` is live with a one-time cleanup worker
for the retired Vue PWA cache. Previously installed clients may show the old
shell until their browser performs its next service-worker update check.
