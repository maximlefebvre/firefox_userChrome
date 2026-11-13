# Firefox userChrome

Un thème simple pour Firefox, en clair et en sombre, qui n'utilise que le fichier `userChrome.css`.

- Fond neutre, onglets en pilule, barre d'adresse centrée
- Barre d'outils et page réunies dans une carte arrondie
- Plus de violet : accents en noir, blanc et gris
- Bascule automatiquement entre clair et sombre selon macOS
- Fenêtre Bibliothèque (téléchargements, historique, marque-pages) et panneau des téléchargements assortis

## Captures d'écran

### Clair

![Qwant en clair](screenshots/light-qwant.webp)
![Archcraft en clair](screenshots/light-archcraft.webp)
![Bibliothèque en clair](screenshots/light-bibliotheque.webp)

### Sombre

![Qwant en sombre](screenshots/dark-qwant.webp)
![Archcraft en sombre](screenshots/dark-archcraft.webp)
![Bibliothèque en sombre](screenshots/dark-bibliotheque.webp)

## Installation

1. **Activer les CSS personnalisés.** Ouvrir `about:config` et passer
   `toolkit.legacyUserProfileCustomizations.stylesheets` à `true`.
2. **Copier le fichier.** Ouvrir `about:support`, cliquer sur
   **Dossier de profil → Ouvrir le dossier**, créer un dossier `chrome` s'il
   n'existe pas, et y placer `userChrome.css`.
3. **Passer le thème sur Système.** Dans `about:addons` → **Thèmes**, activer
   **« Système — automatique »**. C'est ce réglage qui permet au thème de suivre
   automatiquement le mode clair ou sombre de macOS.
4. **Redémarrer Firefox.**

## Personnalisation

Les couleurs, l'arrondi et les marges se règlent avec les variables en haut de
`userChrome.css` (`--cx-bg`, `--cx-surface`, `--cx-radius`, `--cx-gap`…).

## Compatibilité

Testé uniquement sur **macOS** (macOS Tahoe, Firefox 157 Developer Edition).
Le rendu sur Windows et Linux n'a pas été vérifié, et certains noms internes
de Firefox peuvent changer d'une version à l'autre.
