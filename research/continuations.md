---
title: "Continuation Triage"
description: "Operational triage of active Cogentia continuations for the Living Corpus."
layout: default
nav_order: 3
document_role: operational
status: "living dashboard"
license: CC BY 4.0
affiliation: Institut Mariani — émanation R&D de C.O.R.S.I.C.A., 1 cours Paoli, F-20250 Corte, Corsica
date: 2026-06-09
creator: Jean Hugues Noël Robert, baron Mariani
canonical_url: https://github.com/JeanHuguesRobert/JeanHuguesRobert/blob/main/research/continuations.md
last_reviewed_at: 2026-06-16
document_kind: "dashboard"
visibility: "public"
lifecycle_state: "active"
classification_source: "cogentia.js"
classification_version: "1"
classification_rule: "dashboard"
classification_confidence: "medium"
---

# Continuation Triage

This document records the public, human-readable triage of active Cogentia continuations. The operational source of truth remains the local continuation store:

```text
C:\tweesic\JeanHuguesRobert\.cogentia\continuations
```

The current active queue is read with:

```text
node scripts/cogentia.js continuation list --status active --json
```

## Triage Rule

Priority is used as an execution hint, not as a truth claim.

Higher priority means:

- more useful for making the corpus digestible;
- more public-facing;
- more likely to unblock later consolidation;
- less dependent on unstable local code.

Lower priority means:

- exploratory;
- not blocking the current stabilization;
- dependent on a dirty or intentionally deferred repository.

## Active Queue

| Priority | Continuation | Kind | Bucket | Reason |
|---:|---|---|---|---|
| 90 | `ctn_9b562108` | `profile_readme` | public-entrypoint | The profile README is the first public entry point and should reflect the new corpus map. |
| 85 | `ctn_22f5c033` | `derived_trails` | navigation | Curated reading trails make the corpus digestible and should follow the global map/orientation pass. |
| 80 | `ctn_092374da` | `issues_open` | tooling-debt | Cogentia issues concern the continuation mechanism itself; resolving them improves future triage. |
| 70 | `ctn_d65a4ed2` | `derived_tutorials` | derived-products | Tutorials should be refreshed after source/orientation stabilization, but after the public entry point and trails. |
| 60 | `ctn_16d0fda6` | `derived_websites` | derived-products | Website refresh has broad public surface area; run after map, trails and tutorial sources are stable. |
| 55 | `ctn_ebcd475e` | `issues_open` | research-issues | Barons Mariani issues are relevant to Autonomia and housing research, but less blocking than navigation. |
| 45 | `ctn_76d2e69f` | `issues_open` | review | MareNostrum pre-submission review remains useful, but is not blocking current corpus digestion. |
| 35 | `ctn_6d6bf741` | `issues_open` | idea-to-explore | The FractaVolta circular command-center issue is exploratory; keep visible but low priority. |
| 10 | `ctn_426a7406` | `issues_open` | deferred-dirty-repo | Inseme non-research work is intentionally deferred while the local repository remains unstable. |

## Resolved During Triage

| Continuation | Decision | Reason |
|---|---|---|
| `ctn_256919ef` | `request_specifics` | The objection "This proposal seems unrealistic" is not falsifiable without a measurable claim, affected predicate or evidence threshold. |
| `ctn_d41afe9b` | `addressed` | The proposed Inox Rossignol work is already present in pushed history as commit `6658cdc`; later commits supersede the stale file hashes. |

## GitHub Issue Snapshot

Checked on 2026-06-16 with `gh issue list --state open`. The continuation
objects still carry older issue counts in their titles/questions; process the
live GitHub list before resolving any `issues_open` continuation.

| Repository | Open issues | Continuation | Reconciliation note |
|---|---:|---|---|
| `JeanHuguesRobert/cogentia` | 20 | `ctn_092374da` | Priority remains high; issue #19 ("Integrate `ubikia` as an official corpus repository") is now partly addressed by the corpus-navigation pass but is still open on GitHub. |
| `JeanHuguesRobert/barons-Mariani` | 7 | `ctn_ebcd475e` | The issue continuation title says 3; live backlog is broader and includes recent research issues #7 and #8. |
| `JeanHuguesRobert/marenostrum` | 1 | `ctn_76d2e69f` | Count still matches; issue #1 remains the pre-submission review RFC. |
| `JeanHuguesRobert/FractaVolta` | 3 | `ctn_6d6bf741` | The continuation title says 1; issue #6 tracks site follow-up after the EN-first / FR-operational restructure and should be considered with the website continuation. |
| `JeanHuguesRobert/inseme` | 7 | `ctn_426a7406` | The continuation title says 3; keep deferred until the local repository is intentionally stabilized. |

## Next Execution Order

1. Refresh the profile README as a faithful derived product from the now-stabilized corpus map.
2. Refresh curated reading trails so humans and agents have reliable entry paths.
3. Process Cogentia's own GitHub issue continuations, because they concern the continuation mechanism itself.
4. Refresh tutorials, then websites, once navigation remains stable.
5. Keep Barons Mariani and MareNostrum issue continuations active as research/review backlog.
6. Keep FractaVolta's exploratory hardware/interface idea low priority.
7. Do not process Inseme non-research continuations until the local repository is intentionally stabilized.

## Maintenance

When a continuation is processed, update both:

1. the continuation JSON through `cogentia.js continuation resolve` or `cancel`;
2. this dashboard if the public order changes.

Do not use this document to replace the continuation store. It is a digestible view, not the operational queue.
