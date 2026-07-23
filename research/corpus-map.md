---
title: "Corpus Start Here — Carte globale du Corpus"
description: "Point d'entrée court du Living Corpus Cogentia Commons pour lecteurs humains et agents IA."
layout: default
nav_order: 0
document_role: index
status: "living map"
license: CC BY 4.0
affiliation: Institut Mariani — émanation R&D de C.O.R.S.I.C.A., 1 cours Paoli, F-20250 Corte, Corsica
date: 2026-06-18
creator: Jean Hugues Noël Robert, baron Mariani
canonical_url: https://github.com/JeanHuguesRobert/JeanHuguesRobert/blob/main/research/corpus-map.md
document_kind: "navigation"
visibility: "public"
lifecycle_state: "active"
classification_source: "cogentia.js"
classification_version: "1"
classification_rule: "explicit-index"
classification_confidence: "medium"
---

# Corpus Start Here — Carte globale du Corpus

Cette carte est le point d'entrée court du **Living Corpus Cogentia Commons**. Elle sert à rendre le corpus digérable par un lecteur humain, mais aussi par un agent IA qui doit reprendre le travail sans réinventer la structure.

Le corpus n'est pas une bibliothèque plate. C'est un ensemble de dépôts Git reliés par des documents source, des produits dérivés, des index vivants, des continuations et des décisions humaines traçables.

## À quoi sert cette page

Cette page répond à quatre questions pratiques :

1. **Où commencer ?** Lire les documents pivots avant de fouiller les catalogues.
2. **Quel dépôt sert à quoi ?** Ne pas confondre méthode, plateforme, politique, infrastructure et publication.
3. **Que peut faire un agent IA ?** Naviguer, proposer, structurer, vérifier et préparer ; ne pas décider à la place de l'auteur.
4. **Qu'est-ce qui est public ou privé ?** Le corpus public est navigable ; les registres privés ne doivent apparaître publiquement que sous forme de stubs ou de références structurelles.

## Surface publique des vues générées

Pour voir **ce qui est publié maintenant** (issues ouvertes, continuations, index, concepts, état du corpus), sans cloner les dépôts :

