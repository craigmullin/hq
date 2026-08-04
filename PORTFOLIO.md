# CMDC portfolio

Last reviewed: 2026-08-04

| Project | Responsibility | Intended local repository | Audited condition | Identity risk |
|---|---|---|---|---|
| HQ | Portfolio control plane | `C:\Users\cmullin\code\hq` | Baseline committed and pushed | None known |
| CMDC | `craigmullin.com` application | `C:\Users\cmullin\code\cmdc` | Empty repository | Website implementation currently lives in Design working tree |
| Budget | Future home-budgeting application | `C:\Users\cmullin\code\budget` | Empty repository | None known |
| Wonky Zipper | Independent retail brand and website | `C:\Users\cmullin\code\wonkyzipper` | Existing minimal HTML/CSS site; 19 commits at audit | Production status unknown |
| Ledger | Auto-maintenance tracking application | `C:\Users\cmullin\code\ledger` | Empty repository | None known |
| Stat | Volleyball statistics application | `C:\Users\cmullin\code\stat` | Empty repository | None known |
| Design | Craig Mullin Design Language | `C:\Users\cmullin\code\design` | Developed design system plus CMDC site | Canonical origin verified; CMDC separation remains |
| Chat | SpikeChat application | `C:\Users\cmullin\code\chat` | Mature React/Vite PWA; 39 commits at audit | Canonical origin verified; three modified files protected |

## Portfolio boundaries

- HQ coordinates the portfolio and owns no product code.
- Design provides principles, tokens, typography, components, and standards.
- CMDC owns the deployable `craigmullin.com` application once the approved
  history-preserving separation is complete.
- Wonky Zipper remains a distinct public brand while belonging to the internal
  portfolio.
- Chat, Budget, Ledger, and Stat remain independently bounded products.

## Dependency view

- CMDC is expected to consume guidance or assets from Design; the exact delivery
  mechanism is not yet decided.
- Other products may adopt Design guidance later, but no package or runtime
  dependency has been approved.
- No other cross-repository dependencies were verified during the audit.

Machine-readable details and explicit unknowns are maintained in
`projects.yaml`.
