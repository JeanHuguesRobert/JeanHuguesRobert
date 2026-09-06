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
