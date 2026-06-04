# 🏥 EHPAD Finder — Moteur de Recherche & Simulateur National

Une application web moderne, fluide et **entièrement autonome (Client-Side)** permettant aux familles de trouver un établissement médicalisé (EHPAD) adapté à leurs besoins, leurs critères médicaux et leur budget.

Ce projet exploite les données ouvertes de l'État français pour centraliser les tarifs et les prestations de plus de 7 000 structures.

## ✨ Fonctionnalités

*   🔍 **Moteur de recherche ciblé :** Filtrage par Région, Département, budget mensuel maximum et spécificités (Unités Alzheimer, habilitation Aide Sociale (ASH), conventionné APL).
*   🌐 **Architecture Hybride (API / Fallback) :** L'application interroge en temps réel l'API officielle `data.gouv.fr` (CNSA). En cas d'indisponibilité ou de hors-échantillon, un système intelligent bascule instantanément sur un jeu de données locales embarquées.
*   🗺️ **Cartographie Interactive :** Visualisation géographique des établissements correspondants via **Leaflet.js** (sans clé API requise, alternative éco-responsable à Google Maps).
*   🧮 **Simulateur de Reste à Charge :** Calculateur financier interactif qui estime l'effort mensuel net après déduction des revenus, de l'APA (GIR 1-4) et des allocations logement.
*   ✉️ **Formulaire de Contact Réactif :** Interface de dépôt de dossier avec validation des données et confirmation dynamique (UX soignée).

## 🛠️ Stack Technique

*   **Frontend :** HTML5 pur / CSS3 (Design moderne et épuré avec variables CSS, layout Grid et Flexbox).
*   **Logic / Async :** JavaScript Vanilla (ES6+), Fetch API, manipulation dynamique du DOM.
*   **Cartographie :** Leaflet.js & CartoDB Tiles (OpenStreetMap).
*   **Données :** API Tabular de la CNSA (`data.gouv.fr`).

## 🚀 Installation & Déploiement

Le projet est **zéro-configuration** et n'a besoin d'aucun serveur de base de données ni de runtime (Node, PHP, etc.).

1. Clonez le dépôt :
```bash
   git clone [https://github.com/VOTRE_PSEUDO/ehpad-finder.git](https://github.com/VOTRE_PSEUDO/ehpad-finder.git)
