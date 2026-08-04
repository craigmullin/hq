# Design context

Last reviewed: 2026-08-04

Design is the canonical product name and owns the shared design system:
principles, tokens, typography, components, standards, and visual assets. On 2026-08-04, `design.git` was
verified to contain the exact local `develop` and `main` branch tips. The local
`origin` now points to `design.git`; the prior `mullin-design-language.git`
remote is retained as `legacy-mullin-design-language`.

On 2026-08-04, ordinary cleanup commit `5ba934b` removed the CMDC application
runtime from Design `develop` without rewriting the shared history. The branch
retains all principles, tokens, typography, component specifications,
references, questions, and explorations. The combined pre-separation tip is
retained at `backup/pre-separation-2026-08-04`, and the legacy remote remains.

Design is guidance and source material rather than a runtime package. Its
delivery mechanism to products remains undecided.
