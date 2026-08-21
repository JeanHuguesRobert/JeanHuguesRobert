---
title: "Instagram pilot kit — Agent JHN"
date: "2026-08-20"
document_role: "operational"
document_kind: "pilot-protocol"
visibility: "public"
language: "fr"
lifecycle_state: "working"
status: "not started — no platform access or publication authority"
related:
  - "../etude_agent_jhn_instagram.md"
  - "../agent_brief.md"
---

# Kit de pilotage Instagram — Agent JHN

Ce dossier prépare un essai organique de quatorze jours. Il ne donne à aucun agent l'accès à Instagram et n'autorise aucune publication, programmation, réponse, interaction, collecte de données ou dépense.

L'humain conserve les trois décisions : sélectionner la source, valider le paquet, puis publier depuis son propre compte. Agent JHN peut seulement préparer un paquet `ctn_ig_*` et inscrire les décisions effectivement prises dans le registre.

## Préconditions humaines, à constater avant J1

- Le compte choisi est public, professionnel si son titulaire le souhaite, et son identité est vérifiée par Jean Hugues Robert.
- Les médias de terrain retenus ont une provenance et une autorisation de publication explicites.
- Aucun boost, publicité, audience, liste de personnes, donnée personnelle ou outil de ciblage n'est activé.
- Le registre [publication-register.md](publication-register.md) est disponible à la revue ; un paquet refusé ou expiré reste visible comme tel.

L'absence d'une précondition ne doit pas être compensée par une hypothèse : le pilote reste `not started`.

## Paquet de proposition obligatoire

Chaque proposition doit tenir dans un fichier Markdown et employer l'identifiant `ctn_ig_YYYYMMDD_nn`.

```markdown
---
packet_id: ctn_ig_YYYYMMDD_nn
status: draft # draft | approved | rejected | published | expired
prepared_by: agent:jhn:john
prepared_at: YYYY-MM-DD
expires_at: YYYY-MM-DD
platform: Instagram
action_scope: draft-only
human_publication_required: true
ai_media_disclosure: none # none | edited-with-ai | generated-with-ai
---

# Titre de travail

## Source fidelity

- Source primaire : lien stable et date de lecture
- Passage / fait contrôlé :
- Statut épistémique : observé | proposition | hypothèse | question ouverte
- Limite ou objection :

## Produit proposé

- Format : carrousel | Reel | Story
- Audience / scène :
- Angle :
- Média réel autorisé requis : oui / non
- Cartes ou script :
- Légende :
- Source publique à l'écran ou dans la légende :

## Risques et contrôle humain

- Donnée personnelle ou droit à l'image : aucun / à vérifier
- Promesse, accusation, information électorale ou juridique : aucun / à vérifier
- Vérification factuelle à refaire à la publication :
- Décision humaine : en attente
```

## Cadence et limite de volume

- Trois propositions au maximum pendant quatorze jours.
- Une publication n'est préparée qu'après validation de sa source ; elle expire après sept jours si elle n'est pas relue.
- Une publication refusée n'est ni reformulée ni soumise à nouveau sans instruction humaine distincte.
- Les commentaires sont seulement signalés et résumés par catégorie ; aucune réponse n'est générée ou envoyée par défaut.

## Revue de clôture

À J14, le registre doit permettre de répondre sans données individuelles :

1. Combien de paquets ont été approuvés, refusés, expirés et publiés ?
2. Quelle correction factuelle ou de ton a été apportée avant publication ?
3. Combien de temps la revue humaine a-t-elle demandé ?
4. Quelles statistiques agrégées la plateforme a-t-elle fournies, sans en déduire l'adhésion ou l'intention politique des personnes ?
5. Le format reste-t-il fidèle au corpus et à DHITL ?

La revue peut décider de continuer, modifier ou arrêter. Elle ne déclenche jamais un accès API ou une automatisation.

## Références

- [Étude de mandat Instagram](../etude_agent_jhn_instagram.md)
- [Agent Brief — red lines et représentation](../agent_brief.md)
- [Registre de publication de campagne existant](https://github.com/JeanHuguesRobert/cogentia/blob/main/research/campaign/2026_senatoriales_memory.md)
