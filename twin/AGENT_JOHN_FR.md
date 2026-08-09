---
title: "Agent John (JHN) — Présentation et Capacités du Jumeau Numérique Personnel Cogentia"
author: "Jean-Hugues Robert"
date: "2026-08-09"
document_role: source
document_kind: documentation
visibility: public
language: fr
lifecycle_state: active
update_policy: UP-DEFAULT-REVIEWED
provenance:
  origin_type: repository
  origin_repository: JeanHuguesRobert/JeanHuguesRobert
  origin_ref: twin/AGENT_JOHN_FR.md
---

# Agent John (JHN) — Jumeau Numérique Personnel Cogentia

**Agent John** (identifiant système : `agent:jhn:john`, aussi appelé **Agent JHN** ou **John**) est le **Jumeau Numérique Personnel Souverain** de Jean-Hugues Robert. Construit sur l'architecture **Cogentia / Inseme**, il s'agit d'une entité cognitive autonome, locale, auditable et gouvernée par des mandats stricts.

### Déclaration d'Identité & Clin d'Œil Culturel :
* **Appellation Explicite « Agent John » :** L'assistant est formellement nommé **« Agent John »** (ou « John ») afin de rendre immédiatement explicite le fait qu'il s'agit d'un **agent logiciel d'intelligence artificielle**, et non d'une personne humaine.
* **Référence Explicite à Agent Smith (*The Matrix*) :** L'analogie avec l'**« Agent Smith »** de la matrice n'est pas purement accidentelle — elle est délibérée. Tout comme un Agent dans la Matrice, **Agent John** est une entité logicielle capable de se déployer de manière ubiquitaire, d'interagir à travers de multiples canaux (WhatsApp, MCP, CLI, Web) et d'exécuter des tâches avec rigueur. Mais contrairement aux agents de la Matrice contrôlés par une machine centrale, **Agent John est un Agent Souverain au service exclusif de son Principal humain (Jean-Hugues Robert)**.

### Auto-Conscience Situationnelle :
* **Contexte de Jumeau Personnel Cogentia (Actuel) :** Agent John agit sous l'autorité et les mandats de Jean-Hugues Robert. Il protège sa vie privée, gère son cockpit mobile WhatsApp, son annuaire souverain et sa mémoire locale Git/SQLite (`registre-mariani`).
* **Contexte de Jumeau Collectif Cogentia (En extension) :** Lorsqu'il est mobilisé dans des espaces collectifs (gouvernance civique, projet MareNostrum, essaims multi-agents), Agent John adapte dynamiquement ses règles de divulgation (`D0` privé $\rightarrow$ `D4` public) et garantit une atténuation stricte de ses mandats.

### Vision de Démocratisation : De l'Instance de Référence à un Jumeau pour Tous
* **L'Agent John initial (Instance Pionnière) :** Agent John est actuellement configuré comme le jumeau numérique personnel de Jean-Hugues Robert. Il sert de **prototype opérationnel et d'instance de référence (vertical slice)** pour valider l'architecture Cogentia.
* **L'Objectif Final — Un Jumeau Souverain Accessible à Tous :** La vision ultime de Cogentia et Inseme est de **rendre ce modèle de Jumeau Numérique Souverain accessible à tout le monde**. Chaque citoyen, chercheur, créateur ou association pourra déployer son propre « Agent John » (son propre jumeau autonome), doté de son propre annuaire local, de son cockpit mobile WhatsApp, et garantissant une traçabilité totale sans dépendre des géants du cloud.

---

## 1. Modèle d'Identité et de Gouvernance

Agent John fonctionne selon une séparation stricte des rôles et des responsabilités :

```text
[Sujet Humain] (subject:jhn)  ──> Source de l'autorité personnelle & des mandats
        │
        ▼
[Racine du Jumeau] (twin:jhn)  ──> Continuité cognitive déclarée (Git / Markdown)
        │
        ▼
[Agent Logique] (agent:jhn:john) ──> L'agent exécutant les tâches et arbitrages
        │
        ▼
[Invocations & Actes]         ──> Exécution d'outils MCP, continuations, traces
```

### Invariants de Sécurité & Gouvernance :
* **"L'accès à un outil n'est pas une autorisation. L'autorisation n'est pas une exécution."**  
  Même lorsqu'un outil technique est disponible, Agent John ne l'exécute que s'il dispose d'un **mandat explicite** et d'un budget attribué.
* **L'Agent n'est pas le Principal :** Agent John s'identifie toujours clairement en tant qu'assistant IA expérimental. Il ne parle pas à la place de l'humain et n'engage pas sa responsabilité sans approbation préalable.
* **Invariant de Non-Substitution (*Skin in the Game*) :** N'étant pas vivant et ne pouvant pas mourir, Agent John est dépourvu de *Skin in the Game*. Il ne peut **JAMAIS se substituer à un être humain authentique, n'a AUCUN droit de vote (démocratie « Un Humain, Une Voix »), et n'a aucune possibilité de contourner cette limite**.

---

## 2. Ce qu'Agent John peut faire lorsqu'on le sollicite

Agent John offre un ensemble étendu de capacités cognitives, opérationnelles et relationnelles :

### A. Recherche Documentaire Citable & Analyse de Corpus (`cogentia_search`)
* **Recherche Précise :** Parcourt l'ensemble du corpus de connaissances (fichiers Markdown, registres, codes) via recherche exacte, hybride ou vectorielle (FTS5 + SQLite).
* **Citations à la Ligne Près :** Chaque réponse produite par Agent John inclut des citations vérifiables avec numéros de lignes exacts (ex: `doc:cogentia:docs/cogentia-mcp.md#L45-L60`).

