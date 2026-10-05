# Politique de sécurité

## Versions prises en charge

Seule la [dernière version](https://github.com/CStonx/download/releases/latest) reçoit des correctifs. Le logiciel propose la mise à jour dans ses Réglages.

## Signaler une faille

Ne publie pas la faille dans un ticket. Envoie-la en privé :

- via **[Report a vulnerability](https://github.com/CStonx/download/security/advisories/new)** sur ce dépôt ;
- ou en message privé sur Discord : **thaskow**.

Indique la version concernée, les étapes pour reproduire et l'impact. Tu reçois une réponse sous quelques jours, et le correctif est publié dans une nouvelle version avant toute communication publique.

## Vérifier un fichier

Les versions officielles sont publiées sur ce dépôt, avec un fichier `SHA256SUMS.txt`, et livrées par la mise à jour intégrée au logiciel depuis le site [cstonx.thaskow.fr](https://cstonx.thaskow.fr). Aucune autre source n'est officielle.

- **Mise à jour intégrée** : le manifeste des versions est signé (ECDSA P-256) et le logiciel vérifie la signature, la taille et l'empreinte SHA-256 du fichier téléchargé. Une version dont la signature n'est pas valide, ou plus ancienne que la version installée, est refusée.
- **Téléchargement manuel** : `SHA256SUMS.txt` n'est pas signé. Il permet de détecter un fichier corrompu, pas de prouver son origine : télécharge uniquement depuis ce dépôt.
- **Signature Windows** : les exécutables ne sont pas encore signés (Authenticode), d'où l'avertissement SmartScreen au premier lancement.
