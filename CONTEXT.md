# Project Context — Jean Hugues Noël Robert, baron Mariani

*This file exists to help any collaborator — human or AI — get up to speed quickly on the current state of the project. It is a living document, updated as the project evolves. Last updated: April 2026.*

---

## The Single Question

**How do autonomous agents coordinate without a capturable centre?**

Everything else in this repository ecosystem is an answer to this question at a different scale. When in doubt, this is the thread to pull.

---

## Current Priorities (April 2026)

1. **ICOME'26** — waiting for acceptance of *Constellia* (co-authored with Guillermo Valdes). Conference in Corte, June 10–12, 2026. This is the first formal academic step.

2. **Academic credibility** — consolidating a publication record as an independent researcher without institutional affiliation. The Tocqueville paper is ready for submission; SSRN posting is the immediate next step (free, creates a citable DOI, dates priority publicly). Target journal: *European Journal of Social Theory* or *Archives européennes de sociologie*.

3. **Senatorial campaign** — candidate for French Senate, Haute-Corse, September 27, 2026 (Plan 2038, two-mandate strategy). Physical meetings with *grands électeurs* planned for August, focused on rural communes. No privileged media access; *Corse Matin* is hostile (caricatured as "illuminé souverainiste" in 2024 legislative). Strategy: bypass local media via social/direct contact, build credibility via academic recognition and institutional references.

4. **Cogentia MVP** — copy-paste workflow (prompt → personal AI agent → JSON response → analysis). Targeting GitHub Pages deployment — no server, no storage, consistent with the "know thyself" principle. Honesty indicators and PrivAI governance are prerequisites for any public deployment beyond MVP experiment. PrivAI does not yet exist.

5. **Mariani Village** — SCIC student housing in Corte, parcelle AB 0120 (540m², adjacent to Couvent des Capucins), bail à construction model, targeting landowner Sylvie Bertrand. Key legal enabler: loi Huwart (November 2025). PLU status of Corte (commune 2B096) requires verification. Not yet in GitHub — will be added.

6. **Minesteggio** — heritage investigation, DRAC Corse, Sophia Garonne as institutional relay. Not yet in GitHub — will be added.

---

## The Architecture (Six Scales)

| Scale | Project |
|---|---|
| Language | [Inox](https://github.com/virteal/Inox) — concatenative VM, control/data plane separation |
| Network | [Patent US7606221B2](https://patents.google.com/patent/US7606221B2/en) — autodiscover, no capturable server |
| Territory | [VIGILIA](https://github.com/JeanHuguesRobert/barons-Mariani/blob/main/vigilia.md) — distributed LoRaWAN detection |
| Individual | [Cogentia](https://github.com/JeanHuguesRobert/cogentia) — sovereign digital twin, Layer 4 of DHITL |
| Governance | [MareNostrum](https://github.com/JeanHuguesRobert/marenostrum) + [DHITL](https://github.com/JeanHuguesRobert/marenostrum/blob/main/DHITL.md) + Kudocracy |
| Politics | Plan 2038 · C.O.R.S.I.C.A. · Mariani Village |

The social science research is the **diagnostic** that makes the architecture necessary:
- *Generalized Tocqueville Law* → why distributed governance becomes structurally inevitable
- *Cogentia* → why personal AI alignment requires self-knowledge owned by the individual
- *Invidia* → why concentrated success is structurally destroyed in dense networks
- *Protection responsable* → why siloed institutions fail at transitions

---

## Repository Map

| Repo | Purpose | Branch |
|---|---|---|
| [JeanHuguesRobert/JeanHuguesRobert](https://github.com/JeanHuguesRobert/JeanHuguesRobert) | Profile — entry point to the ecosystem | main |
| [JeanHuguesRobert/barons-Mariani](https://github.com/JeanHuguesRobert/barons-Mariani) | Social science research + campaign + family | main |
| [JeanHuguesRobert/marenostrum](https://github.com/JeanHuguesRobert/marenostrum) | AI governance + energy sovereignty framework | main |
| [JeanHuguesRobert/cogentia](https://github.com/JeanHuguesRobert/cogentia) | Sovereign digital twin MVP | main |
| [virteal/Inox](https://github.com/virteal/Inox) | Concatenative language — edge runtime | master |

GitHub Pages active on barons-Mariani: `https://jeanhuguesrobert.github.io/barons-Mariani/`

---

## Key Working Papers (Status April 2026)

| Paper | Status | Location |
|---|---|---|
| *The Generalized Tocqueville Law* | Ready, not yet submitted | [barons-Mariani](https://github.com/JeanHuguesRobert/barons-Mariani/blob/main/tocqueville_law.md) |
| *Constellia* (with G. Valdes) | Submitted to ICOME'26, response pending | marenostrum |
| *DHITL* | Working paper | [marenostrum](https://github.com/JeanHuguesRobert/marenostrum/blob/main/DHITL.md) |
| *Cogentia Digital Twin* | Position paper | [cogentia](https://github.com/JeanHuguesRobert/cogentia/blob/main/cogentia-digital-twin.md) |
| *Invidia* | Working paper | [barons-Mariani](https://github.com/JeanHuguesRobert/barons-Mariani/blob/main/invidia.md) |
| *Protection responsable* | Working paper | [barons-Mariani](https://github.com/JeanHuguesRobert/barons-Mariani/blob/main/protection_responsable.md) |

---

## Key People

| Person | Role / Relation |
|---|---|
| Guillermo Valdes | Co-author, *Constellia* |
| Andria Fazi | Université de Corse, Mediterranean island politics — known personally, potential reader/endorser |
| Thierry Dominici | Université de Bordeaux, Corsican nationalism — known personally, potential reader/endorser |
| Sophia Garonne | DRAC Corse, key relay for Minesteggio |
| Sylvie Bertrand | Landowner, parcelle AB 0120, Mariani Village target |
| Marie-Louise Robert (Malou) | Daughter — subject of *Protection responsable*, 2024 legislative candidate |
| Lucas Robert | Son |

---

## Constraints and Context

**Financial:** significant cash flow gap currently. Claude Code (paid) not available. Working with Claude.ai web interface + git via PAT tokens.

**Institutional:** no university affiliation — deliberate, considered an advantage philosophically, but creates friction for academic publication. C.O.R.S.I.C.A. (loi 1901, Corte 1995) and Institut Mariani R&D are the institutional anchors.

**Media:** *Corse Matin* hostile. No privileged media access. Strategy is academic credibility first, direct contact second.

**Legal/political:** 2024 legislative candidacy with Marie-Louise Robert as titular. Recours au Conseil Constitutionnel — rejected September 27, 2024. Notable: the CC addressed the response to "baron Mariani" — institutional recognition of the title at national level.

**Personal philosophy:** Possibilisme — joyful exploration of the possible regardless of outcome. "Die for ideas, yes — but slowly" (Brassens). Design in the open.

---

## What Works Well with AI Assistance

- Drafting and iterating academic papers (structure, bibliography, formal argumentation)
- Git operations with PAT tokens (clone, commit, push)
- README consolidation and cross-repo coherence
- Generating interactive figures (Chart.js, SVG)
- Critical analysis of drafts (identifying weaknesses, missing references, scope conditions)
- Position papers and conceptual documents

## What Requires Human Action

- GitHub Pages activation (Settings → Pages)
- PAT token generation (https://github.com/settings/tokens/new — scope: repo, 1 day)
- Physical meetings with grands électeurs
- PrivAI institutional creation
- SSRN submission (account required)

---

*Maintained by Jean Hugues Noël Robert in collaboration with Claude (Anthropic). CC BY 4.0.*
