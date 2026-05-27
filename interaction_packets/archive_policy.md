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

## Règle importante

Une copie masquée doit l’indiquer clairement.

Exemples :

- `[adresse masquée]`
- `[numéro masqué]`
- `[passage supprimé : données personnelles]`
- `[pièce jointe non publiée]`

La transparence exige aussi la traçabilité des coupes.
