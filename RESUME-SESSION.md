---
document_role: "operational"
document_kind: "continuation-packet"
visibility: "public"
lifecycle_state: "active"
classification_source: "cogentia.js"
classification_version: "1"
classification_rule: "continuation-resume"
classification_confidence: "strong"
---

# Workspace Continuation & Session Handoff (July 31, 2026) 📜🌐🚀

> **Status**: **DELIVERABLE v1, SSE STREAMING, PURE EMBEDDINGS, AUTONOMOUS WORKER, 2026-W31 DIGEST & GENERIC DIGITAL TWIN ENGINE COMPLETED** 🎉 (Public Guide Web UI live at `https://cogentia.fractavolta.com/guide`; Generic Digital Twin Engine & Instance Bindings published; Agent JHN bound to `JeanHuguesRobert/JeanHuguesRobert`).

---

## 🎯 Completed Deliverables & Milestones

### 1. Public Guide Web Application (Deliverable v1)
- **Web UI**: Live at `https://cogentia.fractavolta.com/guide` (Modern dark theme, glassmorphism, EN/FR multi-language, interactive starter prompts, responsive chat stream).
- **Real-Time SSE Streaming**: Fully enabled (`text/event-stream`). Emits live visual progress stages (`guide_status`, `guide_plan`, `guide_retrieval`, `guide_answer`, `done`) directly to the browser chat interface.
- **API Endpoint**: `POST https://cogentia.fractavolta.com/guide/chat`
- **Retrieval**: S7 Layered Retrieval (Layer 1 S7 deterministic alias resolve + Layer 2 Frontmatter filtering + Layer 3 Vector / Keyword search).
- **Synthesis Mode**: **`mode=conversational`** (VERIFIED LIVE IN EN & FR).
- **Infrastructure Reliability**: 24/7 OpenRouter cloud fallback in Magistral AI router on `fracta` node with fail-fast router-only capability routing.

### 2. Pure Signal Embeddings Calibration & Noise Pruning
- **Diagnostic**: Identified 1,572 noisy chunks (short fragments < 120 chars, auto-generated backlink blocks, raw templates, structural indices) diluting vector similarity.
- **Signal Filter**: Enforced min-length (>= 120 chars), excluded `<!-- END_AUTO: backlinks -->`, `Backlinks`, `*_template.md`, and structural index files in `cogentia.js`.
- **Database Pruning**: Pruned 1,572 noisy vector rows locally and on production VPS `fracta`.
- **Active Index**: Rebuilt `sqlite-vec` v0.1.9 index with **7,391 pure high-signal vector rows** active on `fracta`.

### 3. Autonomous Node Worker & Site Update Migration
- **Daemon Health**: Confirmed `operium-node-agent.service` (`resource://fracta`) running 24/7 at `:8794` with `health_score: 4`.
- **Autonomous Worker Execution**: Dispatched background worker `/srv/cogentia/work/update_fractavolta_site_remote.js` on `fracta`.
- **Merged & Published**: 38 curated papers across 6 stack layers committed to `docs/_data/papers.yml` and merged into `main` on GitHub (`https://fractavolta.com/papers`).

