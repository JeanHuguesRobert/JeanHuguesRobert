---
shared_instructions: https://github.com/JeanHuguesRobert/cogentia/blob/main/instructions/AGENTS.shared.md
document_role: "operational"
document_kind: "agent-mandate"
visibility: "public"
lifecycle_state: "active"
classification_source: "cogentia.js"
classification_version: "1"
classification_rule: "agent-mandate"
classification_confidence: "strong"
---

# JeanHuguesRobert agent mandate

Read the shared Cogentia agent instructions referenced above before making changes. This local mandate activates the corpus-wide operational layer for this repository.

## Repository role for the first Cogentia Digital Twin

This public repository is the canonical public instance layer for the JHN Personal Digital Twin.

Keep the architectural separation explicit:

```text
Cogentia / Inseme
= generic Digital Twin machinery and COP semantics

JeanHuguesRobert/JeanHuguesRobert
= public definition of TwinRoot JHN and Agent JHN / John

JeanHuguesRobert/registre-mariani
= private/restricted overlay for the same Twin
```

This repository may define public identity, public constitutional constraints, public corpus references, public Agent John profiles and public specialization defaults. It must not redefine generic COP concepts merely to fit JHN; reusable abstractions belong in Cogentia/Inseme.

`TwinRoot JHN` and `Agent JHN / John` are not synonyms. The TwinRoot represents durable cognitive continuity associated with the represented subject; John is the first durable `LogicalAgent` operating within that Twin under explicit mandates.

## Public/private composition

The private registry is an additional governed source for the same Twin, not a second private Twin. Public agents and artifacts must never infer that permission to read private material implies permission to disclose it.

When private evidence affects a public conclusion, preserve provenance and disclosure boundaries. Prefer public reasoning that can be supported from public sources whenever the private basis cannot itself be disclosed.

## Specializations

John may have situated profiles such as coding, research, publication, correspondence or administration. A profile describes potential behavior and preferred capabilities; it does not grant authority.

Actual authority always comes from the current COP Mandate and its budget/resource limits. Create a distinct sub-`LogicalAgent` only when separate durable mandate continuity, budget, revocation or accountability is materially required.

Start with [`twin/README.md`](twin/README.md) for the public JHN Twin definition.
