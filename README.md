# Gitlo

**Un client Git de bureau rapide, pilotable au clavier**, pour Windows, macOS et Linux.
Historique en graphe, staging ligne par ligne, résolution de conflits, rebase interactif, pull requests GitHub et merge requests GitLab.

Gitlo s'appuie sur votre installation de `git` : votre configuration, vos hooks, SSH, GPG et vos identifiants fonctionnent tels quels.

---

## Télécharger

➡️ **[Dernière version](https://github.com/IMAMx39/gitlo-releases/releases/latest)**

| Système | Fichier |
|---|---|
| Windows 10 / 11 (64 bits) | `Gitlo-Setup-x.y.z.exe` |
| macOS | `Gitlo-x.y.z.dmg` |
| Linux (x64) | `Gitlo-x.y.z-linux-x64.tar.gz` |

**Prérequis :** [Git](https://git-scm.com/downloads) installé et disponible dans le `PATH` (`git --version` doit répondre dans un terminal).

---

## Installer

### Windows
1. Lancez `Gitlo-Setup-x.y.z.exe`. L'installation se fait dans votre dossier utilisateur et **ne demande pas de droits administrateur**.
2. L'installeur n'est pas encore signé, donc Windows SmartScreen peut afficher « Windows a protégé votre ordinateur ». Cliquez **Informations complémentaires**, puis **Exécuter quand même**.

Pour désinstaller : *Paramètres › Applications › Gitlo › Désinstaller*.

### macOS
1. Ouvrez le `.dmg` et glissez **Gitlo** dans **Applications**.
2. L'application n'est pas encore signée. Au premier lancement, faites **clic droit sur Gitlo › Ouvrir**, puis confirmez.

### Linux
```bash
mkdir -p ~/.local/opt/gitlo
tar -xzf Gitlo-x.y.z-linux-x64.tar.gz -C ~/.local/opt/gitlo
~/.local/opt/gitlo/gitlow
```
Dépendances : GTK 3 et `libsecret` (stockage sécurisé des jetons). Par exemple, sous Debian ou Ubuntu : `sudo apt install libgtk-3-0 libsecret-1-0`.

---

## Mises à jour

Gitlo vérifie les nouvelles versions au démarrage.
- **Windows :** un bandeau propose **Installer et redémarrer**. La mise à jour se télécharge et s'installe en un clic.
- **macOS / Linux :** le bandeau propose de télécharger la nouvelle version.

Après une mise à jour, la fenêtre **« Quoi de neuf »** présente les nouveautés.
Vous pouvez désactiver la vérification dans *Paramètres › Mises à jour*.

---

## Fonctionnalités

- **Historique** : graphe des branches, recherche (message, auteur, contenu), historique d'un fichier, blame, reflog
- **Modifications** : staging et discard par fichier, par hunk ou par ligne ; diff unifié ou côte à côte ; diff d'images
- **Branches** : checkout, création, glisser-déposer pour merger, rebaser ou pousser ; stash ; tags
- **Opérations avancées** : merge avec résolution de conflits en 3 panneaux, rebase interactif, cherry-pick, revert, reset, bisect guidé
- **Annuler / refaire** (Ctrl+Z / Ctrl+Maj+Z) : commit, checkout, merge, rebase, reset…
- **Réseau** : fetch, pull, push avec progression et annulation, fetch automatique, clonage
- **GitHub et GitLab** : pull / merge requests (liste, création, extraction), statut CI, issues liées aux branches, clonage depuis votre compte, avatars
- **Clavier** : palette de commandes (Ctrl+Maj+P) et raccourcis pour tout
- **Gros dépôts et partages réseau** : historique en streaming, index commit-graph proposé, dépôts sur SMB pris en charge

---

## Signaler un problème

Dans Gitlo : *Paramètres › Diagnostic › **Copier le rapport de diagnostic***.
Le rapport contient les versions et la fin du journal d'erreurs ; identifiants et jetons y sont masqués.
Collez-le dans une [nouvelle issue](https://github.com/IMAMx39/gitlo-releases/issues/new) avec une description du problème.
