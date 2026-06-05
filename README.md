<div align="center">

<img src="https://img.shields.io/badge/version-2.0-7dd3fc?style=for-the-badge&logo=github&logoColor=white" />
<img src="https://img.shields.io/badge/status-en%20développement-fbbf24?style=for-the-badge" />
<img src="https://img.shields.io/badge/HTML%20%2B%20CSS%20%2B%20JS-100%25-38bdf8?style=for-the-badge&logo=html5&logoColor=white" />
<img src="https://img.shields.io/badge/Tailwind%20CSS-CDN-06b6d4?style=for-the-badge&logo=tailwindcss&logoColor=white" />

<br /><br />

```
███████╗██╗  ██╗██╗   ██╗      ██████╗  █████╗ ███╗   ███╗███████╗███████╗
██╔════╝██║ ██╔╝╚██╗ ██╔╝     ██╔════╝ ██╔══██╗████╗ ████║██╔════╝██╔════╝
███████╗█████╔╝  ╚████╔╝█████╗██║  ███╗███████║██╔████╔██║█████╗  ███████╗
╚════██║██╔═██╗   ╚██╔╝ ╚════╝██║   ██║██╔══██║██║╚██╔╝██║██╔══╝  ╚════██║
███████║██║  ██╗   ██║        ╚██████╔╝██║  ██║██║ ╚═╝ ██║███████╗███████║
╚══════╝╚═╝  ╚═╝   ╚═╝         ╚═════╝ ╚═╝  ╚═╝╚═╝     ╚═╝╚══════╝╚══════╝
```

### 🌌 *Bibliothèque de jeux en ligne — Joue partout, tout le temps.*

</div>

-----

## ✦ C’est quoi Sky-Games ?

**Sky-Games** est une bibliothèque de jeux web, conçue pour être belle, rapide et entièrement dans le navigateur. Pas d’installation, pas de compte, pas de prise de tête — tu ouvres la page, tu choisis un jeu, tu joues.

Le projet est un **fichier HTML unique** (vanilla JS + Tailwind CSS CDN) avec une identité visuelle gaming immersive : pluie animée en canvas, étoiles clignotantes, modale de fiche détaillée, filtres par genre et recherche en temps réel.

-----

## ✦ Fonctionnalités

|Fonctionnalité               |Description                                                                      |
|-----------------------------|---------------------------------------------------------------------------------|
|🎮 **Catalogue de jeux**      |10 jeux avec fiche détaillée (genre, âge, durée, thèmes, description)            |
|🔍 **Recherche en temps réel**|Filtre par titre, genre ou mot-clé instantanément                                |
|🏷️ **Filtres par genre**      |Vitesse · Aventure · Puzzle · Sport · Course · Combat · Espace · Survie · Gestion|
|🪟 **Modale animée**          |Fiche complète avec bandeau coloré propre à chaque jeu                           |
|🌧️ **Fond animé**             |Pluie canvas + étoiles clignotantes + nuages en mouvement                        |
|📱 **Responsive**             |Grille adaptative de 2 à 5 colonnes selon l’écran                                |
|🎨 **Design gaming**          |Police Orbitron · Glassmorphism · Palette bleu nuit                              |

-----

## ✦ Stack technique

```
┌─────────────────────────────────────────────────────────┐
│                                                         │
│   HTML5          ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓  Structure       │
│   CSS3           ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓  Animations      │
│   JavaScript     ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓  Logique (Vanilla)│
│   Tailwind CSS   ▓▓▓▓▓▓▓▓▓▓▓▓░░░░░░░░  UI (CDN)        │
│   Canvas API     ▓▓▓▓▓▓▓▓▓▓░░░░░░░░░░  Pluie animée    │
│                                                         │
│   Dépendances : 0 npm  ·  0 build  ·  1 fichier        │
└─────────────────────────────────────────────────────────┘
```

- **Polices** : [Orbitron](https://fonts.google.com/specimen/Orbitron) + [Rajdhani](https://fonts.google.com/specimen/Rajdhani) (Google Fonts)
- **Icons** : SVG inline (aucune dépendance externe)
- **Déploiement** : n’importe quel hébergeur statique (GitHub Pages, Vercel, Netlify…)

-----

## ✦ Structure du projet

```
sky-games/
│
├── sky-games-v3.html     ← Tout le projet est ici (HTML + CSS + JS)
└── README.md
```

Le tableau `GAMES` dans le JS contient toutes les données des jeux :

```js
{
    id: 1,
    emoji: "⚡",
    title: "Volt Runner",
    genre: "Vitesse",       // doit correspondre à un bouton de filtre
    ageMin: 7,
    players: "1 joueur",
    duration: "5 – 20 min",
    themes: ["Action", "Arcade", "Réflexes"],
    description: "...",
    playUrl: "https://...", // 🔗 lien du vrai jeu
    color: "from-yellow-600 to-amber-900"
}
```

-----

## ✦ Lancer le projet

```bash
# Cloner le repo
git clone https://github.com/ton-pseudo/sky-games.git

# Ouvrir directement dans le navigateur
open sky-games-v3.html
# ou double-cliquer sur le fichier — c'est tout.
```

> Aucune installation, aucun `npm install`, aucun build. Juste un fichier HTML.

-----

## ✦ Ajouter un jeu

1. Ouvre `sky-games-v3.html`
1. Trouve le tableau `const GAMES = [...]` dans le JS
1. Copie-colle un bloc existant et modifie les champs
1. Assure-toi que le champ `genre` correspond **exactement** à un bouton de filtre
1. Remplace `playUrl: "#"` par le vrai lien du jeu

-----

## ✦ Bilan du projet

### Points forts

- ✅ Design gaming immersif et cohérent (animations, glassmorphism, typographie)
- ✅ Zéro dépendance — un seul fichier, déployable partout
- ✅ Recherche + filtres combinables en temps réel
- ✅ Code très bien commenté, facile à modifier sans connaître le JS
- ✅ Responsive natif, animations fluides

### Axes d’amélioration prévus

- 🔧 Remplir les vrais liens `playUrl` pour rendre les jeux jouables
- 🔧 Ajouter un burger menu sur mobile
- 🔧 Accessibilité clavier (Tab + Entrée sur les cartes)
- 🔧 Images réelles à la place des emojis
- 🔧 Compteur de résultats après filtrage
- 🔧 Pause de l’animation canvas quand l’onglet est en arrière-plan

-----

## ✦ Roadmap

- [ ] Remplir les `playUrl` avec de vrais jeux
- [ ] Burger menu mobile
- [ ] Favicon + meta Open Graph (partage sur réseaux sociaux)
- [ ] Système de favoris (localStorage)
- [ ] Page “À propos” / mentions légales
- [ ] Séparation HTML / CSS / JS (multi-fichiers)
- [ ] Back-end ou fichier JSON externe pour gérer le catalogue

-----

<div align="center">

**Sky-Games** — fait avec ☁️ et beaucoup de ⚡

*`© 2024 Sky-Games — Joue partout, tout le temps.`*

</div>
