# Note de cadrage — Blog des Lauréats

**Statut :** Document soumis à la validation du Product Owner (Groupe 1)

## 1. Présentation du Projet & Contexte Institutionnel

Le Blog des Lauréats de Solicode a pour objectif de valoriser les parcours des anciens apprenants et de partager leurs expériences professionnelles avec les apprenants actuels et le grand public.

Les articles présenteront leur parcours depuis la formation jusqu'à leur situation professionnelle actuelle, les difficultés rencontrées et les conseils qu'ils souhaitent transmettre.

Le projet comprend deux supports :
- **Plateforme web :** consultation publique, contribution des anciens apprenants vérifiés et administration.
- **Application mobile :** consultation du catalogue et lecture des articles publiés uniquement.

Les anciens apprenants pourront créer un compte. Après vérification manuelle de leur statut par un administrateur, ils pourront publier directement leurs articles, puis modifier ou supprimer leurs propres publications. Les articles seront accessibles publiquement sans compte. Les administrateurs pourront gérer tous les articles et les comptes utilisateurs.

## 2. Objectifs Stratégiques & SMART

La méthode SMART permet de vérifier qu'un objectif est suffisamment clair, quantifiable, réalisable, adapté aux moyens disponibles et limité dans le temps.

- **Spécifique (S) :** un objectif doit décrire précisément le résultat attendu, les utilisateurs concernés et les actions à réaliser. Pour ce projet, l'objectif est défini autour de la mise à disposition d'une plateforme permettant aux lauréats de publier leurs parcours et aux visiteurs de consulter ces publications.
- **Mesurable (M) :** un objectif doit comporter des éléments observables permettant d'évaluer sa réalisation. Les preuves retenues seront les fonctionnalités validées, les tests réussis et la disponibilité effective des articles sur les supports concernés.
- **Atteignable (A) :** un objectif doit rester possible à atteindre avec les compétences, les ressources et le temps disponibles. Le développement sera donc découpé en sprints afin de progresser par étapes et de résoudre les difficultés au fur et à mesure.
- **Réaliste (R) :** un objectif doit correspondre aux contraintes du projet et aux technologies maîtrisées. Laravel, MySQL, Blade, Tailwind CSS, Preline UI, Alpine.js et NativePHP constituent l'ensemble technique retenu pour concevoir les fonctionnalités prévues.
- **Temporel (T) :** un objectif doit être associé à une échéance claire. Le projet sera évalué à la fin de chaque sprint, puis une première version complète sera livrée à l'issue du cycle de développement.

## 3. Matrice de Périmètre

### In-Scope — Périmètre inclus

| Support | Fonctionnalités |
|---|---|
| **Plateforme web** | Consultation des articles par catégorie ; recherche ; lecture complète ; profils des lauréats ; création de compte et authentification ; vérification manuelle des anciens apprenants ; création, publication, modification et suppression de ses propres articles par un lauréat vérifié ; espace d'administration ; gestion des articles, des statuts de publication et des comptes utilisateurs. |
| **Application mobile** | Affichage du catalogue des articles publiés et lecture complète des articles en lecture seule. |

### Out-of-Scope — Périmètre exclu

- **Application mobile :** rédaction, création, publication, modification ou suppression d'articles ; modération ; gestion des comptes et administration.
- **Projet global :** messagerie instantanée, paiement en ligne et fonctionnalités complexes de réseau social.

## 4. Parties Prenantes

| Partie prenante | Rôle |
|---|---|
| Product Owner — Groupe 1 | Définit les besoins, priorise les fonctionnalités et valide le cadrage. |
| Développeurs web | Réalisent la plateforme web et son espace d'administration. |
| Développeurs mobile | Réalisent l'application mobile de consultation. |
| Formateurs référents | Accompagnent et suivent le projet. |
| Administrateurs Solicode | Vérifient les anciens apprenants et gèrent les comptes et les articles. |
| Anciens apprenants / lauréats | Partagent leurs expériences en publiant et en gérant leurs articles. |
| Apprenants et visiteurs | Consultent librement les articles sur ordinateur ou smartphone. |

## 5. Contraintes Majeures & Risques Identifiés

### Contraintes

- **Techniques :** Laravel, MySQL, Blade, Tailwind CSS, Preline UI, Alpine.js et NativePHP. Les tests unitaires et fonctionnels seront réalisés dans une démarche TDD. L'environnement prévu comprend Windows, PowerShell, Composer, Node.js, Android Studio et Git. Les données publiées devront être accessibles de façon cohérente depuis le web et l'application mobile.
- **Temporelles :** le projet sera réalisé par sprints. La durée des sprints et la date de livraison restent à confirmer avec le Product Owner.
- **Juridiques :** respecter les règles applicables à la protection des données personnelles, notamment la loi marocaine 09-08 et les formalités de la CNDP. Informer les utilisateurs et obtenir les autorisations nécessaires avant la publication de données personnelles, photos ou témoignages identifiables. Le RGPD s'applique si les conditions de son champ d'application sont réunies.
- **Accessibilité :** proposer des interfaces lisibles et adaptées aux écrans d'ordinateur et de smartphone ; prévoir un contraste suffisant, des libellés explicites et une navigation compréhensible.

### Risques et stratégies d'atténuation

| Risque | Stratégie d'atténuation |
|---|---|
| Manque d'articles disponibles | Identifier et contacter les anciens apprenants suffisamment tôt. |
| Retard dans les sprints | Prioriser les fonctionnalités avec le Product Owner et suivre l'avancement à chaque sprint. |
| Incohérence des contenus entre web et mobile | Définir un mécanisme commun de consultation des articles publiés et tester les échanges à chaque sprint. |
| Vérification incorrecte d'un compte | Réserver l'activation des droits de publication à la validation manuelle d'un administrateur. |
| Publication d'un contenu inapproprié ou non autorisé | Définir des règles de publication et permettre aux administrateurs de modifier, dépublier ou supprimer un article. |

---