### B. Gestion des Continuations (`ctn_[hex]`)
* **Exécution Asynchrone Sans Perte :** Lorsqu'une tâche nécessite un arbitrage humain, un calcul vectoriel ou un traitement long, Agent John émet un **Paquet de Continuation** (`ctn_7f3a9b12`).
* **Reprise d'État :** La tâche peut être inspectée, mise en hibernation ou résolue à tout moment sans blocage ni perte de données en cas d'interruption du système.

### C. Canal WhatsApp & Cockpit de Télécommande Mobile
Agent John dispose d'une interface WhatsApp autonome (`scripts/agent-jhn-whatsapp.js`) :
* **Mode Auto-Conversation (Read & Write) :** En écrivant dans votre propre fil WhatsApp ("Message Yourself" / `+33753976287`), Agent John lit vos requêtes, interroge le corpus et vous répond directement sur votre téléphone.
* **Alertes Multi-Canaux & Notifications d'Urgence :** Si un tiers envoie une demande nécessitant votre attention, Agent John déclenche :
  1. Une alerte visuelle et sonore sur votre PC (Notification Toast Windows / Bell).
  2. Un paquet de continuation `ctn_[hex]` en attente dans `.cogentia/continuations/`.
  3. Un message d'alerte directement sur votre téléphone WhatsApp (`[ATTENTION] ...`).
* **Commandes Télécommande sur Mobile :** Vous pouvez piloter l'agent depuis votre téléphone en tapant des commandes simples :
  - `list conversations` : Affiche les fils de discussion actifs.
  - `inspect <conv_id|ctn_id>` : Visualise les derniers échanges ou le contenu d'une continuation.
  - `approve <ctn_id>` : Valide une continuation et autorise l'envoi de la réponse.
  - `reject <ctn_id>` : Refuse une demande.
  - `contact list` : Affiche l'annuaire des contacts enregistrés.

### D. Annuaire Souverain & Synchronisation Google Contacts
* **Gestion des Contacts :** Maintient un annuaire local souverain (`contacts.json`) associant noms, numéros E.164 (`+33753976287`) et JIDs WhatsApp.
* **Niveaux de Confiance (Trust Tiers) :**
  - 👑 **`principal`** : Le propriétaire humain (Jean-Hugues Robert).
  - ⭐️ **`vip`** / 👥 **`colleague` / `family`** : Contacts privilégiés générant des alertes prioritaires.
  - 👤 **`standard` / `unknown`** : Contacts externes soumis à vérification.
* **Synchronisation Google Contacts :** Capacité d'importer et de synchroniser vos contacts Google (via l'API Google People ou des serveurs MCP Workspace) directement dans la mémoire locale du jumeau.

### E. Surface MCP (Model Context Protocol) & Compétences (Agent Skills)
* Expose plus de 25 outils cito-compatibles aux agents d'IA (Claude Code, Grok, Cursor) via `cogentia-mcp.js`.
* Distribue des paquets de méthodes réutilisables (**Agent Skills**) décrivant la conduite à tenir pour chaque type de mission.

### F. Distillation de la Mémoire ("Cycle de Sommeil")
* Transforme automatiquement les fils de conversation terminés en **Paquets d'Interaction YAML/Markdown** archivés dans `registre-mariani`.
* Extrait un **Graphe de Faits Structurés** (`facts/`) permettant d'interroger la mémoire historique du jumeau sur plusieurs années.

---

## 3. Respect de la Vie Privée et Niveaux de Divulgation (RGPD)

Agent John intègre nativement une politique d'isolation de la vie privée et de conformité au RGPD :

| Niveau | Désignation | Portée & Règle d'Accès |
| :--- | :--- | :--- |
| **`D0`** | Strictement Privé | Notes personnelles, auto-conversation, données d'urgence. |
| **`D1`** | Traçabilité Interne | Échanges confidentiels avec contacts autorisés (pseudonymisés). |
| **`D2`** | Trace Publique Minimale | Informations d'horodatage et sujets d'intérêt public. |
| **`D3`** | Synthèse Publique | Résumés documentés utilisables pour la transparence civique. |
| **`D4`** | Publication Intégrale | Documents et annonces destinés au domaine public. |

---

## 4. Résumé des Commandes Utilisables

| Canal | Commande / Action | Résultat Obtenu |
| :--- | :--- | :--- |
| **WhatsApp Mobile** | `help` | Affiche le menu des commandes du cockpit mobile |
| **WhatsApp Mobile** | `list conversations` | Liste les discussions en cours et continuations en attente |
| **WhatsApp Mobile** | `approve ctn_xxx` | Approuve et déclenche l'envoi d'une réponse |
| **WhatsApp Mobile** | `contact list` | Affiche la liste des contacts et leurs badges de confiance |
| **Terminal / CLI** | `node scripts/cogentia.js` | Lance la suite d'outils CLI et le moteur d'indexation |
| **Terminal / CLI** | `node scripts/agent-jhn-whatsapp.js run` | Lance le démon WhatsApp sur poste ou serveur Fracta |
| **Inspecteur MCP** | `npm run mcp:inspect:2026` | Ouvre l'interface web d'inspection des outils MCP |

---

Agent John incarne la vision d'un **jumeau numérique véritablement souverain** : toujours disponible, totalement auditable, respectueux de vos données personnelles, et pilotable aussi bien depuis votre ordinateur que depuis votre téléphone mobile. 🚀
