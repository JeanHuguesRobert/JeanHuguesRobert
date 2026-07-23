---
title: "Public Corpus Navigation"
description: "Compact public navigation map for the corpus, derived from registry metadata."
layout: default
nav_order: 2
date: 2026-07-23
license: CC BY 4.0
document_role: index
document_kind: navigation
visibility: public
lifecycle_state: active
derived_from: ".cogentia.json"
classification_source: "cogentia.js"
classification_version: "1"
classification_rule: "explicit-index"
classification_confidence: "strong"
---

# Public Corpus Navigation

This page is the short public map for the corpus.

It is derived from the registry metadata in [`.cogentia.json`](../.cogentia.json) and keeps the first question simple:

what should a human, an agent, or a site visitor open first?

## Live surface (generated views)

Before diving into GitHub trees, the **public published state** of the corpus is browsable here:

| Surface | URL | For |
|---------|-----|-----|
| **Views Store** | https://cogentia.fractavolta.com/ | Humans & agents — tag browser over generated views (issues, continuations, indexes, concepts, env samples, corpus-state) |
| Views API docs | https://cogentia.fractavolta.com/docs | Machines — list/filter contract |
| Example: open issues | https://cogentia.fractavolta.com/views/current-issues-list.md | Operational “open work” aggregate |

Source repositories remain the authority for doctrine and code; the Views Store is the **export surface**, not a second source of truth.

## Reading paths

### Human reader

1. **[Views Store](https://cogentia.fractavolta.com/)** — what is published *now*
2. [Corpus Start Here — Carte globale du Corpus](corpus-map.md)
3. [Research Index — Jean Hugues Noël Robert](index.md)
4. [README](../README.md)
5. [Cogentia Commons Living Corpus](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/cogentia_commons_living_corpus.md)
6. [Discours de la seconde méthode](https://github.com/JeanHuguesRobert/barons-Mariani/blob/main/research/second_method.md)
7. [DHITL](https://github.com/JeanHuguesRobert/marenostrum/blob/main/DHITL.md)
8. [COGENTIA.md](https://github.com/JeanHuguesRobert/cogentia/blob/main/COGENTIA.md)

### Agent reader

1. **[Views Store](https://cogentia.fractavolta.com/)** + [API docs](https://cogentia.fractavolta.com/docs) — published operational views
2. [Research Index — Jean Hugues Noël Robert](index.md)
3. [Cogentia Commons Living Corpus](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/cogentia_commons_living_corpus.md)
4. [Agent-Resumable CLI](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/agent_resumable_cli.md)
5. [cogentia.js tutorial](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/cogentia_js_tutorial.md)
6. [Corpus Status](corpus-status.md)

### Site visitor

1. **[Views Store](https://cogentia.fractavolta.com/)** — corpus export browser (no Git clone required)
2. [FractaVolta](https://github.com/JeanHuguesRobert/FractaVolta) / [fractavolta.com](https://fractavolta.com/)
3. [FractaVolta research index](https://github.com/JeanHuguesRobert/FractaVolta/blob/main/research/index.md)
4. [Packetized Gravity Networks (PGN)](https://github.com/JeanHuguesRobert/FractaVolta/blob/main/PGN.md)
5. [Public / private split](https://github.com/JeanHuguesRobert/operium/blob/main/docs/public-private-split.md)

## Ranked entry points

| Rank | Repository | Role | Start here | Public index | Primary reader |
|---|---|---|---|---|---|
| 1 | JeanHuguesRobert | entry point | `research/corpus-map.md` | `research/index.md` | human |
| 2 | barons-Mariani | source | `README.md` | `research/index.md` | human |
| 3 | marenostrum | doctrine | `README.md` | `research/index.md` | human |
| 4 | cogentia | tooling | `README.md` | `research/index.md` | agent |
| 5 | FractaVolta | site_facing | `README.md` | `research/index.md` | human |
| 6 | inseme | platform | `README.md` | `research/index.md` | mixed |
| 7 | ubikia | publication | `README.md` | `research/index.md` | human |
| 8 | operium | methodology | `README.md` | `docs/public-private-split.md` | human |
| 9 | Inox | runtime | `README.md` | `research/index.md` | human |
| 99 | registre-mariani | private_registry | n/a | n/a | internal |

## Notes

- The **Views Store** is the preferred entry for *generated* operational state; GitHub remains the entry for *source* documents and code.
- `registre-mariani` is intentionally only a structural stub in public navigation.
- The site-facing path for FractaVolta remains the GitHub repo and its site surface; the registry only says where the public reader should begin.
- `StructEnv` is registered tooling with a planned revival; it is not yet a ranked reading path.
- This page is a navigation layer, not a doctrinal source.
