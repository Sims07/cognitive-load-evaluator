# 🧠 Team Topologies - Calculateur & Audit de Charge Cognitive

> **Outil d'évaluation organisationnelle et d'architecture SI basé sur la Théorie de la Charge Cognitive (John Sweller, 1988) et l'approche Team Topologies (Matthew Skelton & Manuel Pais, 2019).**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.x-38B2AC?logo=tailwind-css)](https://tailwindcss.com/)
[![React](https://img.shields.io/badge/React-18.x-61DAFB?logo=react)](https://reactjs.org/)
[![No Build Required](https://img.shields.io/badge/Build-Single--File_HTML-brightgreen)](#-démarrage-rapide)

---

## 📌 Présentation

Dans les architectures logicielles modernes, la capacité d'innovation et de livraison d'une équipe n'est pas limitée par le nombre d'heures de travail, mais par sa **Capacité Cognitive Maximale**. 

Ce projet fournit à la fois :
1. **Un calculateur interactif (Web App)** permettant de mesurer la charge mentale d'une équipe (*Stream-Aligned*), d'identifier les violations d'heuristiques d'architecture et de générer un rapport d'audit en Markdown.
2. **Un guide théorique et métrologique complet** expliquant la validité scientifique du modèle et le détail des formules de calcul.

---

## ✨ Fonctionnalités Principales

* 🧮 **Calculateur Dynamique de Charge Cognitive :**
  * **Charge Extrinsèque (Bruit & Ops) :** Absence de Platform Team, autonomie CI/CD, dépendances synchrones inter-équipes, dette technique.
  * **Charge Intrinsèque (Séniorité & Cadre) :** Expérience de l'équipe, taux de turnover et limites anthropologiques (**Nombre de Dunbar**).
  * **Charge Essentielle / Germane (Valeur Métier) :** Évaluation DDD (*Domain-Driven Design*) des domaines Simples, Compliqués et Complexes.
* 🚨 **Audit automatique des 5 Heuristiques Team Topologies :** Détection des goulots d'étranglement, surcharges contextuelles et non-respect des règles de domaine.
* 💡 **Recommandations d'Architecture :** Suggestions d'actions correctives ciblées (création de *Platform Team*, extraction de *Complicated Subsystem*, etc.).
* 📄 **Exportation Markdown 1-Click :** Génération d'un rapport structuré prêt à copier dans vos ADR (*Architecture Decision Records*), Confluence ou issues GitHub.
* 🌓 **Interface Sombre / Claire :** Toggle de thème dynamique avec adaptation responsive moderne (Tailwind CSS).
* ⚡ **Zero Setup / Single-File :** Fonctionne directement dans n'importe quel navigateur web, sans étape de build ou d'installation Node.js/npm.

---

## 🧮 Modèle Mathématique & Formule

Le modèle évalue la charge sur une échelle ordinale de **100 points** :

$$ \text{Charge Cognitive Totale} = \text{Charge Extrinsèque} + \text{Charge Intrinsèque} + \text{Charge Essentielle (Germane)} $$

```
┌────────────────────────────────────────────────────────────────────────┐
│                        CAPACITÉ COGNITIVE MAXIMALE (100 pts)           │
├───────────────────┬────────────────────┬───────────────────────────────┤
│  EXTRINSÈQUE      │    INTRINSÈQUE     │    ESSENTIELLE (GERMANE)      │
│  (Bruit, Ops)     │    (Stack, Taille) │    (Périmètre Métier usager)  │
│                   │                    │                               │
│  ⚠️ À MINIMISER    │  📉 À OPTIMISER    │  🎯 À MAXIMISER / PROTÉGER     │
└───────────────────┴────────────────────┴───────────────────────────────┘
```

* **Indicateur de Santé :**
  * 🟢 **< 65% :** Équipe Saine (Marge d'innovation et d'apprentissage conservée).
  * 🟠 **65% - 84% :** Tension Modérée (Risque de ralentissement sur les livraisons).
  * 🔴 **$\ge$ 85% :** Surcharge Critique / Violations (Risque élevé de burnout et dette technique).

---

## 🚀 Démarrage Rapide

### Option 1 : Utilisation directe locale
1. Clonez ce dépôt :
   ```bash
   git clone https://github.com/votre-utilisateur/team-topologies-cognitive-load.git
   cd team-topologies-cognitive-load
   ```
2. Ouvrez simplement le fichier `team_topologies_explorer.html` dans votre navigateur web (Chrome, Firefox, Edge, Safari).

### Option 2 : Hébergement via GitHub Pages
1. Rendez-vous dans les **Settings** de votre dépôt GitHub.
2. Allez dans la section **Pages**.
3. Sélectionnez la branche `main` et le dossier `/ (root)` comme source.
4. Votre application sera instantanément accessible en ligne !

---

## 📁 Structure du Projet

```
.
├── README.md                                       # Documentation générale du dépôt
├── team_topologies_explorer.html                   # Application web interactive (Single-file HTML + React + Tailwind)
└── Team_Topologies_Regles_Calcul_Charge_Cognitive.md # Guide métier, règles de calcul & validité scientifique
```

---

## 📚 Références & Fondements Théoriques

* **John Sweller (1988)** – *Cognitive Load Theory during Learning* (Psychologie Cognitive).
* **Matthew Skelton & Manuel Pais (2019)** – *Team Topologies: Organizing Business and Technology Teams for Fast Flow* (IT Revolution).
* **Robin Dunbar (1992)** – *Neocortex size as a constraint on group size in primates* (Limites anthropologiques de communication).

---

## 📄 Licence

Ce projet est sous licence MIT - voir le fichier [LICENSE](LICENSE) pour plus de détails.