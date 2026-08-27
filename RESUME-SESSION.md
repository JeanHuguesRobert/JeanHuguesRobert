---
document_role: "operational"
document_kind: "continuation-packet"
visibility: "public"
lifecycle_state: "active"
classification_source: "cogentia.js"
classification_version: "1"
classification_rule: "continuation-resume"
classification_confidence: "strong"
packet_id: "cop-pkt-20260828-inseme-57-hosted-twins"
packet_type: "cop.continuation_packet/v1"
packet_version: "1.0.0"
topic_id: "topic:twins:hosted-provisioning"
producer_ref: "agent:antigravity"
causal_refs:
  - "https://github.com/JeanHuguesRobert/inseme/issues/57"
  - "commit:457561b"
  - "commit:302c19c"
  - "commit:63cd284"
  - "commit:3a9e194"
epistemic_status: "decided"
required_capabilities:
  - "supabase:db:ndiysuhzmztatpxbkezn"
  - "git:branch:main"
  - "x:archive_ingestion"
date: "2026-08-28"
---

# Workspace Continuation & Session Handoff (August 28, 2026) 📜🌐🚀

> **Status**: **HOSTED DIGITAL TWINS PROVISIONED, MONOTONE ALIAS REGISTRY & X/TWITTER BOOTSTRAP PIPELINE COMPLETED** 🎉  
> Live on Supabase Production (`ndiysuhzmztatpxbkezn`); Git commits pushed to `main` on `JeanHuguesRobert/inseme`; Twitter archive requested on `@suvranu`.

---

## 🎯 Active Digital Twins & Infrastructure Status

### 1. The 4 Provisioned Twins on Supabase Production (`ndiysuhzmztatpxbkezn`)
All 4 instances are live in `public.instances` with canonical UUIDs and hierarchical hosting:

| Canonical UUID | Canonical Slug | Display Name | Bot / Persona | Kind / Purpose | Host |
| :--- | :--- | :--- | :--- | :--- | :--- |
| `00000000-0000-0000-0000-000000000001` | `jhn` | Jean Hugues Noël Robert | John | `living_person` (Root Host) | `none` |
| `00000000-0000-0000-0000-000000000002` | `frederic-lecourtois` | Frédéric Lecourtois | Aréopage | `autonomy_augmentation` | `jhn` |
| `00000000-0000-0000-0000-000000000003` | `marie-cornelie-lenglet` | Marie-Cornélie Lenglet | Ophélia | `autonomy_augmentation` | `jhn` |
| `00000000-0000-0000-0000-000000000004` | `marie-louise-robert` | Marie-Louise Robert | Marie-Louise | `posthumous_memorial` | `jhn` |

### 2. Taxonomy & Purpose Enum of Digital Twins
* **`autonomy_augmentation`** : For private individuals / close circles (e.g. Frédéric Lecourtois, Marie-Cornélie Lenglet) seeking cognitive augmentation, memory preservation, and intellectual assistance (e.g. classical humanities: French, Latin, Greek in Ghisonaccia).
* **`public_territorial_actor`** : For public figures, officials, academics, journalists, and civic collectives discovered via the social graph (e.g. `@suvranu`).
* **`hybrid`** : Dual nature (personal autonomy + public presence).
* **`posthumous_memorial`** : Memorial / posthumous twins under family/patrimonial mandate (e.g. Marie-Louise Robert).

### 3. Monotone Alias Registry (`public.instance_aliases`)
* **First-Come, First-Served**: 34 aliases registered with immutable `allocated_at` timestamps.
* **Anti-Usurpation Trigger**: `enforce_instance_alias_monotonicity` prevents retroactivity and silent re-allocation.
* **Key Reservations**:
  * **JHN**: `jhn`, `john`, `jean`, `jean-hugues`, `jhr` (early Twitter/X handle `@jhr` historical anchor), `baron-mariani`, `mariani`, `robert`.
  * **Frédéric Lecourtois**: `frederic-lecourtois`, `areopage`, `aréopage`, `frederic`, `frédéric`, `lecourtois`, `f-lecourtois`.
  * **Marie-Cornélie Lenglet**: `marie-cornelie-lenglet`, `marie-cornelie`, `marie-cornélie`, `cornelie`, `cornélie`, `mc-lenglet`, `lenglet`.
  * **Marie-Louise Robert**: `marie-louise-robert`, `marie-louise`, `marie`, `mary`, `mlr`, `ml-robert`, `marie-robert`.

### 4. Recursive Configuration Inheritance (`@inseme/cop-host`)
* **Cycle-Detected Traversal**: `resolveHostChain(...)` traverses parent hosts up to root JHN (`...001`).
* **Non-Inheritable Keys**: Identity keys (`bot_name`, `community_name`, `app_url`, `twin_root_ref`, etc.) never leak to child instances.
* **Shared Technical Capacity**: AI models (`openai_model`), database settings, and tool endpoints are inherited automatically from JHN.

---

## 📡 Bootstrap & Ingestion Pipeline (`@suvranu` & Olé Olé)

### 1. The `@suvranu` Social Graph Strategy
* **Seed Account**: `@suvranu` (~5 000 following, ~1 000 followers) is the curated reference account for Corsican public life.
* **TwitTrust Core (`Following ∩ Followers`)**: The intersection represents the high-signal mutual trust community in Corsica.
* **Access Strategy**: Lean approach via official X account data archive (requested on 2026-08-28, ETA ~24h).
* **Tooling Ready**:
  ```powershell
  node apps/platform/scripts/bootstrap-suvranu-twins.js --archive <path_to_zip_or_folder> --discover
  node apps/platform/scripts/bootstrap-suvranu-twins.js --provision <handle>
  ```

### 2. Impact on the Olé Olé Platform (`oleole.acorsica.org`)
* **Météo du Débat Public**: Ingested tweets from accounts followed by `@suvranu` populate `public_traces` and `derived_claims`, driving the territorial heat map on `public.oleole_places` (Corte, Bastia, Ajaccio, Ghisonaccia, etc.).
* **Acquisition Funnel**: Public actors discovered can later claim their pre-existing Provisional Twin on Olé Olé.

---

## 💻 Zero-Local-State Machine & Agent Resumption Instructions

### 🌐 GitHub Repositories (Branch `main`)
* **Platform Inseme**: [`https://github.com/JeanHuguesRobert/inseme`](https://github.com/JeanHuguesRobert/inseme) (Latest commit `63cd284`)
* **Root Sovereign JHN**: [`https://github.com/JeanHuguesRobert/JeanHuguesRobert`](https://github.com/JeanHuguesRobert/JeanHuguesRobert)
* **Pertitellu / Corte**: [`https://github.com/JeanHuguesRobert/pertitellu`](https://github.com/JeanHuguesRobert/pertitellu)
* **Cogentia**: [`https://github.com/JeanHuguesRobert/cogentia`](https://github.com/JeanHuguesRobert/cogentia)

### 🎯 Single-Phrase Resumption Trigger:
> **`Continue Inseme Issue #57 — Ingest Suvranu Twitter Archive`**  
> *(ou : "Poursuis l'issue 57 d'Inseme et ingère l'archive Suvranu")*
