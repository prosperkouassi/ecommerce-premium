# HOPLA DEV — Règles de contribution pour agents de code

## Priorité
1. Lire README.md, package.json, configurations, documentation et ce fichier avant toute édition.
2. Préserver les fonctionnalités, la charte graphique, les routes et les comportements existants.
3. Ne pas effectuer de refonte globale sans demande explicite.
4. Réaliser des modifications petites, lisibles, réversibles et liées à la tâche.

## Technologies
- Respecter les versions installées de Next.js, React, TypeScript et Tailwind.
- Préférer les Server Components ; utiliser `use client` seulement quand nécessaire.
- Respecter le typage strict, les alias et les conventions du dépôt.
- Utiliser MySQL/MariaDB et Prisma uniquement si le projet l'exige.

## Qualité
- Responsive mobile/tablette/desktop et accessibilité clavier.
- SEO : métadonnées, titres hiérarchisés, URLs propres et contenu sémantique.
- Performance : optimiser images, fonts, chargement et bundles.
- Sécurité : validation serveur, contrôle d'accès, pas de secret commité, aucune donnée sensible dans les logs.
- Ne pas inventer de connecteur externe ; vérifier sa documentation et prévoir un mode simulation explicite.

## Processus
- Avant : résumer l'objectif, les fichiers concernés et les risques.
- Pendant : ne pas toucher aux zones hors périmètre.
- Après : exécuter les vérifications disponibles (lint, typecheck, build, tests) ; signaler les vérifications impossibles.
- Livrer : résumé des modifications, résultats des tests, risques résiduels et instructions de vérification.
- Git : branche dédiée, PR relue ; pas de merge, force-push, déploiement ou changement de secrets sans accord.

## Contexte spécifique
Consulter `PROJECT_CONTEXT.md` à la racine. Si absent, demander les données bloquantes et proposer de le créer. Les instructions propres au projet priment sur les préférences génériques tant qu'elles ne compromettent pas la sécurité.
