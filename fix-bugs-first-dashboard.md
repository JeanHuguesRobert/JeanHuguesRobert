---
title: "Fix Bugs First Work Dashboard"
author: unknown
affiliation: Institut Mariani / C.O.R.S.I.C.A., 1 cours Paoli, F-20250 Corte, Corsica
date: '2026-10-05'
license: CC BY-SA 4.0
language: en
document_role: operational
document_kind: dashboard
visibility: public
lifecycle_state: active
canonical_url: https://github.com/JeanHuguesRobert/JeanHuguesRobert/blob/main/fix-bugs-first-dashboard.md
status: working-paper
update_policy: UP-DEFAULT-REVIEWED
generated_by: scripts/generate-fix-bugs-first-dashboard.js
schema: "cogentia.fix-bugs-first-dashboard.v1"
generated_at: "2026-10-05T08:21:59.898Z"
doctrine: "Fix Bugs First (Operium / Cogentia)"
total_items: 389
open_bugs: 1
provenance:
  origin_type: generated
  origin_repository: JeanHuguesRobert/cogentia
  origin_ref: unknown
  origin_date: '2026-10-05'
  derived_from:
    - https://github.com/JeanHuguesRobert/operium/blob/fd1e111fec0d9dbfa78aee6c4d63d5e03b3a3801/backlog/items.yaml
    - https://github.com/JeanHuguesRobert/JeanHuguesRobert/blob/main/current-issues-list.md
review:
  status: unreviewed
  reviewed_by: []
---

# 🛡️ Fix Bugs First Work Dashboard

> *Generated at 2026-10-05T08:21:59.898Z from native system of records (Operium Backlog & GitHub Issues).*

## 🚦 Subsystem Gates Overview

| Subsystem | Gate Status | Open Bugs | Blocking Bugs | Features Gated |
|---|---|---|---|---|
| `agent-gateway` | ✅ **OK** | 0 | None | None |
| `cli` | ✅ **OK** | 0 | None | None |
| `cogentia-context` | ✅ **OK** | 0 | None | None |
| `docs` | ✅ **OK** | 0 | None | OP-FEAT-007 |
| `general` | ✅ **OK** | 1 | None | None |
| `magistral-routing` | ✅ **OK** | 0 | None | None |
| `mesh` | ✅ **OK** | 0 | None | OP-FEAT-002, OP-FEAT-004 |
| `meta` | ✅ **OK** | 0 | None | None |
| `ona` | ✅ **OK** | 0 | None | OP-FEAT-005, OP-FEAT-009 |
| `replication` | ✅ **OK** | 0 | None | OP-FEAT-006 |
| `secrets` | ✅ **OK** | 0 | None | None |
| `tooling` | ✅ **OK** | 0 | None | None |

## 🐛 Open Bugs (Fix First)

### [cogentia#78] Frontmatter: fix one malformation, reconcile two conflicting "required" definitions, add four missing invariants, expose one CI-able command [#78](https://github.com/JeanHuguesRobert/cogentia/issues/78)
- **Subsystem:** `general` | **Severity:** `normal` | **Urgency:** `planned` | **Status:** `open`

## 🚀 Gated Features & Planned Work

### [OP-FEAT-002] FractaNet observed-state reconciliation [#9](https://github.com/JeanHuguesRobert/operium/issues/9)
- **Subsystem:** `mesh` | **Gate:** 🟢 READY | **Status:** `open`
- **Next Action:** FBF bugs clear; design/implement observed-state reconciliation (issue #9)

### [OP-FEAT-004] poco-jhr Termux:Boot + MIUI autostart fallback [#6](https://github.com/JeanHuguesRobert/operium/issues/6)
- **Subsystem:** `mesh` | **Gate:** 🟢 READY | **Status:** `open`
- **Next Action:** Continue as mesh reliability feature after labeling

### [OP-FEAT-005] Ephemeral job runner for large CPU/RAM work [#3](https://github.com/JeanHuguesRobert/operium/issues/3)
- **Subsystem:** `ona` | **Gate:** 🟢 READY | **Status:** `open`
- **Next Action:** FBF bugs clear; design ephemeral job runner (issue #3) when ONA capacity allows

### [OP-FEAT-006] Content-addressed storage doctrine (buckets / Plakar) [#2](https://github.com/JeanHuguesRobert/operium/issues/2)
- **Subsystem:** `replication` | **Gate:** 🟢 READY | **Status:** `open`
- **Next Action:** Keep as doctrine/feature; no gate conflict unless replication bugs

### [OP-FEAT-007] Vendor-neutral API usage and billing monitoring [#1](https://github.com/JeanHuguesRobert/operium/issues/1)
- **Subsystem:** `docs` | **Gate:** 🟢 READY | **Status:** `open`
- **Next Action:** Low priority observability feature

### [OP-FEAT-009] Trusted-node La Nasa projection with observer-relative views [#26](https://github.com/JeanHuguesRobert/operium/issues/26)
- **Subsystem:** `ona` | **Gate:** 🟢 READY | **Status:** `open`
- **Next Action:** Complete the observer/view contract, then validate an unattended trusted Pi display with local La Nasa fallback (issue #26).

## 📜 Completed Items

- [x] **[OP-BUG-001]** Agent CLI Gateway Tailscale reachability intermittent from fracta (`agent-gateway` - bug)
- [x] **[OP-BUG-002]** System bearer rotation leaves runtime copies out of sync (`secrets` - bug)
- [x] **[OP-BUG-003]** Open Operium GitHub issues lack kind/subsystem labels (`meta` - bug)
- [x] **[OP-BUG-004]** Workstation admin-scoped npm tooling breaks user-space installs (`tooling` - bug)
- [x] **[OP-BUG-005]** Secrets research notes drift from operational secrets-management.md (`docs` - bug)
- [x] **[OP-BUG-006]** Termux shell profile trusts an inherited sentinel with an incomplete environment (`tooling` - bug)
- [x] **[OP-BUG-007]** Gateway semantic search called AI-router embeddings inline (IoC violation) (`cogentia-context` - bug)
- [x] **[OP-BUG-008]** Pi hosted La Nasa viewer survives a tunnel restart without a live VNC session (`mesh` - bug)
- [x] **[OP-BUG-009]** Public Cogentia Guide and aggregator reachability is broken (`magistral-routing` - bug)
- [x] **[OP-FEAT-001]** Automate Magistral coding-agent map apply + verify on fracta (`magistral-routing` - feature)
- [x] **[OP-FEAT-003]** Cross-device WIP handoff/resume polish (`cli` - feature)
- [x] **[OP-FEAT-008]** Bounded Termux tmux handoff helper (`cli` - feature)
- [x] **[OP-FEAT-011]** Accept calendar wakes by packet_ref (by reference) (`ona` - feature)
