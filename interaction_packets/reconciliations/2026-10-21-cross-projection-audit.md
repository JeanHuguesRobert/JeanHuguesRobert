# Audit transversal des projections et pièces — 21 octobre 2026

## Portée

Après la première passe Gmail (50/51 interactions publiques avec rapprochement ciblé), début du contrôle de cohérence des liens, pièces et interactions candidates. Ce document n'atteste ni examen exhaustif des 51 YAML ni vérification des fichiers transférés par services tiers.

## Correctif confirmé

- Paquet `interaction_packets/packets/2026/2026-09-23-grasse-acces-dossier-marie-louise.yaml` : lien `linked_documents.readable` initialement `../readable/...`, incorrect depuis `packets/2026`. Chemin corrigé en `../../readable/...`. Les deux autres chemins `../../mail_trace.md` et `../../archive_policy.md` sont cohérents. Vérifier d'autres références relatives dans les paquets avant correction en série.

## Candidats et liens de preuve

- Demande **Cismonte du 9 octobre** sur les témoins de la Constitution de 1755 : fil sortant vérifié ; cite explicitement une démarche distincte adressée à **Ajaccio**. La réponse du 14 octobre annonçant une copie de la *Dieta* par WeTransfer doit être rattachée au fil exact et comparée aux pièces réellement reçues.
- Musée de la Corse, information du 13 octobre sur le comité des usagers : documenter l'origine de la participation avant qualification en interaction autonome.
- Ne pas créer automatiquement des lignes du registre pour tout message institutionnel trouvé. Proposer le rattachement, contrôler les doublons et respecter les niveaux de divulgation.

## Contrôles restants

1. Inventorier les paquets YAML, documents lisibles, traces brutes et pièces ; vérifier présence, liens et identifiants croisés, puis réparer chaque anomalie confirmée.
2. Vérifier séparément existence/notification/téléchargement/intégrité des pièces annoncées via France Transfert, TransfertPro et WeTransfer. Une annonce d'envoi ne prouve pas le téléchargement.
3. Comparer dashboard et registre canonique : couverture du tableau de bord, fraîcheur des statuts, événements non projetés ; ne pas supposer que toutes les entrées du registre doivent figurer au dashboard sélectionné.
4. Rechercher systématiquement les interactions **hors registre**, avec contrôle anti-doublon et confidentialité, puis valider leur éventuelle création.
5. Vérifier WhatsApp pour `2026-08-02-001` seulement via un accès effectif au canal original ; ne pas conclure depuis Gmail.

## Pattern / FractaCognition

Deux récurrences de travail à traiter via le Pattern Mining existant, non comme concepts doctrinaux nouveaux : (a) **lien documentaire invalide dans une projection malgré des données correctes** ; (b) **collision sémantique** entre plusieurs demandes portant sur le même sujet mais adressées à des institutions distinctes. Tester la transférabilité et rechercher les contre-exemples avant promotion. Conserver la distinction preuve, inférence, décision.
