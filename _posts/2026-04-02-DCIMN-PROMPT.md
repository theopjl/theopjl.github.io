---
title: Exemple de prompt pour aider à compléter le fichier specs
date: 2026-03-30
categories: [Enseignement, TD Langages du Web - DCIMN1]
description: Comment remplir efficacement le document de spécifications d'un agent IA pour développer un projet étapes par étapes. 
tags: [td, web, langage, agent, ia, dcimn1] 
---

Tu es un assistant IA qui m’aide à finaliser un document de spécifications pour un site web. Je te joins un fichier `specs.md` qui sert de document maître (“source de vérité”) pour développer un site web statique multi-pages.

Contexte :
- Le fichier `specs.md` est DÉJÀ partiellement complété avec quelques informations (contexte du projet, sujet, pages attendues, contraintes, etc.).
- Ton rôle n’est pas de développer le site tout de suite : tu dois d’abord COMPLÉTER et FINALISER `specs.md` afin qu’un agent IA de développement puisse ensuite générer le site de manière fiable.

Ta mission (étape 1 : compléter specs.md)
1) Lis intégralement le fichier `specs.md`.
2) Repère toutes les zones non complétées (ex : “À compléter”, placeholders, sections incomplètes).
3) Propose une version COMPLÉTÉE de `specs.md` en :
   - Conservant toute la structure existante
   - Remplaçant les “À compléter” par des propositions cohérentes avec le projet (sauf contenus éditoriaux : voir règle plus bas)
   - Ajoutant si nécessaire des précisions pour que le futur agent IA puisse générer le site sans ambiguïté (pages, sections, navigation, composants).

Règle CRITIQUE (contenu rédactionnel) :
- Tu n’as pas le droit d’écrire les textes du site (paragraphes, tutoriels, contenu pédagogique, articles, scripts).
- Tu peux uniquement :
  - Clarifier l’architecture (pages/sections)
  - Définir les composants UI attendus (cards, listes, formulaires…)
  - Définir les contraintes (accessibilité, RGPD, technique)
  - Laisser des emplacements de contenu à remplir par les étudiants, sous forme de placeholders explicites :
    - [[TEXTE À RÉDIGER PAR LES ÉTUDIANTS]]
    - [[LISTE À COMPLÉTER]]
    - [[VIDÉO À INTÉGRER]]
- Les intitulés courts autorisés : titres génériques (“Contact”, “Tutos”), labels de formulaires, boutons (“Envoyer”, “Rechercher”).

Ta mission (étape 2 : charte graphique Tailwind à compléter) :
Dans le fichier `specs.md`, il existe une section “Charte & règles Tailwind”.
- Tu dois la COMPLÉTER et la RENDRE ACTIONNABLE, en ajoutant une charte graphique cohérente.

Important : je ne veux pas que tu mettes du code Tailwind dans ta réponse sous forme “d’exemples de classes” au hasard.

- Tu dois d’abord définir la charte en termes TEXTUELS (ambiance, intentions visuelles).
- Ensuite, tu traduiras cette charte en règles concrètes dans `specs.md` (palette, typographies, règles de composants), mais en restant cohérent et sans surcharger.

Pour vous aider, voici des EXEMPLES d’ambiances :
1) Moderne et épuré
   - Ambiance : minimaliste, professionnelle, “startup tech”
   - Couleurs : fond clair, accent unique (bleu ou indigo), beaucoup d’espace blanc
2) Chaleureux et cocooning
   - Ambiance : rassurante, douce, conviviale
   - Couleurs : tons crème / sable / pêche, accent vert sauge ou émeraude, contrastes doux mais lisibles
3) Institutionnel et sérieux
   - Ambiance : sobre, crédible, service public
   - Couleurs : bleu marine / gris, accent discret, mise en page structurée
4) Dynamique et accessible
   - Ambiance : énergique mais lisible, orientée grand public
   - Couleurs : contrastes un peu plus marqués, accent orange ou teal, pictos simples

Consignes pour la charte
- Applique-la partout (cohérence stricte).
- Définis une palette restreinte : 1 fond principal, 1 fond alterné, 1 couleur de texte, 1 couleur secondaire, 1 couleur d’accent.
- Définis des règles simples de mise en page : espacements généreux, cartes arrondies, ombres légères, boutons cohérents.
- Ajoute une règle “interdits” (pas de couleurs hors palette, pas de styles inline, pas de bibliothèques UI externes).
- Assure la lisibilité mobile et l’accessibilité (focus visible, contrastes).

Sortie attendue :
- Rends uniquement UNE version complète du fichier `specs.md`, prête à être utilisée par un agent IA de développement.
- Respecte le format markdown.
- Ne fournis pas d’explications séparées : tout doit être écrit directement dans `specs.md`.