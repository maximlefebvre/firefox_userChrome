# Firefox userChrome

Un thème simple pour Firefox, en clair et en sombre, fait de deux feuilles de style :

- **`userChrome.css`** pour l'interface : onglets, barre d'adresse, menus,
  panneau des téléchargements, fenêtre Bibliothèque. C'est le thème lui-même.
- **`userContent.css`** (facultatif) pour les pages internes de Firefox :
  paramètres, nouvel onglet, extensions, `about:config`… Il n'a aucun effet
  sur les sites web.

Ce que fait le thème :

- Fond neutre, onglets en pilule, barre d'adresse centrée
- Barre d'outils et page réunies dans une carte arrondie
- Plus de violet : accents en noir, blanc et gris
- Bascule automatiquement entre clair et sombre selon macOS
- Fenêtre Bibliothèque, panneau des téléchargements et paramètres assortis

## Captures d'écran

### Clair

![Qwant en clair](screenshots/light-qwant.webp)
![Archcraft en clair](screenshots/light-archcraft.webp)
![Bibliothèque en clair](screenshots/light-bibliotheque.webp)
![Paramètres en clair](screenshots/light-parametres.webp)

### Sombre

![Qwant en sombre](screenshots/dark-qwant.webp)
![Archcraft en sombre](screenshots/dark-archcraft.webp)
![Bibliothèque en sombre](screenshots/dark-bibliotheque.webp)
![Paramètres en sombre](screenshots/dark-parametres.webp)

## Installation

1. **Activer les CSS personnalisés.** Ouvrir `about:config` et passer
   `toolkit.legacyUserProfileCustomizations.stylesheets` à `true`.
2. **Trouver le dossier du profil.** Ouvrir `about:support` et cliquer sur
   **Dossier de profil → Ouvrir le dossier**. Y créer un dossier `chrome`
   s'il n'existe pas.
3. **Copier les fichiers** dans ce dossier `chrome` :
   - `userChrome.css` pour le thème de l'interface ;
   - `userContent.css` si l'on veut aussi les pages internes de Firefox
     assorties (sans lui, elles gardent les couleurs d'origine de Firefox,
     violet compris).
4. **Passer le thème sur Système.** Dans `about:addons` → **Thèmes**, activer
   **« Système — automatique »**. C'est ce réglage qui permet au thème de suivre
   automatiquement le mode clair ou sombre de macOS.
5. **Redémarrer Firefox.**

Pour que les pages internes (et les sites qui le gèrent) suivent aussi le mode
de macOS : **Paramètres → Général → Apparence des sites web → Automatique**.

## Personnalisation

Les couleurs, l'arrondi et les marges se règlent avec les variables en haut
des fichiers (`--cx-bg`, `--cx-surface`, `--cx-radius`, `--cx-gap`…).
Les deux fichiers utilisent la même palette : penser à modifier les deux.

## Compatibilité

Testé uniquement sur **macOS 27.2.1** avec **Firefox Developer Edition 161.0**.

Le rendu sur Windows et Linux n'a pas été vérifié. Le thème s'appuie sur des
noms internes de Firefox, qui peuvent changer d'une version à l'autre.
