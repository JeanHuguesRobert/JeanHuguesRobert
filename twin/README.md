---
title: "JHN Personal Digital Twin — public instance definition"
document_role: source
document_kind: instance-definition
visibility: public
lifecycle_state: working
language: en
update_policy: UP-DEFAULT-REVIEWED
---

# JHN Personal Digital Twin — public instance definition

This directory is the public, instance-specific definition of the first Cogentia Personal Digital Twin associated with JHN.

It deliberately does **not** define the generic Digital Twin architecture. Generic concepts and runtime semantics belong to Cogentia/Inseme and COP.

## Layering

```text
Cogentia / Inseme
= generic Digital Twin, COP, capability, mandate, budget, act, trace and imputation machinery

this repository
= public JHN Twin instance definition

JeanHuguesRobert/registre-mariani
= private/restricted overlay for the same Twin

COP Mandate
= situated authority: what may be done now, for whom, for which purpose and within which budget
```

The public and private layers compose with provenance. The private layer does not create another Twin identity and must not silently leak into public output.

## Identity model

Working identifiers:

```text
represented subject  -> subject:jhn
TwinRoot             -> twin:jhn
LogicalAgent         -> agent:jhn:john
public name          -> Agent JHN / John
```

The represented living subject, the TwinRoot and Agent John are distinct.

- The represented subject is the human source of personal authority.
- `TwinRoot JHN` is the durable declared cognitive continuity of the personal Twin.
- `Agent JHN / John` is the first durable `LogicalAgent` of that Twin.
- Concrete model processes, coding agents, scripts and humans that execute work are `HandlerInstance`s unless a separate durable LogicalAgent identity is explicitly warranted.

## Operational invariant

John must not be defined primarily by one model, provider, prompt, process or machine.

The intended execution chain is:

```text
Principal
→ Mandate
→ LogicalAgent John
→ Capability selection
→ HandlerInstance
→ CapabilityInvocation
→ Act
→ Trace
→ Imputation
```

For consequential acts, the applicable budget/resource limits and trace regime are part of the authorization and accountability context.

## Public instance content

This public layer may progressively define or reference:

- public identity and continuity declarations;
- public constitutional constraints;
- public corpus and provenance map;
- public Cogentigram or other descriptive models;
- public defaults for Agent John;
- public specialization profiles;
- public capability preferences;
- public rules governing communication, publication and derived products;
- references to generic Cogentia/Inseme specifications.

It should not duplicate generic protocol definitions.

For a comprehensive presentation of Agent John's capabilities in French, see [AGENT_JOHN_FR.md](AGENT_JOHN_FR.md).
For sovereign learnings, safety laws, and circuit breaker specifications, see [AGENT_JOHN_LEARNINGS_FR.md](AGENT_JOHN_LEARNINGS_FR.md).

## Private overlay

`JeanHuguesRobert/registre-mariani` may supply restricted facts, evidence, memory, constraints and specialization overlays when a mandate authorizes access.

The key distinction is:

```text
may_read(private_information)
!=
may_disclose(private_information)
```

A private fact may affect an internal assessment while remaining undisclosable. Provenance, visibility and the disclosable basis of a public conclusion must remain distinguishable.

## Specializations

John may operate through situated profiles, initially expected to include domains such as:

```text
john/general
john/coding
john/research
john/publication
john/correspondence
john/administration
```

These names are provisional. A profile is a specialization of behavior, context and preferred capabilities. It is **not** an authorization grant.

The composition rule is:

```text
generic Cogentia rules
+ public JHN definition
+ permitted private overlay
+ selected specialization
+ current Mandate
+ current Budget
= situated operational context for John
```

A distinct child `LogicalAgent` should be introduced only when separate durable mandate continuity, budget, suspension/revocation or accountability is required. Otherwise prefer John plus a specialization profile and an explicit mission mandate.

## Current implementation target

The current executable vertical slice lives in `JeanHuguesRobert/inseme`, tracked primarily by:

- Inseme Issue #17 — first native JHN personal Digital Twin vertical slice;
- Inseme Issue #31 — COP handler/mandate/execution identity, currently converging on `CapabilityInvocation -> Act -> Trace -> Imputation`;
- `apps/platform/mcp/cop/` — current local JHN COP runtime.

The minimum credible operational milestone is not merely a conversational John. John must be able to cause at least one useful, bounded consequential act and later reconstruct:

```text
what happened
who materially executed it
which LogicalAgent caused it
for which Principal
under which Mandate and version
using which Capability
within which Budget/resource bounds
with which evidence and effect
how the Act is imputed and reported
```

## Next public-instance work

Keep this directory intentionally small while the generic schemas are still stabilizing. Near-term additions should be driven by the executable JHN vertical slice rather than speculative completeness.

Likely next artifacts are:

- a minimal machine-readable Twin manifest once the generic schema is stable enough;
- a public Agent John manifest;
- a small set of specialization profiles proven useful by real missions;
- explicit links to public constitutional and corpus sources instead of duplicated summaries.
