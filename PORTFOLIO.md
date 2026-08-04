# CMDC portfolio

Last reviewed: 2026-08-04

| Project | Responsibility | Intended local repository | Audited condition | Identity risk |
|---|---|---|---|---|
| HQ | Portfolio control plane | `C:\Users\cmullin\code\hq` | Baseline committed and pushed | None known |
| CMDC | `craigmullin.com` application | `C:\Users\cmullin\code\cmdc` | Developed React/Vite site; canonical naming baseline prepared | Design-system refactor pending |
| Budget | Future home-budgeting application | `C:\Users\cmullin\code\budget` | Documentation baseline prepared; implementation intentionally absent | Product outcome unknown |
| Wonky Zipper | Independent retail brand and website | `C:\Users\cmullin\code\wonkyzipper` | Existing minimal HTML/CSS site; 19 commits at audit | Production status unknown |
| Ledger | Auto-maintenance tracking application | `C:\Users\cmullin\code\ledger` | Documentation baseline prepared; implementation intentionally absent | Initial scope unknown |
| Stat | Volleyball statistics application | `C:\Users\cmullin\code\stat` | Public synthetic-data demo and private Google-authenticated owner workspace deployed | `spikestat.craigmullin.com` TLS provisioning pending |
| Design | Shared design system and product guidance | `C:\Users\cmullin\code\design` | Updated v1 guidance; Playfair Display and Inter approved | Product accent hex values unresolved |
| Chat | Chat application | `C:\Users\cmullin\code\chat` | Canonical naming applied; lint, tests, build, and PWA generation pass | Deployed PWA verification remains before legacy archival |

## Portfolio boundaries

- HQ coordinates the portfolio and owns no product code.
- Design provides principles, tokens, typography, components, and standards.
- CMDC owns the deployable `craigmullin.com` application.
- Wonky Zipper remains a distinct public brand while belonging to the internal
  portfolio.
- Chat, Budget, Ledger, and Stat remain independently bounded products.
- CMDC means only `craigmullin.com`; HQ is the portfolio umbrella and is not
  named CMDC HQ.

## Dependency view

- CMDC is expected to consume guidance or assets from Design; the exact delivery
  mechanism is not yet decided.
- Other products may adopt Design guidance later, but no package or runtime
  dependency has been approved.
- No other cross-repository dependencies were verified during the audit.

Machine-readable details and explicit unknowns are maintained in
`projects.yaml`.
