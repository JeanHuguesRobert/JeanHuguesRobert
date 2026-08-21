---
packet_id: CPKT-2026-008
packet_kind: cognitive-packet/v0.1
packet_version: 1
created: "2026-08-20"
title: "Session handoff — Agent JHN Instagram preparation pilot"
home_of_record: "JeanHuguesRobert/JeanHuguesRobert"
carrier: "the human author"
transmission_mode: by-copy
status: "active — human account verification and draft review required"
visibility: public
document_role: operational
document_kind: cognitive-packet-handoff
lifecycle_state: working
update_policy: UP-DEFAULT-REVIEWED
related_documents:
  - "research/etude_agent_jhn_instagram.md"
  - "research/instagram-pilot/README.md"
  - "research/instagram-pilot/publication-register.md"
  - "research/instagram-pilot/packets/ctn_ig_20260820_01.md"
  - "research/agent_brief.md"
  - "research/agent-jhn-experimental-notice.md"
---

# CPKT-2026-008 — Agent JHN Instagram preparation pilot handoff

**You are a cognitive processor receiving a continuation packet.** Resume from
the listed files and Git state, not from a previous chat transcript. This is a
preparation-only packet: it provides no authority to operate Instagram or to
publish material.

## One-line status

The JHN Instagram work is a bounded organic-content pilot in a dedicated local
branch. The policy study, a no-API pilot kit, an empty-by-design publication
register, and one source-grounded carousel draft exist. No Instagram account
was inspected, created, connected, or used; no content was published.

## Durable state

| Item | Location | State |
|---|---|---|
| Dedicated branch | `research/jhn-instagram-mandate-20260820` | checked out locally |
| Base commit | `b6beb14` | was equal to `origin/main` after fetch on 2026-08-20 |
| Policy study | `research/etude_agent_jhn_instagram.md` | uncommitted new file |
| Pilot protocol | `research/instagram-pilot/README.md` | uncommitted new file |
| Decision register | `research/instagram-pilot/publication-register.md` | uncommitted new file; one draft row |
| First proposal | `research/instagram-pilot/packets/ctn_ig_20260820_01.md` | `draft`, expires 2026-08-27 |
| This handoff | `research/CPKT-2026-008_agent_jhn_instagram_pilot_handoff.md` | uncommitted new file |
| Unrelated worktree item | `.cogentia/views-publish/` | pre-existing untracked directory; do not stage, delete, or alter |

All JHN Instagram files above are presently untracked. A normal PC restart
keeps them on disk, but they are not yet protected by a Git commit or remote
push.

## Mandate and hard limits

Agent JHN is an experimental artificial assistant, not Jean Hugues Robert,
not a voter, and not a representative. It may retrieve public sources and
prepare drafts. A human principal must decide and publish every public item.

Absolute limits for this work:

- no account creation, account setting change, API credential, connector, or
  publication without explicit human authorization;
- no paid boost, political advertising, targeting, profiling, scraping,
  follower list, automated DM, reply, like, follow or unfollow;
- no fake testimony, synthetic portrait/voice, simulated field footage, or
  material presented as a human statement unless the human has approved it;
- preserve the distinction between `agent:jhn:john`, Jean Hugues Robert, and
  the source corpus;
- do not commit or push this work unless the human explicitly authorizes that
  Git act.

## Current judgment boundary

**Classification:** `mandate_gate` / `judgment_boundary`.

The next prerequisite is a human verification of the intended Instagram
account: that it is controlled by Jean Hugues Robert, public (and professional
only if he chooses), and without boost or targeting. This packet does not ask
an agent to discover or access that account.

The second human judgment is to approve, revise, reject, or let expire
`ctn_ig_20260820_01`. It is a six-card explanatory carousel about the boundary
between preparation by an agent and human decision. It has no personal-image
requirement and no electoral fact claim.

## Safe resume commands

```powershell
cd C:\tweesic\JeanHuguesRobert
git switch research/jhn-instagram-mandate-20260820
git status --short --branch
Get-Content research\CPKT-2026-008_agent_jhn_instagram_pilot_handoff.md
Get-Content research\instagram-pilot\packets\ctn_ig_20260820_01.md
```

Then inspect the source files named in the table before changing anything.
Do not run `git clean`, `git reset --hard`, or any account/API tooling to
resume this packet.

## Ordered next actions

