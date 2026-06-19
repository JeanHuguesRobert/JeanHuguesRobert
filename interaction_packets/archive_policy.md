---
title: "Politique d’archivage des interactions"
description: "Disclosure and archival policy for interaction traces — copy forms (YAML/readable/raw), default publicity, disclosure levels D0–D4, redaction rules."
author: "Jean Hugues Noël Robert, baron Mariani"
affiliation: "Institut Mariani — émanation R&D de C.O.R.S.I.C.A., 1 cours Paoli, F-20250 Corte, Corsica"
date: "2026-05-29"
status: "working-note"
license: "CC BY 4.0"
canonical_url: https://github.com/JeanHuguesRobert/JeanHuguesRobert/blob/main/interaction_packets/archive_policy.md
last_stamped_at: 2026-06-01
document_role: "operational"
document_kind: "continuation-packet"
visibility: "public"
lifecycle_state: "working"
classification_source: "cogentia.js"
classification_version: "1"
classification_rule: "continuation-packet"
classification_confidence: "strong"
---

# Politique d’archivage des interactions

## Principe

Les traces concernent une personne, une organisation ou un compte opérationnel.

Elles doivent donc être stockées dans le dépôt attaché à ce sujet, et non uniquement dans le dépôt qui porte la méthode générique.

Dans ce cas :

- `JeanHuguesRobert/cogentia` porte la méthode Interaction Packets ;
- `JeanHuguesRobert/JeanHuguesRobert` porte les traces personnelles publiques de Jean Hugues Robert.

## Copies des interactions

Pour chaque interaction importante, il est utile de conserver plusieurs formes complémentaires.

### 1. Paquet YAML

Le paquet YAML contient les métadonnées structurées :

- date ;
- canal ;
- interlocuteur ;
- sujet ;
- statut ;
- niveau de divulgation ;
- résumé public ;
- correction éventuelle.

### 2. Copie lisible

La copie lisible est destinée aux humains.

Elle reformule ou reproduit l’échange dans un format Markdown clair, avec éventuellement des coupes explicites.

### 3. Copie brute ou quasi brute

La copie brute vise l’auditabilité.

Elle peut contenir les en-têtes principaux du message et le corps de l’échange.

Elle peut être :

- intégrale ;
- partiellement masquée ;
- remplacée par une copie quasi brute lorsque certains éléments doivent être protégés.

## Divulgation par défaut

La règle générale est la publicité par défaut.

Cependant, l’agent personnel doit signaler les cas où une publication intégrale semble risquée ou inappropriée.

Dans ces cas, il doit :

- masquer les éléments sensibles ;
- ou demander confirmation à l’utilisateur ;
- ou proposer un niveau de divulgation plus prudent.

## Éléments à vérifier avant publication

L’agent doit notamment détecter :

- données médicales ;
- informations concernant des personnes vulnérables ;
- informations familiales sensibles ;
- adresses personnelles ;
- numéros de téléphone privés ;
- données bancaires ;
- secrets professionnels ou juridiques ;
- pièces jointes non destinées à publication ;
- informations de sécurité ;
- propos de tiers n’ayant pas vocation publique évidente.

## Niveaux recommandés

- D0 : privé, non publié ;
- D1 : trace interne privée ;
- D2 : métadonnées publiques, contenu non publié ;
- D3 : copie lisible publique avec masquages éventuels ;
- D4 : copie complète publique.

## Structure recommandée

```text
interaction_packets/
  dashboard.md
  mail_trace.md
  archive_policy.md
  packets/
    2026/
      2026-05-04-session_marenostrum.yaml
  readable/
    2026/
      2026-05-04-session_marenostrum.md
  raw/
    2026/
      2026-05-04-session_marenostrum_redacted.eml.md
```

## Mode d’emploi rapide

### 1. Créer ou mettre à jour le registre

Le registre `mail_trace.md` doit rester synthétique.

Il sert à répondre rapidement à la question :

> Quels cas sont actuellement suivis, avec quel statut et quel niveau de divulgation ?

Il ne doit pas devenir le lieu principal du récit détaillé.

