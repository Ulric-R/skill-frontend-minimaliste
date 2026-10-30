# Front-end Minimaliste

> Skill OpenCode pour concevoir une interface minimaliste mais optimale, avec une typographie « AI-less » (polices non conventionnelles) — sans les codes visuels génériques générés par l'IA.

**ID** : `frontend-minimaliste` · **Portée** : globale (`~/.config/opencode/skills/`) · **Langue** : FR

## Ce que fait le skill

Il guide le modèle pour produire un front-end sobre et abouti :

- **Typographie d'abord** : catalogue de polices originales consulté avant tout choix, échelle unique (ratio 1.2 ou 1.25)
- **Hiérarchie par le contraste** : taille, graisse, espace — pas de décoration
- **Palette réduite** : 1 accent, neutres cohérents
- **Interdits du look IA** : dégradés violets, glassmorphism, emojis-icônes, héros centré 2 boutons, Inter/Roboto par défaut
- **Accessibilité** : contraste AA, `:focus-visible`, `prefers-reduced-motion`

## Structure

```text
frontend-minimaliste/
├── SKILL.md              # Workflow, règles typo/CSS, interdits, checklist
└── references/
    └── fonts.md          # Catalogue de polices AI-less (paires, catégories, sources)
```

## Déclenchement

- **Automatique** : toute demande de design UI, refonte de page, choix de polices
- **Manuel** : `@frontend-minimaliste` dans un prompt

## Vérification

- [ ] Aucune police par défaut générique choisie sans consulter `references/fonts.md`
- [ ] Aucun élément de la liste d'interdits produit
- [ ] Contraste AA vérifié

## Skills liés

- `frontend-design` et `modern-web-design` (skills internes) pour la production d'UI
- `anti-dream` pour ne rien affirmer sans vérifier
