# Agent John — Apprentissages & Règles Souveraines de Protection

Ce document consigne les leçons d'ingénierie et règles de sécurité apprises lors de l'exploitation de l'Agent John (Jumeau Numérique Souverain Cogentia).

---

### 1. La Loi de l'Écho Auto-Référentiel (Boucles Auto-Générées)

**Problème constaté :**
En mode *Message à soi-même* (*"Message Yourself"* sur WhatsApp), toute réponse envoyée par l'Agent John est diffusée par le protocole WhatsApp comme un événement entrant (*inbound sync*). Si l'Agent John ne distingue pas de manière déterministe sa propre voix d'un message humain, il répond à son propre écho et génère une boucle infinie.

**Règle de sécurité (Invariance de Réflexion) :**
- L'Agent John **doit impérativement vérifier le filtre d'écho** (`looksLikeAgentJhnOutbound`) sur tout message entrant.
- Les motifs tels que `Reçu`, `Received`, `📱 *Agent JHN`, `📇 *Agent JHN`, `✅ Saved contact`, `📁 Conversation` sont immédiatement classés comme échos et **bloqués avant tout traitement**.

---

### 2. Le Disjoncteur Organique (Rate Limiter & Circuit Breaker)

**Principe :**
L'Intelligence Artificielle ne doit jamais reposer sur une seule ligne de défense. Si une variante d'écho échappe aux filtres, un disjoncteur physique découplé doit stopper le système.

**Seuils de sécurité :**
- Maximum 5 messages sortants par fenêtre glissante de 60 secondes.
- En cas de dépassement, le **Disjoncteur SAUTE (Circuit Breaker Tripped)**.
- Toute émission sortante est verrouillée au niveau de la porte `outbound-gate`.
- Une alarme multi-canal est émise vers le Répertoire d'Urgence.
- Le réarmement s'effectue via la commande de contrôle mobile : `reset rate limit`.

---

### 3. Souveraineté & Traçabilité 24/7/365

- L'Agent John fonctionne en démon autonome sur Fracta VPS.
- Chaque décision (`reject`, `hold_for_human`, `approve`) donne lieu à une empreinte SHA256 anonymisée dans `traces/whatsapp_trace.jsonl`.
