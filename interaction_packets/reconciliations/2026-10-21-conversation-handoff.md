# Passation — consolidation des interactions, 21 octobre 2026

L'audit ciblé est clos ; reprendre les travaux restants par leurs sources, sans répéter la passe Gmail.

- [Inventaire de couverture](2026-10-21-coverage-public.md) : 50/51 rapprochements publics, A Fucina/WhatsApp non vérifié.
- [Audit transversal et critère d'arrêt](2026-10-21-cross-projection-audit.md) : corrections de liens et vérification bornée des projections ; complétude des pièces non établie.
- [Interactions candidates hors registre](2026-10-21-unregistered-candidates.md) : Dieta 1755 et Musée de la Corse à qualifier, sans fusion ni inscription automatique.
- [Patterns observés](2026-10-21-pattern-observations.md) : garder faits, incertitudes, canaux et contre-exemples.
- [Cognitive Packet Cogentia #271](https://github.com/JeanHuguesRobert/cogentia/issues/271) : amélioration future du Sleep Cycle, toujours différée et sans mutation automatique.

Périmètres non clos : sources privées sous autorisation distincte, réception/intégrité des fichiers transmis par plateformes externes, canal WhatsApp et découverte d'autres interactions non enregistrées. Réouvrir seulement en présence de preuve, anomalie reproductible ou mandat ciblé.

## Règle opérationnelle de publication — optimistic locking

Pour une écriture GitHub explicitement mandatée et normalement autorisée : (1) lire la cible et son SHA courant, (2) produire un patch minimal et conserver la provenance, (3) écrire avec ce SHA comme précondition, (4) relire pour vérifier le résultat. En cas de conflit de version, rafraîchir puis réconcilier les différences avant une nouvelle tentative ; ne jamais écraser à l'aveugle. En cas de refus de sécurité ou de permission, enregistrer l'échec comme tel, sans le déguiser en conflit de version ni chercher à neutraliser les protections. L'existence de contrôles préventifs ne dispense pas de tenter les écritures ordinaires que le mandat et les permissions rendent légitimes.
