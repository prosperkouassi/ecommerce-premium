# Installation HOPLA DEV

## A. GPT personnalisé ChatGPT
1. Ouvrir ChatGPT > GPTs > Créer (l'intitulé peut varier selon l'interface).
2. Nom : HOPLA DEV — Architecte Next.js.
3. Description : Architecte et développeur Next.js pour concevoir, améliorer et sécuriser les projets web AlteractWeb / Hopla Groupe.
4. Coller intégralement le contenu de `GPT-INSTRUCTIONS.md` dans le champ Instructions.
5. Activer les capacités pertinentes proposées dans l'interface (analyse de fichiers, navigation si disponible).
6. Configurer l'accès GitHub séparément dans les connexions/apps disponibles ; sa présence dans ChatGPT ne garantit pas automatiquement son accès au GPT personnalisé.
7. Garder le GPT privé, le tester sur un dépôt non critique, puis le partager seulement si nécessaire.

## B. Dépôts GitHub
1. Créer une branche `chore/hopla-dev-setup` dans chaque dépôt choisi.
2. Copier `AGENTS.md` à la racine, `templates/PROJECT_CONTEXT.md` vers `PROJECT_CONTEXT.md` à la racine et `.github/pull_request_template.md` vers `.github/pull_request_template.md`.
3. Renseigner `PROJECT_CONTEXT.md` sans y placer de secrets.
4. Ouvrir une pull request et valider les modifications avant fusion.
5. Vérifier que l'outil de codage réellement utilisé lit `AGENTS.md` ; les instructions d'un GPT personnalisé et celles d'un agent de code sont des configurations distinctes.

## C. Travail local
1. Cloner le dépôt dans VS Code.
2. Installer les dépendances avec le gestionnaire de paquets du projet.
3. Créer `.env.local` à partir d'un exemple validé, sans le commiter.
4. Exécuter les commandes définies dans `package.json` (lint, typecheck, build, tests selon disponibilité).
5. Développer sur une branche dédiée ; demander une revue avant fusion et déploiement.

## Exemple de premier message
« HOPLA DEV, voici mon dépôt GitHub [owner/repo]. Commence par auditer son architecture, son SEO, sa sécurité et ses performances, sans modifier le code. Présente ensuite un plan de travail priorisé. »
