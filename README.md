# HQ

HQ is the portfolio control plane for Craig's product and site ecosystem. It records what
the projects are, where their canonical repositories live, how they relate, and
what portfolio-level work should happen next.

HQ contains no product application code. Product implementation and
project-specific decisions belong in their respective repositories.

## Start here

- [NOW.md](NOW.md) — the portfolio's current condition and next actions
- [PORTFOLIO.md](PORTFOLIO.md) — a human-readable project dashboard
- [projects.yaml](projects.yaml) — the machine-readable project registry
- [ROADMAP.md](ROADMAP.md) — approved normalization sequence
- [decisions/](decisions/) — settled portfolio-level decisions
- [context/](context/) — concise audit context for each project
- [templates/](templates/) — operating-document templates for later phases

## Source-of-truth hierarchy

1. The relevant repository and its committed documentation
2. Settled decision records
3. Current-state documents such as `NOW.md`
4. Conversation history and AI memory

When sources disagree, verify the repository state and update the durable
documentation. Do not silently resolve a project-level conflict in HQ.

## Repository boundaries

The ecosystem uses eight repositories: HQ plus seven product or design
repositories. HQ coordinates them but does not own their implementation.

CMDC refers only to the `craigmullin.com` site. HQ is distinct from CMDC and
sits above every product and site in the portfolio.

The initial registry reflects the read-only audit completed on 2026-08-04.
Fields marked `unknown` have not been verified and must not be guessed.
