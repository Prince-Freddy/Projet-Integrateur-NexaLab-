# NexaLab — Document d'Architecture
### Projet Intégrateur · Bloc 2 · Académie de Programmation IFRI · L1


---

## Table des matières

1. [Présentation du projet](#1-présentation-du-projet)
2. [Structure du dépôt](#2-structure-du-dépôt)
3. [Architecture CSS modulaire](#3-architecture-css-modulaire)
4. [Identité visuelle & choix de design](#4-identité-visuelle--choix-de-design)
5. [Auteurs](#5-auteurs)

---

## 1. Présentation du projet

### Le client

**NexaLab** est un laboratoire d'innovation spécialisé dans les solutions technologiques pour les entreprises africaines. Leur ADN : modernité, rigueur, impact. Leur audience cible réunit directeurs d'entreprise, investisseurs et jeunes talents tech.

### La mission

Concevoir et développer la **page d'accueil complète de NexaLab** depuis zéro, avec :
- une architecture CSS modulaire irréprochable
- un HTML5 sémantique et propre
- un design responsive (mobile, tablette, desktop)
- un rendu visuel professionnel cohérent avec l'identité du client

### Sections livrées

| # | Section | Description |
|---|---------|-------------|
| 01 | **Header & Navigation** | Logo NexaLab + menu sticky + boutons CTA |
| 02 | **Hero** | Accroche forte, sous-titre, call-to-action + visuel dashboard |
| 03 | **À propos** | Mission et vision de NexaLab, layout image/texte |
| 04 | **Services** | IA, Data Science & Analytics, IoT — cartes avec visuels |
| 05 | **Statistiques** | Chiffres clés : 120+ projets, 50+ partenaires, 15+ pays |
| 06 | **Équipe** | Présentation des membres core |
| 07 | **Témoignages** | 3 retours clients mis en page |
| 08 | **Contact** | Formulaire stylisé (nom, email, sujet, message) |
| 09 | **Footer** | Liens, réseaux, copyright |

---

## 2. Structure du dépôt

```
nexalab/
├── index.html               ← Page d'accueil unique
├── styles/
│   ├── base.css             ← Reset, variables CSS, typographie globale
│   ├── header.css           ← Navigation et logo
│   ├── hero.css             ← Section d'accroche principale
│   ├── about.css            ← Section À propos / Mission
│   ├── services.css         ← Cartes services (IA, IoT, Data)
│   ├── stats.css            ← Section chiffres clés
│   ├── team.css             ← Présentation équipe
│   ├── testimonials.css     ← Témoignages clients
│   ├── contact.css          ← Formulaire de contact
│   └── footer.css           ← Pied de page
├── assets/
│   ├── images/              ← Visuels libres de droits (Unsplash/Pexels)
│   └── icons/               ← Icônes SVG personnalisées
└── README.md                ← Ce document
```

**Pourquoi cette structure ?**
Chaque fichier CSS correspond exactement à une section HTML. Cela permet à n'importe quel membre de l'équipe de modifier la section `services` sans risquer de casser le `hero`. C'est le principe de **séparation des responsabilités** appliqué au CSS.

---

## 3. Architecture CSS modulaire

| Fichier CSS | Responsabilité |
|---|---|
| `base.css` | Variables globales, reset, typographie |
| `header.css` | Navigation et logo |
| `hero.css` | Section d'accroche |
| `about.css` | Présentation du labo |
| `services.css` | Cartes de services |
| `stats.css` | Chiffres clés |
| `team.css` | Équipe NexaLab |
| `testimonials.css` | Avis clients |
| `contact.css` | Formulaire de contact |
| `footer.css` | Pied de page |

---

## 4. Identité visuelle & choix de design

**Palette :** fond noir profond `#0d0f1a` + bleu nuit `#131726` + accent or `#c9a84c`. L'association noir/or crée une identité premium et technologique, adaptée à une audience de décideurs africains exigeants.

**Typographie :** `Barlow Condensed` (titres, uppercase, bold) pour l'impact visuel — `Inter` (corps de texte) pour la lisibilité sur fond sombre.

**Mise en page :** Header sticky, Hero deux colonnes (texte + dashboard), Services en grille 3 colonnes, Stats en ligne avec chiffres dorés surdimensionnés. Flexbox comme base principale, Grid en complément pour les cartes.

---

## 5. Auteurs

Projet réalisé dans le cadre du **Bloc 2 — Projet Intégrateur**
Académie de Programmation · IFRI · Parcours L1

| Membre | Fichiers gérés |
|---|---|
| **Leslie** | `hero.css`, `about.css` |
| **Loth** | `services.css`, `stats.css` |
| **Melvine** | `team.css`, `testimonials.css` |
| **Bryan** | `contact.css`, responsive design (media queries dans tous les fichiers) |

---
