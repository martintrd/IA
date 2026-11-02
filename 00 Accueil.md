# Carnet de route IA

Parcours en 19 modules et 182 tâches pour comprendre et utiliser l'IA de A à Z : usage quotidien, maths, machine learning, deep learning, LLM, RAG, agents, production, sécurité et droit.

## Comment l'utiliser

1. Coche la case `- [ ]` de chaque tâche terminée.
2. Sous **Mes notes**, écris ce que tu as fait, le code ou le prompt utilisé, et ce que tu en retiens.
3. Chaque nouveau terme va dans le [[Glossaire]], que tu complètes avec tes mots.
4. Pour chaque projet, duplique le [[Modèle de projet]] dans le dossier Projets, et chaque lecture dans le dossier Lectures.

## Trois parcours possibles

Tu n'es pas obligé de suivre l'ordre des modules. Choisis selon ton objectif du moment :

- **Utilisateur avancé (1 à 2 mois)** : [[A01 Culture générale de l'IA|A01]], [[A02 Utiliser les assistants IA au quotidien|A02]], [[A03 Prompt engineering avancé|A03]], [[A17 Éthique, droit et société|A17]].
- **Constructeur d'applications (3 à 6 mois)** : ajoute [[A05 Python pour la donnée|A05]], [[A10 Construire avec les API|A10]], [[A11 RAG et recherche sémantique|A11]], [[A12 Agents et automatisation|A12]], [[A13 IA locale et open source|A13]], [[A15 Mise en production et MLOps|A15]], [[A16 IA et cybersécurité|A16]].
- **Compréhension profonde (6 à 12 mois)** : ajoute [[A04 Les maths essentielles|A04]], [[A06 Machine learning classique|A06]], [[A07 Deep learning|A07]], [[A08 Langage et architecture Transformer|A08]], [[A09 Les grands modèles de langage|A09]], [[A14 IA multimodale et générative|A14]].

Le module A18 (veille et carrière) se mène en continu dès le début.

## Modules

- [[A00 Préparer son environnement]] (7 tâches) · Les outils de base pour suivre tout le parcours.
- [[A01 Culture générale de l'IA]] (9 tâches) · Savoir de quoi on parle, et parler juste.
- [[A02 Utiliser les assistants IA au quotidien]] (9 tâches) · Devenir un utilisateur efficace avant de devenir un constructeur.
- [[A03 Prompt engineering avancé]] (8 tâches) · Obtenir des résultats fiables et reproductibles.
- [[A04 Les maths essentielles]] (9 tâches) · Le minimum nécessaire pour comprendre vraiment ce qui se passe. Peut se faire en parallèle des modules A05 à A07.
- [[A05 Python pour la donnée]] (8 tâches) · L'outil de travail de toute l'IA.
- [[A06 Machine learning classique]] (12 tâches) · Les fondations, encore très utilisées en entreprise.
- [[A07 Deep learning]] (12 tâches) · Les réseaux de neurones, de la théorie au code.
- [[A08 Langage et architecture Transformer]] (9 tâches) · Comprendre la mécanique qui fait tourner tous les LLM.
- [[A09 Les grands modèles de langage]] (11 tâches) · Comment on fabrique, aligne et évalue un LLM.
- [[A10 Construire avec les API]] (10 tâches) · Passer d'utilisateur à développeur.
- [[A11 RAG et recherche sémantique]] (10 tâches) · Faire répondre un modèle à partir de tes propres documents.
- [[A12 Agents et automatisation]] (11 tâches) · Des modèles qui agissent, pas seulement qui répondent.
- [[A13 IA locale et open source]] (9 tâches) · Faire tourner des modèles sur ta propre machine.
- [[A14 IA multimodale et générative]] (8 tâches) · Images, son, vidéo et vision.
- [[A15 Mise en production et MLOps]] (9 tâches) · Ce qui sépare une démo d'un vrai produit.
- [[A16 IA et cybersécurité]] (12 tâches) · Le module qui valorise directement ton profil d'analyste SOC.
- [[A17 Éthique, droit et société]] (9 tâches) · Comprendre les enjeux, pas seulement la technique.
- [[A18 Veille, projets et carrière]] (10 tâches) · Rester à jour et le prouver.

## Progression

Ces tableaux s'affichent avec le plugin communautaire **Dataview**.

### Par module

```dataview
TABLE length(filter(file.tasks, (t) => t.completed)) AS "Faites", length(file.tasks) AS "Total", round(100 * length(filter(file.tasks, (t) => t.completed)) / length(file.tasks)) + " %" AS "Avancement"
FROM "Modules"
SORT file.name ASC
```

### Prochaines tâches

```dataview
TASK
FROM "Modules"
WHERE !completed
LIMIT 5
```

### Mes projets

```dataview
TABLE statut AS "Statut"
FROM "Projets"
WHERE file.name != "Lisez-moi"
```
