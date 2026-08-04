# Design context

Last reviewed: 2026-08-04

Design owns the Craig Mullin Design Language: principles, tokens, typography,
components, standards, and visual assets. The local working tree is developed
but points to `mullin-design-language.git`, while `design.git` is the intended
canonical repository and contains five design-language documents remotely.

The working tree also contains the CMDC React/Vite website and Firebase
configuration, so it currently has two responsibilities. Their later
separation must preserve history and avoid prematurely defining Design as a
runtime package. The delivery mechanism to products remains undecided.
