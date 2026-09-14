# Thème Samsung Galaxy — Guide de finalisation

Ce dossier contient les visuels de base (dégradé bleu Samsung, motif hexagone Galaxy) :

- `wallpaper-home.svg` — fond d'écran écran d'accueil (1440×3120)
- `wallpaper-lock.svg` — fond d'écran écran verrouillé (1440×3120)
- `icon-template.svg` — gabarit d'icône d'application (512×512)

Je ne peux pas produire le fichier `.st` final (format propriétaire signé par
Samsung) ni le publier sur le Galaxy Themes Store — ces étapes se font avec
les outils officiels Samsung, sous ton compte. Voici comment continuer.

## 1. Exporter les visuels en PNG

Les fichiers sont en SVG (vectoriel, modifiable). Ouvre-les avec un logiciel
gratuit (Inkscape, Figma, ou un convertisseur SVG→PNG en ligne) et exporte :

- `wallpaper-home.png` — 1440×3120 px
- `wallpaper-lock.png` — 1440×3120 px
- Icônes d'app — 512×512 px chacune (dupliquer `icon-template.svg`, changer
  le glyphe dans `<g id="app-glyph">`, puis exporter)

## 2. Télécharger Samsung Theme Studio

- Site officiel : https://developer.samsung.com/themes (compte Samsung
  développeur requis, gratuit)
- Outil disponible pour Windows

## 3. Monter le thème dans Theme Studio

1. Nouveau projet → renseigner nom, description, catégorie "Galaxy"
2. Onglet **Wallpaper** → importer `wallpaper-home.png` et `wallpaper-lock.png`
3. Onglet **Icons** → importer les icônes exportées, une par application
   courante (Téléphone, Messages, Appareil photo, Galerie, Chrome...)
4. Onglet **Color/Style** → couleur d'accent `#1428A0` (bleu Samsung) pour
   rester cohérent avec le fond d'écran
5. **Preview** → tester sur l'aperçu intégré avant export

## 4. Publier et fixer le prix

1. Dans Theme Studio : **Export** → génère le fichier `.st`
2. Créer un compte sur le **Samsung Seller Portal**
   (https://seller.samsungapps.com) — vérification d'identité requise pour
   vendre (pas seulement publier gratuitement)
3. Uploader le `.st`, renseigner captures d'écran, description
4. Définir le prix : **0,99 USD**
5. Soumettre pour revue — délai de validation Samsung avant mise en ligne

## Notes

- Le montant réellement perçu par vente sera réduit de la commission
  Samsung (vérifie le taux en vigueur sur le Seller Portal avant de fixer
  ton prix).
- Pour tester le thème sur TON téléphone avant publication, tu peux
  installer le `.st` exporté directement via l'app **Themes** en mode test
  développeur, sans attendre la validation du store.