### 4. Generic Digital Twin Engine, Mandates & Persona Governance (`digital-twin-engine.js`)
- **Engine Architecture**: Extracted generic Digital Twin runtime ([`scripts/lib/digital-twin-engine.js`](file:///C:/tweesic/cogentia/scripts/lib/digital-twin-engine.js)) separating shared execution mechanisms from instance-specific configurations.
- **Universal External Surface Contract (`EXTERNAL_SURFACE_CONTRACT`)**: Encodes the normative invariant for ALL Digital Twin external chatbots (whether Agent JHN's Guide, Ophélia, or future collective twins): **`readonly` exploratory guide**, **zero financial/legal guarantees**, **zero legal engagement**.
- **Mandate & Persona Governance**: Encodes `active_mandate` (e.g. `MND-JHN-GUIDE-v1`, `MND-PERTITELLU-OPHELIA-v1`) and `persona` boundaries. Read-only by default; any capability expansion beyond read-only requires a formal versioned Mandate revision.
- **Personal Twin Binding (`jhn-personal`)**: Bound to Principal Sovereign Source of Truth **`JeanHuguesRobert/JeanHuguesRobert`** (`INTENT_KERNEL.md`, `POSSIBILISM.md`), with self-chat WhatsApp scope and `— agent-jhn-experimental (readonly, zero guarantees)` disclosure.
- **Collective Twin Binding (`pertitellu-corte`)**: Bound to Principal Sovereign Source of Truth **`JeanHuguesRobert/pertitellu`** (*Ophélia* / *The Pertitellu Civic Guide*, municipal program, public civic chat).
- **Supabase Operational Mirror**: Reads runtime configuration overrides from Supabase `instance_config` table without placing heavy load on `fracta` VPS.
- **Test Suite**: 100% PASS on [`scripts/test-digital-twin-engine.js`](file:///C:/tweesic/cogentia/scripts/test-digital-twin-engine.js), committed & pushed to GitHub (`commit 6b4f5fd`).

### 5. Agent JHN WhatsApp S7 Cognitive Retrieval & Preemptible Sleep Cycle
- **WhatsApp Cognitive Synthesis**: Integrated `buildCognitiveDraft()` in [`scripts/lib/agent-jhn-whatsapp/draft.js`](file:///C:/tweesic/cogentia/scripts/lib/agent-jhn-whatsapp/draft.js). Answers self-chat questions using S7 retrieval and Magistral AI synthesis over 7,391 pure vector embeddings. 23/23 unit tests PASS.
- **Dynamic Availability Qualification Engine**: Created [`scripts/lib/idle-qualification.js`](file:///C:/tweesic/cogentia/scripts/lib/idle-qualification.js) checking real-time CPU load, memory, and active requests instead of hardcoded cron times.
- **Preemptible Corpus Sleep Cycle Runner**: Created and executed [`scripts/run-corpus-sleep-cycle.js`](file:///C:/tweesic/cogentia/scripts/run-corpus-sleep-cycle.js). Performs Monte Carlo pairwise audits and vector checks when system availability is qualified. Committed & pushed to GitHub (`commit bf61b7a`).
### 6. Console de Contrôle Operium & Panneau d'Actions SOMA
- **Panneau d'Actions SOMA (`SomaActionsPanel.jsx`)** : Intégré dans l'application Operium Console ([`operium/apps/console/src/components/SomaActionsPanel.jsx`](file:///C:/tweesic/operium/apps/console/src/components/SomaActionsPanel.jsx)).
- **Déclenchement d'Actions en Direct** : Permet aux opérateurs de déclencher `sleep_cycle.run` (*Run preemptible Corpus Sleep Cycle*), `observation.refresh`, et `agent.restart` avec retour visuel d'exécution et gestion d'erreurs.
- **Build & Publication GitHub** : Build client Vite compilé avec succès (`dist/assets/index-NmlF4I8F.js`), commit `77d44cd` poussé sur `main`.

### 7. Inseme Issue #28 & #29 — Schema & Ingress Webhook COP Append-Only
- **Migration SQL (`20260731180000_cop_append_only_event_log.sql`)** : Livrée dans [`inseme/apps/platform/supabase/migrations/20260731180000_cop_append_only_event_log.sql`](file:///C:/tweesic/inseme/apps/platform/supabase/migrations/20260731180000_cop_append_only_event_log.sql). Commit `91b9141`.
- **Adaptateur d'Entrée Webhook & Normalisateur (`github-ingress.js`)** : Livré dans [`inseme/packages/cop-core/src/github-ingress.js`](file:///C:/tweesic/inseme/packages/cop-core/src/github-ingress.js). Commit `e5cec1d`.
- **Fonction Edge Webhook Deno Moderne (`github-webhook.js`)** :
  - Livrée dans [`inseme/apps/platform/netlify/edge-functions/github-webhook.js`](file:///C:/tweesic/inseme/apps/platform/netlify/edge-functions/github-webhook.js) au format moderne Deno Edge (Web Crypto API `crypto.subtle` native, pas de Node.js hérité).
  - Expose `/api/webhooks/github` (déclaré dans `netlify.toml`).
  - Validation HMAC-SHA256, enregistrement dans Supabase `github_webhook_deliveries` et normalisation instantanée dans `cop_event_log` (`cop.event/v1`).
  - Réponse asynchrone rapide `202 Accepted`.
- **Tests & Publication GitHub** : Suite de tests JS ESM validée à 100% dans [`inseme/scripts/test-deno-github-webhook-edge.js`](file:///C:/tweesic/inseme/scripts/test-deno-github-webhook-edge.js). Commit `84e3f45` poussé sur la branche `main` de **`JeanHuguesRobert/inseme`**.
- **Résolution des Échecs de Build Netlify CI & Nettoyage Architecturel** :
  1. *ERR_PNPM_OUTDATED_LOCKFILE* : Lockfile réaligné (`pnpm-lock.yaml`) suite à l'ajout de `@supabase/supabase-js`.
  2. *Esbuild Export Resolution Error* : Ajout de `"./src/*"` et `"./client/*"` dans le map `exports` de [`packages/cop-host/package.json`](file:///C:/tweesic/inseme/packages/cop-host/package.json) pour autoriser l'importation de `@inseme/cop-host/src/client/supabase.js` par les Netlify Functions.
  3. *Heap Out of Memory Error* : Déclaration de `NODE_OPTIONS = "--max-old-space-size=4096"` sous `[build.environment]` dans [`apps/platform/netlify.toml`](file:///C:/tweesic/inseme/apps/platform/netlify.toml).
  4. *Suppression Nettoyage `tipping.js` Orphelin* : Suppression du fichier orphelin `apps/platform/netlify/functions/tipping.js` (propre uniquement à Cyrnea) et retrait de `jsonwebtoken` des dépendances de `apps/platform/package.json`. Commit `84e3f45`.
  5. *Ignore Logs* : Inscription de `tmp/` et `**/.temp/` dans [`.gitignore`](file:///C:/tweesic/inseme/.gitignore).

### 5. Corpus README.md Synchronization & 2026-W31 Weekly Digest
- **Corpus READMEs**: `cogentia`, `barons-Mariani`, `FractaVolta`, `operium` updated and pushed to GitHub.
- **2026-W31 Weekly Consolidation**: Executed `cogentia consolidate --weekly`. Generated & published [`weekly_digest_2026-W31.md`](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/sprints/weekly_digest_2026-W31.md), root `llms.txt`, `llms-full.txt`, and `docs/registry.json`.

---

## 💻 Zero-Local-State Machine & Agent Resumption Instructions

> **Note importante** : Tout le travail en cours a été commité et poussé sur GitHub. Aucune donnée ou état n'est dépendant de la machine locale ou de la mémoire d'un agent spécifique.

### 🌐 Dépôts GitHub de Référence (Branches `main`)
- **Souverain Racine JHN** : [`https://github.com/JeanHuguesRobert/JeanHuguesRobert`](https://github.com/JeanHuguesRobert/JeanHuguesRobert) (contient `RESUME-SESSION.md`, `INTENT_KERNEL.md`, `POSSIBILISM.md`)
- **Plateforme Inseme** : [`https://github.com/JeanHuguesRobert/inseme`](https://github.com/JeanHuguesRobert/inseme) (contient `apps/platform`, `packages/cop-core`, `supabase/migrations`)
- **Pertitellu / Corte** : [`https://github.com/JeanHuguesRobert/pertitellu`](https://github.com/JeanHuguesRobert/pertitellu)
- **Cogentia Twin Engine** : [`https://github.com/JeanHuguesRobert/cogentia`](https://github.com/JeanHuguesRobert/cogentia)

### 🛠️ Prérequis de la Machine Cible
- **Node.js** : `>= 24.0.0`
- **Gestionnaire de paquets** : `pnpm` v10 (Corepack activé : `corepack enable`)
- **Projet Supabase JHN** : `ndiysuhzmztatpxbkezn` (`https://ndiysuhzmztatpxbkezn.supabase.co`)
- **Règles de Code Strictes** :
  - ❌ **PAS DE PYTHON** (Tout en JavaScript ESM natif, sans TypeScript si possible).
  - ⚡ **Fonctions Edge** : Au format Deno moderne (`export default async (request, context) => ...`).

---

## 🎯 Prochaine Tâche Immédiate à la Reprise : Inseme Issue #31

**Objectif** : Implémenter le générateur de projections d'activité humaine ([`packages/cop-core/src/activity-projection.js`](file:///C:/tweesic/inseme/packages/cop-core/src/activity-projection.js)).

1. **Fonctionnalité** : Lire les événements normalisés `cop.event/v1` depuis la table `cop_event_log` et reconstruire le flux d'activité lisible pour le mandant / l'instance.
2. **Spécification** :
   - Agrégation par `topic_id` et séquence `topic_seq`.
   - Transformation des événements `push`, `pull_request`, `issues`, `workflow_run`, `security_alert` en items de fil d'activité lisibles par des humains.
3. **Validation** : Écrire et valider la suite de tests JS ESM (`node scripts/test-activity-projection.js`).

---

## 🎯 Déclencheur Simple de Reprise (1 Seule Phrase)

Pour n'importe quel agent de développement AI sur n'importe quelle machine, il vous suffira de taper simplement :

> **`Check issue 31 of Inseme`**  
> *(ou : "Poursuis l'issue 31 d'Inseme")*

### 📜 Ce que l'agent exécutera immédiatement :
1. **Source de Vérité** : Consulter `RESUME-SESSION.md` dans `JeanHuguesRobert/JeanHuguesRobert` et l'issue #31 sur `JeanHuguesRobert/inseme`.
2. **Action** : Développer le module [`packages/cop-core/src/activity-projection.js`](file:///C:/tweesic/inseme/packages/cop-core/src/activity-projection.js) pour agréger les événements `cop.event/v1` (`push`, `issues`, `pull_request`, `workflow_run`, `security_alert`) depuis la table Supabase `cop_event_log` et générer le flux d'activité humaine lisible pour l'instance JHN.
3. **Validation** : Exécuter la suite de tests JS ESM (`node scripts/test-activity-projection.js`) et commiter/pousser sur GitHub `main`.
