---
title: Appearance log
author: Jean Hugues Noël Robert, baron Mariani
affiliation: Institut Mariani / C.O.R.S.I.C.A., 1 cours Paoli, F-20250 Corte, Corsica
date: '2026-09-15'
last_modified_at: '2026-09-15'
version: '0.1'
status: published
license: CC BY-SA 4.0
language: en
document_role: operational
update_policy: UP-DEFAULT-REVIEWED
provenance:
  origin_type: repository
  origin_repository: unknown
  origin_ref: unknown
  origin_date: '2026-09-15'
  derived_from: []
review:
  status: unreviewed
  reviewed_by: []
---

# Appearance log

This directory retains public, observed appearances attributable to the JHN
TwinRoot. It is a source-fact log, not a persona registry or a publication
campaign model.

```text
appearance-log/<platform>/<year>/<month>/segment-####.jsonl
```

Each line is an immutable `ubikia.observed-appearance.v0.1` record. It keeps
the displayed text, available locator, visibility, observed time and minimal
parent context. Interpretations such as persona, role, theme, mandate and
source derivation are intentionally excluded: they remain revisable
projections with their own provenance.

The Ubikia adapter is experimental and intentionally does not claim COP
TraceDescriptor conformance while Inseme #61/#63 are being stabilized.
