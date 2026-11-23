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

| Objectif | Indicateur de réussite | Échéance |
|---|---|---|
| Valoriser les parcours des lauréats sur le web. | Tous les articles publiés sont consultables sur la plateforme web. | Avant la livraison web. |
| Permettre aux anciens apprenants vérifiés de contribuer. | Seuls les comptes vérifiés disposent des droits de publication ; les auteurs peuvent gérer leurs propres articles. | Avant la livraison web. |
| Assurer la gestion de la plateforme. | Les administrateurs peuvent gérer les articles, les statuts de publication et les comptes. | Avant la livraison web. |
| Faciliter la lecture sur mobile. | Les articles publiés sont consultables dans l'application mobile, sans fonction de rédaction ni d'administration. | Avant la livraison finale. |
| Garantir la cohérence et la qualité. | Les contenus affichés sur le web et le mobile sont cohérents ; les fonctionnalités principales passent les tests. | À chaque sprint et avant la livraison finale. |

*Les échéances précises et la durée des sprints seront confirmées avec le Product Owner.*

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