### 2. Créer ou mettre à jour le paquet YAML

Le paquet YAML est la source structurée principale.

Il doit contenir :

- l’identifiant du cas ;
- le statut courant ;
- la chronologie principale ;
- les suites éventuelles dans `follow_up` ;
- les documents liés ;
- l’interprétation prudente ;
- les points à surveiller.

### 3. Mettre à jour le tableau de bord

Le tableau de bord `dashboard.md` doit rester lisible par un lecteur humain.

Il peut inclure un résumé narratif, mais il ne doit pas répéter toute la matière du paquet YAML.

### 4. Documenter les règles nouvelles dans cette politique

Lorsqu’un cas révèle une règle réutilisable, la règle doit être documentée ici comme mode d’emploi.

Exemples :

- comment traiter un paquet remplacé ;
- comment documenter une suite post-envoi ;
- quand mettre l’Institut Mariani en copie ;
- comment corriger un oubli de copie sans re-solliciter inutilement les destinataires initiaux.

## Évolution d’un même cas

Un même cas peut évoluer après sa première documentation : réponse tardive, refus explicite, transformation d’une demande initiale en contribution écrite, relance, publication d’un rapport, correction d’une interprétation initiale, etc.

Dans ce cas, il faut éviter deux erreurs symétriques :

- supprimer trop vite la première trace, ce qui efface l’historique réel du dossier ;
- laisser coexister plusieurs paquets actifs portant le même identifiant ou le même cas, ce qui crée une ambiguïté.

La règle recommandée est donc la conservation avec remplacement explicite.

Lorsqu’un paquet initial est dépassé par un paquet consolidé, l’ancien paquet doit être conservé mais marqué comme remplacé :

```yaml
status: "superseded"
statut: "superseded" # optionnel, pour compatibilité avec d’anciens paquets bilingues
superseded_by: "interaction_packets/packets/YYYY/YYYY-MM-DD-nouveau-paquet.yaml"
superseded_reason: >
  Ce paquet documentait l’état initial du cas. Le cas a ensuite évolué après
  un événement nouveau documenté dans le paquet consolidé.
```

Le paquet remplacé conserve sa valeur historique. Le paquet consolidé devient la source à lire pour l’état courant du cas.

Le tableau de bord (`dashboard.md`) et le registre principal (`mail_trace.md`) doivent pointer vers le paquet consolidé, non vers le paquet remplacé.

### Cas où une fusion peut être préférable

La fusion avec suppression de l’ancien paquet ne doit être envisagée que si :

- l’ancien paquet contient une erreur matérielle sans valeur historique ;
- le paquet a été créé par doublon accidentel ;
- aucune lecture future utile ne dépend de la distinction entre état initial et état consolidé ;
- la suppression ne réduit pas la traçabilité du processus.

Dans le doute, conserver et marquer `superseded`.

### Cas type

Lorsqu’une demande initiale évolue selon la séquence :

```text
demande d’audience → refus ou impossibilité procédurale → contribution écrite recevable
```

il est préférable de conserver le paquet de demande initiale comme trace historique, puis de créer ou mettre à jour un paquet consolidé documentant la séquence complète.

Le statut courant doit alors refléter l’état institutionnel réel, par exemple :

```yaml
statut: "contribution transmise"
current_status:
  label: "Contribution transmise"
```

## Continuations post-envoi

Une interaction principale ne s’arrête pas nécessairement au premier envoi, à la première réponse ou à la transmission du document attendu.

Lorsqu’un événement ultérieur reste attaché au même cas sans ouvrir une interaction autonome, il doit d’abord être ajouté au paquet consolidé dans une section `follow_up`.

Exemples de continuations post-envoi :

- information d’élus, d’acteurs territoriaux ou de parties concernées ;
- copie corrective à une structure de rattachement ;
- transmission pour archive ;
- annonce publique documentant une démarche déjà réalisée ;
- relance sobre fondée sur un événement nouveau ;
- vérification ultérieure d’un accusé de réception, d’un rapport ou d’une mention.

