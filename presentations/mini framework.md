---
marp: true
theme: gaia
paginate: true
header: "Blog des Lauréats de l’EFP"
footer: "Architecture du mini-framework MVC"
style: |
  section {
    --color: #2563eb;
    background: #f8fafc;
    color: #1e293b;
    font-family: "Aptos", "Segoe UI", sans-serif;
    font-size: 24px;
    line-height: 1.45;
    padding: 58px 72px;
  }

  section h1 {
    color: #0f172a;
    font-size: 38px;
    margin: 0 0 24px;
    padding-bottom: 12px;
    border-bottom: 2px solid #dbeafe;
  }

  section h2 {
    color: #1d4ed8;
    font-size: 29px;
  }

  section header,
  section footer {
    color: #64748b;
    font-size: 13px;
  }

  section strong {
    color: #0f172a;
  }

  section.lead {
    background: linear-gradient(135deg, #0f172a 0%, #163b72 62%, #2563eb 100%);
    color: #f8fafc;
    justify-content: center;
  }

  section.lead h1 {
    color: #ffffff;
    font-size: 58px;
    border: 0;
  }

  section.lead h2 {
    color: #bfdbfe;
  }

  section.lead strong,
  section.lead header,
  section.lead footer {
    color: #ffffff;
  }

  section.blank {
    background: linear-gradient(135deg, #0f172a 0%, #163b72 100%);
    color: #ffffff;
    justify-content: center;
  }

  section.blank h1 {
    color: #ffffff;
    font-size: 52px;
    border: 0;
  }

  section.blank header,
  section.blank footer {
    color: #cbd5e1;
  }

  table {
    font-size: 20px;
  }

  code {
    font-size: 0.9em;
  }

  pre {
    font-size: 19px;
  }

  blockquote {
    background: #eff6ff;
    border-left: 8px solid #2563eb;
    color: #334155;
    font-size: 22px;
    padding: 12px 18px;
  }
---

<!-- _class: lead -->
# Architecture du mini-framework MVC

## Blog des Lauréats de l’EFP

**Article · Catégorie · Router · Service · MVC**

---

# Objectifs de l’architecture

- Séparer les responsabilités dans le code
- Faciliter la maintenance et l’évolution
- Réutiliser les traitements communs
- Structurer la logique métier
- Simplifier la compréhension du projet

> L’application utilise une architecture MVC enrichie par une couche **Service**.

---

# Entités métier

## Article

- Représente une publication d’un lauréat
- Entité principale du blog
- Contient le titre, le contenu et les informations associées

## Catégorie

- Permet de classer les publications
- Une catégorie contient plusieurs articles
- Un article appartient à une seule catégorie

---

# Structure du projet

```text
app/
├── Models/
│   ├── Article.php
│   └── Categorie.php
├── Controllers/
│   ├── ArticleController.php
│   └── CategorieController.php
└── Services/
    ├── BaseService.php
    ├── ArticleService.php
    └── CategorieService.php
```

```text
resources/views/     routes/web.php
├── articles/
└── categories/
```

---

# Responsabilités des couches

| Couche | Responsabilité |
|---|---|
| **Router** | Associer une URL à une action |
| **Controller** | Recevoir la requête et coordonner les traitements |
| **Service** | Appliquer les règles métier |
| **BaseService** | Fournir les méthodes communes |
| **Model** | Accéder aux données et représenter les entités |
| **View** | Afficher les informations à l’utilisateur |

---

# Organisation des Services

```text
BaseService
├── Méthodes communes
└── Fonctionnalités réutilisables

ArticleService
└── Hérite de BaseService
└── Gère la logique des articles

CategorieService
└── Hérite de BaseService
└── Gère la logique des catégories
```

- `ArticleService` et `CategorieService` héritent de `BaseService`
- Les services spécifiques peuvent appeler directement leurs Models
- La logique métier reste indépendante de l’affichage

---

# Schéma global

```text
Utilisateur
     ↓
    View
     ↓
   Router
     ↓
 Controller
     ↓
ArticleService / CategorieService
     ↓
 BaseService
     ↓
   Model
     ↓
   MySQL
```

---

# Exemple : création d’un article

1. **View** : l’utilisateur saisit les données du formulaire
2. **Router** : dirige la requête vers `ArticleController`
3. **Controller** : récupère les données et appelle `ArticleService`
4. **ArticleService** : vérifie les données et applique les règles métier
5. **BaseService** : fournit les méthodes communes nécessaires
6. **Model** : `Article` enregistre les données dans MySQL
7. **Controller / View** : affiche une confirmation à l’utilisateur

---

<!-- _class: blank -->
<!-- _paginate: false -->

# Avantages de cette organisation

---

# Pourquoi cette architecture ?

- **Maintenance** : chaque couche possède une responsabilité précise
- **Réutilisation** : `BaseService` évite la duplication de code
- **Lisibilité** : le flux des requêtes est facile à suivre
- **Évolutivité** : une nouvelle entité peut suivre le même modèle
- **Testabilité** : les règles métier sont isolées dans les Services

> Le mini-framework reste léger tout en introduisant une séparation claire des responsabilités.

---

# Conclusion

- Le **Router** dirige les requêtes
- Le **Controller** coordonne les traitements
- Les **Services** appliquent la logique métier
- `BaseService` centralise les méthodes communes
- Les **Models** gèrent les entités et les données
- La **View** présente les résultats

**Résultat : un code organisé, maintenable et évolutif.**
