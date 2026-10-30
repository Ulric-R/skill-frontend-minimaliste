---
name: Front-end Minimaliste
description: Concevoir une interface minimaliste mais optimale, avec une typographie non conventionnelle (AI-less) — polices originales, hiérarchie par le contraste, palette réduite, et évitation des codes visuels génériques générés par IA. À utiliser pour toute demande de design UI, refonte de page, choix de polices ou de style visuel.
---

# Front-end minimaliste (AI-less)

Objectif : une interface sobre mais aboutie, qui ne ressemble pas à une sortie
générique d'IA. La typographie porte le style ; la structure porte l'usage.

## Workflow

1. **Lire `references/fonts.md`** avant de choisir toute police. Ne jamais
   sélectionner une police par défaut sans consulter le catalogue.
2. **Poser l'échelle typographique** : un ratio unique (1.2 ou 1.25), une
   famille display + une famille texte, une graisse variable éventuelle.
3. **Construire la hiérarchie par le contraste** : taille, graisse, espace et
   couleur — jamais par la décoration (ombres portées, bordures lourdes,
   fonds colorés).
4. **Limiter la palette** : une seule couleur d'accent, des neutres avec une
   température cohérente, un fond non pur de préférence (#FAFAF8 plutôt que
   #FFFFFF).
5. **Appliquer les interdits du look IA** (voir ci-dessous).
6. **Vérifier en fin de parcours** : cohérence de l'échelle, densité, accessibilité.

## Règles typographiques

- Ratio d'échelle unique : **1.2 (mineure tierce)** pour l'UI dense,
  **1.25 (grande seconde)** pour l'éditorial.
- Line-height : 1.5–1.6 pour le texte courant, 1.1–1.25 pour les titres.
- Largeur de colonne de lecture : 60–75 caractères.
- Espacer les titres par le haut (`margin-top` négatif ou `padding` généreux)
  plutôt que par des séparateurs.
- Utiliser `font-feature-settings` quand la police le permet
  (`"tnum"` pour les chiffres, `"ss01"` pour les variantes stylistiques).

## Grille et espacement

- Espacements en multiples d'une base unique (4 px ou 8 px) — aucune valeur
  au hasard.
- Une seule source de vérité pour les variables CSS (`--space-*`, `--text-*`).
- Alignement sur une grille implicite ; marges latérales généreuses,
  jamais de contenu collé au bord.

## Interdits (look IA générique)

Ne jamais produire :

- Dégradés violet/bleu ou « AI gradient » en fond
- Glassmorphism / `backdrop-filter` décoratif
- Émojis utilisés comme icônes
- Héros centré avec un titre, un sous-titre et deux boutons
- Cartes arrondies identiques avec ombre douce et icône emoji
- Polices par défaut : Inter, Roboto, system-ui, SF sans justification
- Boutons pilules excessivement arrondis (`border-radius: 9999px`) partout
- Trois colonnes de « features » équidistantes sans hiérarchie

## Accessibilité et finition

- Contraste texte/fond minimum **AA (4.5:1)** ; vérifier les états de focus
  visibles (`:focus-visible`).
- Respecter `prefers-reduced-motion` pour toute animation.
- Densité assumée : une UI minimaliste n'est pas une UI vide. Garder les
  informations utiles, supprimer le bruit.
- Responsive : l'échelle typographique peut être fluide
  (`clamp()`), les marges latérales croissent avec le viewport.

## Vérification finale

- [ ] Une seule échelle typographique respectée partout
- [ ] Aucune police par défaut générique
- [ ] Palette : 1 accent + neutres cohérents
- [ ] Aucun élément de la liste d'interdits
- [ ] Contraste AA et focus visibles
