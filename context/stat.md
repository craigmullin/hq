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
audit pass. Production release `7c56a18` is live with a one-time cleanup worker
for the retired Vue PWA cache. Previously installed clients may show the old
shell until their browser performs its next service-worker update check.
Release `f9b0590` adds verified Firebase password recovery to the deployed login
screen.

Release `1c2a08b` replaces the transitional password UI with Google sign-in.
Firebase provider settings use public name Stat and support email
`cmlmullin@gmail.com`. Deployed Firestore rules allow reads and writes only for
that verified Google identity.

Release `07193be` adds a public, no-login portfolio demo backed entirely by
synthetic in-memory data. Match creation, game tracking, saving, and viewing
passed browser validation. The private owner workspace and its Firestore data
remain behind Google sign-in and owner-only rules. The release also adopts the
approved Playfair Display and Inter typography and is deployed to Firebase
Hosting. `spikestat.craigmullin.com` is the approved public domain. Its CNAME
target was verified on 2026-08-04; Firebase HTTPS certificate provisioning was
still pending at that review.