1. Human verifies the account preconditions in the pilot protocol.
2. Human reviews the exact first draft and records `approved`, `rejected`, or
   `expired` in the register; approval alone does not publish it.
3. If approved, the human publishes it manually and records only the public
   URL/date in the register.
4. Only after that result, prepare the second draft: a Reel whose real media
   has explicit publication authorization.
5. At day 14, review aggregate descriptive outcomes and decide whether to
   continue, modify, or stop. Do not infer a mandate for API automation.

## Return path

When resumed work reaches a meaningful boundary, update this packet by adding
an append-only hop below. Include the concrete files changed, the human
decision observed, whether any external Instagram act occurred, and any new
human decision required.

## Hop log

### Hop 0 — 2026-08-20 — preparation

- **Handler:** Codex agent, preparation-only.
- **Action:** created the policy study, pilot kit, register, and first draft.
- **External Instagram act:** none.
- **Human authorization used:** research and local branch work only; no
  publication, account, credential, commit, or push authorization.
- **Next gate:** human account verification and draft review.

### Hop 1 — 2026-08-21 — local Ubikia package generation

- **Handler:** Codex agent, preparation-only.
- **Action:** derived `research/instagram-pilot/packages/ctn_ig_20260820_01.draft.json` and `ctn_ig_20260820_01.package.json` from the existing six-card draft through Ubikia's local Instagram package generator. The resolved configuration is stored beside them without instruction content or secret values.
- **Package state:** `draft`; six media filenames are `planned`, not rendered or verified; manual publication and human editorial/account-context checks remain required.
- **External Instagram act:** none; no account access, API call, remote draft, schedule, publication, interaction, targeting, or spend.
- **Human authorization used:** local preparation only.
- **Next gate:** the existing human account verification and exact-draft review; rendering or selecting the six media files needs a separate review of the visual template and assets.

### Hop 2 — 2026-08-21 — local typographic card drafts

- **Handler:** Codex agent, preparation-only.
- **Action:** prepared six simple 1080×1350 SVG typographic card drafts beside the package (`card-01.svg` through `card-06.svg`) and regenerated the package with `media_status: available`.
- **Design status:** neutral reversible template only (ivory, navy, terracotta; no portrait, logo, synthetic image, or factual addition). The SVGs are not yet human-validated, rasterized, or verified against the platform's current upload requirements.
- **External Instagram act:** none.
- **Next gate:** human visual/template review, then a local raster export and asset verification before the existing editorial/account review and manual publication gates.

### Hop 3 — 2026-08-21 — conversation closure and durable resume point

- **Classification:** `mandate_gate` / `judgment_boundary`; the remaining work is not a technical failure.
- **Handler:** Codex agent, preparation and corpus-stabilization mandate only.
- **Durable state:** the pilot and its six SVG card drafts were integrated into `JeanHuguesRobert/JeanHuguesRobert` `main` at `1b0f67bde28c61cead8d8d17ea3a4a63a8d53340`. The untracked local `.cogentia/views-publish/` directory was pre-existing and remains excluded.
- **Related durable changes:** Cogentia public-presence doctrine at `a360eeb286630f44caa640fd31309298d1b0173a`; Ubikia public-presence policy at `b3b3143958899ad72e9e39dc9e6ea6ed7f6bf12e`; local Instagram package generator at `a77413b7f71c031a1e0c523b30ce2cf630d5fad1`.
- **Current proposal:** `ctn_ig_20260820_01` remains `draft`; its package has `media_status: available`, but its SVG cards have not been human-validated, rasterized, or verified against current upload requirements.
- **External Instagram act:** none throughout this work: no account access, setting, credential, API call, remote draft, schedule, publication, interaction, targeting, data collection, or spend.
- **Human decisions still required:** (1) verify the intended account and its no-boost/no-targeting condition; (2) approve, revise, reject, or expire the exact draft and its visual template; (3) personally publish manually if approved. Approval does not authorize agent publication.
- **Deferred doctrinal continuations:** stabilize the naming/identity architecture (principal, *Les Carnets du Baron Mariani*, Barons Mariani / future Fonds); add a dated non-secret account-activation checklist; optionally develop the documented critique of *personal branding* into a sourced corpus note.
- **Safe resume:** `git pull`; read this file, `research/instagram-pilot/README.md`, `research/instagram-pilot/packets/ctn_ig_20260820_01.md`, and `research/instagram-pilot/packages/ctn_ig_20260820_01.package.json`; then inspect current platform requirements before any connector or remote act.