Un nouveau paquet ne doit être créé que si le nouvel échange ouvre un cas autonome : nouvel interlocuteur principal, nouvel objet, nouveau résultat attendu ou nouvelle temporalité de suivi.

Exemple de structure :

```yaml
follow_up:
  - date: "YYYY-MM-DD"
    time: "HH:MM"
    direction: "outbound"
    channel: "email"
    event: "Information des parties concernées"
    summary: >
      Information transmise à des acteurs concernés au sujet d'une interaction
      principale déjà documentée.
    status: "sent"
```

### Critère pratique

Avant de créer un nouveau paquet, poser la question :

> Le nouvel événement change-t-il l’objet du suivi, ou prolonge-t-il simplement le même dossier ?

Si le nouvel événement prolonge le même dossier, utiliser `follow_up`.

Si le nouvel événement crée une demande distincte, un nouvel interlocuteur principal ou une temporalité autonome, créer un nouveau paquet.

## Règle personnelle — Institut Mariani

Lorsque l’interaction relève des travaux associatifs, citoyens, doctrinaux, territoriaux ou patrimoniaux portés dans le cadre de C.O.R.S.I.C.A. ou de l’Institut Mariani, l’Institut Mariani doit être mis en copie lorsque c’est pertinent.

Cette règle ne doit pas conduire à multiplier les destinataires sans nécessité. Elle sert à préserver la traçabilité des actes rattachés à l’écosystème associatif et intellectuel concerné.

### Quand mettre l’Institut Mariani en copie

Mettre l’Institut Mariani en copie lorsque l’échange concerne notamment :

- C.O.R.S.I.C.A. ;
- l’Institut Mariani ;
- l’Autonomie de Capacité ;
- Barons Mariani ;
- Cogentia ;
- #1755 ;
- FractaVolta ;
- un dossier institutionnel, public ou documentaire relevant de l’écosystème.

### Quand ne pas le faire automatiquement

Ne pas mettre l’Institut Mariani en copie si cela risque :

- d’exposer inutilement une personne privée ;
- de créer une confusion juridique ;
- d’alourdir un échange sensible ;
- de rendre institutionnel un échange qui doit rester strictement personnel ;
- de produire un effet de pression disproportionné sur le destinataire.

### Correction d’un oubli

Si l’oubli est détecté après envoi, il doit être corrigé par un message d’archive sobre, adressé à l’Institut Mariani, sans solliciter inutilement à nouveau les destinataires institutionnels.

Cette correction doit être tracée comme `follow_up` du paquet consolidé, sauf si elle ouvre elle-même un nouveau cas autonome.

Exemple :

```yaml
follow_up:
  - date: "YYYY-MM-DD"
    time: "HH:MM"
    direction: "outbound"
    channel: "email"
    event: "Archive corrective Institut Mariani"
    summary: >
      Message adressé à l'Institut Mariani pour archive et traçabilité,
      corrigeant l'absence de copie lors d'un message précédent.
    status: "sent"
```

## Checklist avant archivage

Avant de finaliser une interaction importante, vérifier :

- le statut courant dans `mail_trace.md` ;
- le lien du tableau de bord vers le paquet actif ;
- l’absence de paquet concurrent resté actif par erreur ;
- la présence de `superseded_by` si un paquet initial a été remplacé ;
- le niveau de divulgation ;
- les coupes ou masquages nécessaires ;
- les suites post-envoi à placer dans `follow_up` ;
- la mise en copie de l’Institut Mariani lorsque pertinent ;
- les points à surveiller dans `next_watch`.

## Règle importante

Une copie masquée doit l’indiquer clairement.

Exemples :

- `[adresse masquée]`
- `[numéro masqué]`
- `[passage supprimé : données personnelles]`
- `[pièce jointe non publiée]`

La transparence exige aussi la traçabilité des coupes.
<!-- BEGIN_AUTO: backlinks -->
### Backlinks

*These documents link to this file:*
- [Interaction Packets — Tableau de bord (JHR)](dashboard.md)
- [Research Index — Jean Hugues Noël Robert (Profile / Entry Point)](../research/index.md)
<!-- END_AUTO: backlinks -->
