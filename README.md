# Hermes Client — versions

Application de bureau (macOS / Windows) pour discuter avec l'agent Hermes hébergé sur son propre serveur.

Ce dépôt ne contient **que les versions compilées** : installateurs et fichier `latest.json` lu par la mise à jour intégrée. Le code source est privé.

## Télécharger

Ouvrir la [dernière version](https://github.com/sluve/hermes-releases/releases/latest) et prendre le fichier correspondant :

| Système | Fichier |
|---|---|
| Windows | `Hermes.Client_X.Y.Z_x64-setup.exe` (ou `.msi`) |
| macOS (Apple Silicon et Intel) | `Hermes.Client_X.Y.Z_universal.dmg` |

## Première installation

L'application n'est pas encore signée par Apple ni par Microsoft ; le système affiche donc un avertissement la première fois.

- **Windows** — « Windows a protégé votre ordinateur » : cliquer sur *Informations complémentaires* puis *Exécuter quand même*.
- **macOS** — ouvrir le `.dmg`, glisser Hermes Client dans *Applications*. Au premier lancement : clic droit sur l'app → *Ouvrir* → *Ouvrir*. Si macOS indique que l'app est « endommagée », lancer dans le Terminal :
  `xattr -cr "/Applications/Hermes Client.app"`

## Mises à jour

Une fois installée, l'application vérifie seule les nouvelles versions au démarrage. Le bouton **Mises à jour**, en bas de la barre latérale, permet aussi de vérifier et d'installer.

Chaque mise à jour est **signée** : l'application refuse d'installer une version qui ne porte pas la signature du projet.

## Fichiers d'une version

- Installateurs (`.exe`, `.msi`, `.dmg`) — pour une installation manuelle.
- `.sig`, `.nsis.zip`, `.app.tar.gz` — utilisés par la mise à jour intégrée, inutile de les télécharger.
- `latest.json` — décrit la dernière version pour la mise à jour intégrée.
