# HQ operating instructions

## Purpose

This repository is the CMDC portfolio control plane. Keep it limited to
portfolio coordination, durable context, shared templates, and cross-project
decisions. Do not add product application code here.

## Before making changes

1. Read `NOW.md`, `PORTFOLIO.md`, and `projects.yaml`.
2. Read the relevant file under `context/`.
3. Read applicable records under `decisions/`.
4. Verify time-sensitive repository facts before presenting them as current.

## Boundaries

- Treat each product repository as authoritative for its implementation and
  project-specific decisions.
- Do not modify a product repository from an HQ task unless the user explicitly
  expands the task's scope.
- Do not silently override project-level decisions. Prepare a recommendation
  for the relevant project or record an approved portfolio decision.
- Preserve unknown values as `unknown` until verified.
- Never store credentials, secrets, private keys, or `.env` contents here.
- Keep HQ documents concise enough to serve as a practical reset point.

## Maintaining the registry

- Update `projects.yaml` first when a repository identity, local path, remote,
  domain, lifecycle state, or dependency changes.
- Keep `PORTFOLIO.md` and the matching `context/*.md` summary consistent with
  the registry.
- Put current work in `NOW.md`; put sequencing in `ROADMAP.md`; put settled,
  consequential choices in `decisions/`.
- Mark observations with a review date. Distinguish observed state from intended
  state and from proposals.

## Completion expectations

For substantive HQ work, verify internal links and registry syntax, review the
Git diff, and summarize which canonical artifacts changed. Do not claim product
state changed unless it was explicitly in scope and verified.
