---
title: "Public Corpus Navigation"
description: "Compact public navigation map for the corpus, derived from registry metadata."
layout: default
nav_order: 2
date: 2026-06-25
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

## Reading paths

### Human reader

1. [Corpus Start Here — Carte globale du Corpus](corpus-map.md)
2. [Research Index — Jean Hugues Noël Robert](index.md)
3. [README](../README.md)
4. [Cogentia Commons Living Corpus](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/cogentia_commons_living_corpus.md)
5. [Discours de la seconde méthode](https://github.com/JeanHuguesRobert/barons-Mariani/blob/main/research/second_method.md)
6. [DHITL](https://github.com/JeanHuguesRobert/marenostrum/blob/main/DHITL.md)
7. [COGENTIA.md](https://github.com/JeanHuguesRobert/cogentia/blob/main/COGENTIA.md)

### Agent reader

1. [Research Index — Jean Hugues Noël Robert](index.md)
2. [Cogentia Commons Living Corpus](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/cogentia_commons_living_corpus.md)
3. [Agent-Resumable CLI](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/agent_resumable_cli.md)
4. [cogentia.js tutorial](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/cogentia_js_tutorial.md)
5. [Corpus Status](corpus-status.md)

### Site visitor

1. [FractaVolta](https://github.com/JeanHuguesRobert/FractaVolta)
2. [FractaVolta research index](https://github.com/JeanHuguesRobert/FractaVolta/blob/main/research/index.md)
3. [Packetized Gravity Networks (PGN)](https://github.com/JeanHuguesRobert/FractaVolta/blob/main/PGN.md)
4. [Public / private split](https://github.com/JeanHuguesRobert/operium/blob/main/docs/public-private-split.md)

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

- `registre-mariani` is intentionally only a structural stub in public navigation.
- The site-facing path for FractaVolta remains the GitHub repo and its site surface; the registry only says where the public reader should begin.
- This page is a navigation layer, not a doctrinal source.
