# Blog des Lauréats de l’EFP

## 1. Description du projet
Le projet **Blog des Lauréats de l’EFP** est une application web destinée à valoriser les parcours professionnels des lauréats de Solicode Tanger. Elle permet aux lauréats de publier leurs expériences et aux apprenants actuels de consulter ces témoignages.

---

## 2. Contexte et Objectifs

### Contexte général
- **Établissement** : Solicode Tanger.
- **Promotion** :  2026/2027 DevCave.
- **Formateur référent** : ES-SARRAJ Fouad.

### Démarche pédagogique : Méthode par imitation
Ce projet s'appuie sur la méthode par imitation pour guider l'apprenant pas à pas de A à Z :
- **Tutoriels** : Guides complets détaillant les étapes et les résultats attendus.
- **UA-Lab** : Laboratoires d'apprentissage guidés pour maîtriser les bases théoriques et pratiques.
- **Lab** : Recherche autonome d'une solution technique validée par le formateur.
- **Veille technologique** : Découverte et intégration de nouveaux outils ou composants.
- **Tâches** : Actions pratiques d'ingénierie et d'organisation Scrum.

### Composants pédagogiques (Approche Par Compétences - APC)
- **Domaine de compétence** : Regroupement thématique des compétences du référentiel.
- **Unité d'apprentissage (UA)** :
  - **UA-Tuto** : Unité basée sur des tutoriels pas-à-pas.
  - **UA-Lab** : Unité pratique guidée par le formateur.
  - **UA-tâche** : Unité regroupant les tâches récurrentes de gestion Scrum à chaque sprint.

---

## 3. Stack technique et Architecture
- **Backend** : Laravel.
- **Base de données** : MySQL.
- **Frontend** : Tailwind CSS et Preline UI.
- **Interactions JavaScript** : Alpine.js.
- **Architecture logicielle** : Architecture 3-tier et MVC.
- **Vues** : Gabarits Blade responsives avec HTML5, CSS3 et JavaScript.
- **Modélisation** : Diagramme de contexte et cas d'utilisation avec Mermaid.
- **Gestion de versions & Outils** : Git et GitHub CLI (`gh`).
- **Intelligence Artificielle & Automatisation** : Agent Antigravity (Skills natifs et règles Always-On) Github(Skills natifs et règles Always-On).
- **Documentation et Présentations** : Markdown standard et Marp.
- **Sécurite** : autorisation alpine,authentication laravel.

---

## 4. Organisation des dossiers
- [.agents/](./.agents/) : Configuration native de l'Agent IA (règles permanentes et skills outillés avec leurs missions).
- [docs/](./docs/) : Documentation libre, recherches et veilles technologiques personnelles.

- [issues/](./issues/) : Gestion et suivi des tâches et user stories du projet.
- [tutoriels/](./tutoriels/) : Restitution des tutoriels et ateliers pratiques organisés par domaine.
- [presentations/](./presentations/) : Diaporamas Marp du projet et des restitutions de sprints.
- [rapport/](./rapport/) : Rapport modulaire du projet, chapitres et script de compilation Node.js.
- [sprints/](./sprints/) : Planification Scrum des sprints et suivi de la branche active.

---

## 5. Méthodologie de développement
Le projet intègre les meilleures pratiques de l'ingénierie logicielle :
- **Agile / Scrum** : Découpage par sprints, réunions quotidiennes et revues de sprint.
- **Processus 2TUP** : Séparation claire entre la branche fonctionnelle et la branche technique.
- **Design Thinking** : Conception centrée sur les besoins réels des utilisateurs.
- **Modélisation UML** : Schémas de cas d'utilisation, diagrammes de classes et de séquences.

---

## 6. Équipe projet et rôles Scrum
- **Product Owner** : ES-SARRAJ Fouad.
- **Scrum Master** : El faquihi Ayoub.
- **Équipe de développement** : El faquihi Ayoub.

### Feuille d’engagement active
- [Sprint 0 - Feuille d’engagement](./sprints/sprint-0.md)

---

## 7. Démarrage rapide

### Prérequis
- Git installé sur votre machine.
- GitHub CLI (`gh`) configuré et authentifié.

### Cloner le projet
```bash
git clone https://github.com/elfaquihiayoub/blog-des-laureats.git
cd blog-des-laureats
git checkout sprint1
```