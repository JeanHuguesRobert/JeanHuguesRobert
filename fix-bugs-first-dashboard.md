---
title: "Fix Bugs First Work Dashboard"
schema: "cogentia.fix-bugs-first-dashboard.v1"
generated_at: "2026-08-09T14:30:32.738Z"
doctrine: "Fix Bugs First (Operium / Cogentia)"
total_items: 14
open_bugs: 0
---

# 🛡️ Fix Bugs First Work Dashboard

> *Generated at 2026-08-09T14:30:32.738Z from native system of records (Operium Backlog & GitHub Issues).*

## 🚦 Subsystem Gates Overview

| Subsystem | Gate Status | Open Bugs | Blocking Bugs | Features Gated |
|---|---|---|---|---|
| `agent-gateway` | ✅ **OK** | 0 | None | None |
| `cli` | ✅ **OK** | 0 | None | None |
| `docs` | ✅ **OK** | 0 | None | OP-FEAT-007 |
| `magistral-routing` | ✅ **OK** | 0 | None | None |
| `mesh` | ✅ **OK** | 0 | None | OP-FEAT-002, OP-FEAT-004 |
| `meta` | ✅ **OK** | 0 | None | None |
| `ona` | ✅ **OK** | 0 | None | OP-FEAT-005 |
| `replication` | ✅ **OK** | 0 | None | OP-FEAT-006 |
| `secrets` | ✅ **OK** | 0 | None | None |
| `tooling` | ✅ **OK** | 0 | None | None |

## 🐛 Open Bugs (Fix First)

*No open bugs reported! Clear path for feature development.*
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

## 📜 Completed Items

- [x] **[OP-BUG-001]** Agent CLI Gateway Tailscale reachability intermittent from fracta (`agent-gateway` - bug)
- [x] **[OP-BUG-002]** System bearer rotation leaves runtime copies out of sync (`secrets` - bug)
- [x] **[OP-BUG-003]** Open Operium GitHub issues lack kind/subsystem labels (`meta` - bug)
- [x] **[OP-BUG-004]** Workstation admin-scoped npm tooling breaks user-space installs (`tooling` - bug)
- [x] **[OP-BUG-005]** Secrets research notes drift from operational secrets-management.md (`docs` - bug)
- [x] **[OP-BUG-006]** Termux shell profile trusts an inherited sentinel with an incomplete environment (`tooling` - bug)
- [x] **[OP-FEAT-001]** Automate Magistral coding-agent map apply + verify on fracta (`magistral-routing` - feature)
- [x] **[OP-FEAT-003]** Cross-device WIP handoff/resume polish (`cli` - feature)
- [x] **[OP-FEAT-008]** Bounded Termux tmux handoff helper (`cli` - feature)