- **[Views Store](https://cogentia.fractavolta.com/)** — navigateur à tags des vues générées par Cogentia  
- [Documentation / API](https://cogentia.fractavolta.com/docs)  
- Exemple : [current-issues-list](https://cogentia.fractavolta.com/views/current-issues-list.md)

Les dépôts Git restent la source doctrinale et le code ; le Views Store est la **surface d'export** opérationnelle.

## Lecture en trente minutes

Pour comprendre l'ensemble sans se perdre :

1. Lire cette carte (et ouvrir le [Views Store](https://cogentia.fractavolta.com/) pour l'état publié).
2. Lire [Public Corpus Navigation](public-navigation.md) pour obtenir un ordre de lecture plus court et plus explicite.
3. Lire le [README du profil](../README.md) pour l'identité publique, le fil historique et l'intuition générale.
4. Lire [Cogentia Commons Living Corpus](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/cogentia_commons_living_corpus.md) pour le comportement attendu du corpus vivant.
5. Lire [Discours de la seconde méthode](https://github.com/JeanHuguesRobert/barons-Mariani/blob/main/research/second_method.md) pour la méthode d'exploration rationnelle du possible.
6. Lire [DHITL](https://github.com/JeanHuguesRobert/marenostrum/blob/main/DHITL.md) pour l'axiome démocratique et l'architecture anti-capture.
7. Lire [COGENTIA.md](https://github.com/JeanHuguesRobert/cogentia/blob/main/COGENTIA.md) pour le rôle concret de l'outil et du pipeline.
8. Consulter [Documents — All Tracked Repos](documents.md) ou [Corpus Status](corpus-status.md) seulement ensuite, quand il faut chercher précisément.

## Les dépôts

| Dépôt | Fonction principale | À ouvrir quand |
|---|---|---|
| [JeanHuguesRobert](https://github.com/JeanHuguesRobert/JeanHuguesRobert) | Point d'entrée, profil public, registry Cogentia, carte transversale | comprendre qui parle, quel corpus est suivi, quel état est public |
| [barons-Mariani](https://github.com/JeanHuguesRobert/barons-Mariani) | Recherche sociale, politique, patrimoniale et méthodologique | comprendre la seconde méthode, l'autonomie de capacité, les diagnostics de capture |
| [marenostrum](https://github.com/JeanHuguesRobert/marenostrum) | Souveraineté énergétique, compute, DHITL | comprendre l'axiome démocratique et l'infrastructure de gouvernance |
| [FractaVolta](https://github.com/JeanHuguesRobert/FractaVolta) | Photon-to-inference, PGN, EPN/IPN | comprendre la couche physique et distribuée de l'inférence |
| [cogentia](https://github.com/JeanHuguesRobert/cogentia) | Outillage, pipeline, continuations, mémoire opérationnelle | naviguer, vérifier, consolider, reprendre un travail agentique |
| **[Views Store](https://cogentia.fractavolta.com/)** *(export Cogentia)* | Vues générées publiques (issues, continuations, index, état) | voir l'état publié sans cloner ; API pour agents |
| [inseme](https://github.com/JeanHuguesRobert/inseme) | Plateforme civique, COP runtime, briques | comprendre la mise en artefact logiciel et multi-instance |
| [Inox](https://github.com/JeanHuguesRobert/Inox) | Langage et runtime distribués | comprendre le substrat d'exécution envisagé pour Fractanet |
| [ubikia](https://github.com/JeanHuguesRobert/ubikia) | Dérivation éditoriale source-first, publication, personas, ledger | comprendre comment un corpus source devient produit situé sans perdre la provenance |
| `registre-mariani` *(privé)* | Registre privé, informations personnelles, continuité patrimoniale et opérationnelle | ne pas explorer publiquement ; ne citer que la fonction structurelle et les liens internes autorisés |

## Public, privé, source, généré

Règles minimales de navigation :

- **Public par défaut, privé par exception.** La règle source est dans [Cogentia Commons — Public by Default, Private by Exception](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/cogentia_commons_visibility_and_private_modes.md).
- **Aucun lien public ne doit pointer vers un contenu privé.** Un dépôt privé peut pointer vers du public ; l'inverse doit rester structurel, stub ou interne.
- **Un document source porte une thèse ou une méthode.** Un produit dérivé adapte une source à un public ou une scène.
- **Un index ou un `corpus-status.md` est une vue générée ou semi-générée.** Il aide à naviguer ; il n'est pas souverain doctrinalement.
- **Un agent prépare et vérifie.** L'auteur humain arbitre les doctrines, publications, actes juridiques, engagements institutionnels et décisions sensibles.

## Documents pivots

Ces documents forment la première couche de digestion. Ils ne remplacent pas les index, mais ils disent quoi lire selon l'intention.

| Document | Statut | Lire pour | Suite naturelle |
|---|---|---|---|
| [README du profil](../README.md) | source d'orientation publique | saisir la personne, l'arc historique et le problème civilisationnel | [Project Context](../CONTEXT.md), [Agent Brief](agent_brief.md) |
| [Agent Brief](agent_brief.md) | brief opérationnel | représenter JHR sans trahir sa position ni son style | documents source cités par le brief |
| [C.O.R.S.I.C.A., Institut Mariani et corpus personnel](acorsica-et-corpus.md) | note institutionnelle transversale | distinguer personne, association, institut, corpus et initiatives futures | notes locales `acorsica-institut-mariani.md` |
| [Cogentia Commons Living Corpus](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/cogentia_commons_living_corpus.md) | source méthodologique | comprendre le comportement attendu du corpus vivant | [Agent-Resumable CLI](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/agent_resumable_cli.md) |
| [COGENTIA.md](https://github.com/JeanHuguesRobert/cogentia/blob/main/COGENTIA.md) | source d'orientation outil | comprendre Cogentia comme pipeline et compagnon de navigation | [cogentia.js tutorial](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/cogentia_js_tutorial.md) |
| [Agent-Resumable CLI](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/agent_resumable_cli.md) | source technique | comprendre pourquoi les commandes doivent être reprises par des agents | continuations actives |
| [Cognitive Packets](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/cognitive_packets.md) | source conceptuelle | comprendre l'enveloppe transportable des idées, décisions et objections | [Cognitive Packet Switching](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/cognitive_packet_switching.md) |
| [Discours de la seconde méthode](https://github.com/JeanHuguesRobert/barons-Mariani/blob/main/research/second_method.md) | source souveraine | comprendre l'exploration rationnelle du possible | [Méthode des terrains féconds](https://github.com/JeanHuguesRobert/barons-Mariani/blob/main/research/methode_terrains_feconds.md) |
| [Autonomia](https://github.com/JeanHuguesRobert/barons-Mariani/blob/main/research/autonomia.md) | source politique | comprendre l'autonomie comme capacité plutôt que statut | [Corsica2038](https://github.com/JeanHuguesRobert/barons-Mariani/blob/main/research/autonomia/corsica2038_contre_rapport_pruspettiva2050.md) |
| [Corsica2038](https://github.com/JeanHuguesRobert/barons-Mariani/blob/main/research/autonomia/corsica2038_contre_rapport_pruspettiva2050.md) | source souveraine en brouillon | relier prospective, programme, montagne, énergie, IA et capacité démocratique | revue externe, déclinaisons publiques |
| [DHITL](https://github.com/JeanHuguesRobert/marenostrum/blob/main/DHITL.md) | axiome démocratique | comprendre "One Human, One Voice" et l'anti-capture | [Infrastructure is All You Need](https://github.com/JeanHuguesRobert/marenostrum/blob/main/infrastructure_is_all_you_need.md) |
| [PGN](https://github.com/JeanHuguesRobert/FractaVolta/blob/main/PGN.md) | source infrastructurelle | comprendre le noeud photon-to-inference | [Inference Packet Network](https://github.com/JeanHuguesRobert/FractaVolta/blob/main/research/inference_packet_network.md) |
| [Inox specification](https://github.com/JeanHuguesRobert/Inox/blob/master/research/inox-spec.md) | source technique | comprendre le langage et runtime distribués | tutoriels Inox et futurs noeuds Fractanet |
| [Inseme research index](https://github.com/JeanHuguesRobert/inseme/blob/main/research/index.md) | index logiciel | comprendre la plateforme, les briques et le runtime COP | travaux locaux Inseme avant publication |

## Fiche d'orientation standard

Les documents longs devraient tendre vers ce bloc initial, placé juste après le titre :

```md
## Orientation

Statut : source souveraine / dérivé / dérivé symétrique souverain provisoire / index / opérationnel.

Fonction dans le corpus : ...

À lire avant :
- ...

À lire après :
- ...

Dépend de : ...

Continuation : ...

Dernière consolidation : YYYY-MM-DD — ...
```

Cette fiche n'est pas une formalité. Elle sert de poignée de reprise pour un agent IA et de promesse de lisibilité pour un lecteur humain.

## Chemins de lecture

### Comprendre la personne et le corpus

1. [README du profil](../README.md)
2. [Project Context](../CONTEXT.md)
3. [Agent Brief](agent_brief.md)
4. [C.O.R.S.I.C.A., Institut Mariani et corpus personnel](acorsica-et-corpus.md)

### Comprendre la méthode

1. [Discours de la seconde méthode](https://github.com/JeanHuguesRobert/barons-Mariani/blob/main/research/second_method.md)
2. [La méthode des terrains féconds](https://github.com/JeanHuguesRobert/barons-Mariani/blob/main/research/methode_terrains_feconds.md)
3. [Cogentia Commons Living Corpus](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/cogentia_commons_living_corpus.md)
4. [Cognitive Packets](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/cognitive_packets.md)

### Comprendre l'architecture anti-capture

1. [DHITL](https://github.com/JeanHuguesRobert/marenostrum/blob/main/DHITL.md)
2. [Infrastructure is All You Need](https://github.com/JeanHuguesRobert/marenostrum/blob/main/infrastructure_is_all_you_need.md)
3. [PGN](https://github.com/JeanHuguesRobert/FractaVolta/blob/main/PGN.md)
4. [Inox specification](https://github.com/JeanHuguesRobert/Inox/blob/master/research/inox-spec.md)
5. [Inseme research index](https://github.com/JeanHuguesRobert/inseme/blob/main/research/index.md)

### Comprendre la Corse comme laboratoire

1. [Autonomia](https://github.com/JeanHuguesRobert/barons-Mariani/blob/main/research/autonomia.md)
2. [Projet #1755](https://github.com/JeanHuguesRobert/barons-Mariani/blob/main/research/autonomia/projet_1755.md)
3. [Corsica2038](https://github.com/JeanHuguesRobert/barons-Mariani/blob/main/research/autonomia/corsica2038_contre_rapport_pruspettiva2050.md)
4. [Traçabilité civique anti-mafieuse](https://github.com/JeanHuguesRobert/barons-Mariani/blob/main/research/traceabilite_civique_antimafia.md)
5. [Pathologie du secret](https://github.com/JeanHuguesRobert/barons-Mariani/blob/main/research/pathologie_du_secret.md)

### Reprendre le travail comme agent IA

1. Depuis `cogentia`, lancer `node scripts/cogentia.js agent start --json` avec `COGENTIA_REGISTRY` pointant vers `JeanHuguesRobert/.cogentia.json`.
2. Si le worktree est sale, lancer `node scripts/cogentia.js git noise plan --json` pour distinguer scratch, généré et substantif.
3. Lire les gaps avec `node scripts/cogentia.js docs gaps --json`.
4. Lire les documents récents avec `node scripts/cogentia.js docs query all --sort updated --limit 20 --json`.
5. Lister les continuations avec `node scripts/cogentia.js continuation list --status active --json`.
6. Avant modification, identifier si le document est source, dérivé, index, opérationnel, public, privé ou restreint.
7. Après modification, lancer `corpus plan`, `corpus apply`, `corpus verify`, puis `corpus commit-generated --dry-run` quand des vues générées sont prêtes.

## Continuations

Les continuations sont les chemins d'exploration rationnelle du possible qui restent ouverts. Elles ne sont pas une simple todo-list : elles matérialisent le point exact où un jugement humain ou agentique est encore nécessaire.

La file active se lit avec :

```text
node scripts/cogentia.js continuation list --status active --json
```

Priorité de digestion :

1. Fermer ou requalifier les continuations obsolètes.
2. Donner une priorité explicite aux continuations actives.
3. Transformer les continuations de produits dérivés en lots éditoriaux cohérents.
4. Lier les continuations importantes aux documents source concernés.

## Règles de digestion

- Lire d'abord les sources souveraines, puis seulement les produits dérivés.
- Ne pas confondre index vivant et document doctrinal.
- Ne pas laisser un document important sans orientation initiale.
- Ne pas déplacer un document sans laisser une redirection lisible.
- Ne pas produire un dérivé sans citer ses sources.
- Ne pas fermer une continuation sans dire ce qui a été fait ou pourquoi elle devient caduque.

## État au 2026-06-18

Le corpus est techniquement synchronisé sur GitHub. Les principaux dépôts publics et le registre privé sont intégrés dans la registry Cogentia. Les vues générées, backlinks, gaps, trails, privacy checks et continuations actives sont propres au dernier passage de consolidation.

Prochaine consolidation recommandée : créer des trails supplémentaires pour les humains et agents IA :

1. **Public / privé / visibilité** — de cette carte vers la doctrine Cogentia Commons et les règles de registre privé.
2. **Cogentia → Ubikia** — de la source corpus vers la dérivation éditoriale et la publication.
3. **COP / Inseme** — de la méthode Cogentia vers le runtime de coopération.
4. **Autonomie de capacité / École Mariani** — de la seconde méthode vers les terrains pilotes.
