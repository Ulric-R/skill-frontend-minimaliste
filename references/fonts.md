# Catalogue de polices AI-less

Polices open source ou libres, non conventionnelles — à choisir avant tout
retour vers Inter/Roboto/system-ui. Consulter ce fichier avant de fixer
l'identité visuelle.

## Paires recommandées (display + texte)

| Display (titres) | Texte (corps) | Ton |
| --- | --- | --- |
| **Fraunces** (serif variable, soft) | **Public Sans** ou **Instrument Sans** | Éditorial chaleureux |
| **Space Grotesk** | **Familjen Grotesk** ou **Schibsted Grotesk** | Tech sobre, scandinave |
| **Instrument Serif** (italique expressif) | **Inter Tight** (justifié) | Magazine, contraste fort |
| **Bricolage Grotesque** (variable, largeur) | **Source Sans 3** | Moderne, légèrement atypique |
| **Clash Display** / **General Sans** (Fontshare) | **Satoshi** (Fontshare) | Produit SaaS propre mais original |
| **Geist Sans** + **Geist Mono** | idem | Interface dense, mono pour le code |
| **Syne** (grotesque originale) | **Manrope** | Marque, caractère affirmé |
| **Newsreader** (serif lecture) | **Newsreader** | Blog, long format |
| **JetBrains Mono** / **IBM Plex Mono** | — | Données, tableaux, code |

## Par catégorie

### Grotesques originales
Space Grotesk, Familjen Grotesk, Schibsted Grotesk, Geist, Bricolage
Grotesque, General Sans, Satoshi, Switzer, Hanken Grotesk.

### Serif éditoriales
Fraunces, Instrument Serif, Newsreader, Lora, Literata, Source Serif 4,
Spectral, EB Garamond (classique mais rare en UI).

### Mono / technique
Geist Mono, JetBrains Mono, IBM Plex Mono, Fira Code, Space Mono,
DM Mono, Martian Mono.

### Condensées / affichage à fort caractère
Syne, Clash Display, Archivo Expanded, Anton, Bebas Neue (usage unique),
Unbounded.

## Règles d'usage

1. **Deux familles maximum** (display + texte), trois si une mono est utile.
2. Choisir une **famille variable** quand possible (poids 100–900) pour
   éviter de charger plusieurs fichiers.
3. **Échelle unique** : ratio 1.2 (UI dense) ou 1.25 (éditorial).
4. Line-height : 1.1–1.25 titres, 1.5–1.6 texte courant.
5. Limiter les poids chargés : 2 graisses (400 + 600/700) suffisent souvent.
6. `font-display: swap` et sous-ensembles (`unicode-range`) pour la perf.
7. Tester en **petit corps (14–15 px)** avant de valider — certaines polices
   atypiques deviennent illisibles en dessous de 13 px.
8. Vérifier la présence des chiffres (`tnum`) et des accents français
   (é, è, à, ç, œ) — indispensable pour un site en français.

## Sources

- **Google Fonts** : fonts.google.com — le plus large, gratuit, variable
- **Fontshare** : fontshare.com — gratuite, type fonderie moderne
  (Clash Display, General Sans, Satoshi, Switzer)
- **Velvetyne** : velvetyne.fr — fonderie libre française, très
  non conventionnelle
- **The League of Moveable Type** : leagueofmoveabletype.com
- **Vendée / Open Foundry** : openfoundry.fr
- **GitHub** : rechercher `fonts OFL` pour les polices open source récentes

## À éviter par défaut (déjà présentes partout)

Inter, Roboto, Open Sans, Lato, Montserrat, Poppins, system-ui, SF Pro,
Segoe UI, Helvetica/Arial comme identité principale.

> Inter reste acceptable en **fallback** après une vraie police d'identité,
> jamais comme premier choix.
