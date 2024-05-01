# Workshop-epitech-backend

# Bienvenue pour ce workshop

Ici vous aller apprendre comment utiliser bun et hono, 
tout en explorant typescript et mongoDB

## Objectifs 🎯

- Comprendre les fondamentaux de Bun and son role dans le développement backend

- Initiation a typescript dans les projest hono

#### Installer bun

```bash
curl -fsSL https://bun.sh/install | bash
```

#### Créer un projet

```bash
bun init
```

```bash
bun install hono
```

copier le code dans index.ts

```bash
import { Hono } from 'hono';

const app = new Hono();

Bun.serve({
    fetch: app.fetch,
    port: 3000
})
```


## Exercices

### Exercice 1: Envoyer `Hello World` avec hono
**Objectif**: Créer un endpoint qui renvoie `Hello World` en utilisant hono
1. Choisir la bonne méthode HTTP

### Exercice 2: Créer un endpoint qui renvoie un objet
**Objectif**: Créer un endpoint qui renvoie un objet avec les propriétés `name` et `age`

### Exercice 3: Créer un endpoint qui recoit un objet composé de `name`, `email` et `age` le parse et le renvoie



### Exercice 4: base de donner avec mongoDB

**Objectif**: Créer un endpoint qui enregistre un utilisateur dans une base de données mongoDB

1. Installer mongoose

```bash
bun add mongoose
```

2. creer un compte sur mongoDB atlas

3. creer un cluster

4. creer un schema pour l'utilisateur ayant les propriétés `name`, `email` et `password`

5. creer un endpoint qui enregistre un utilisateur dans la base de données (! attention le mot de passe doit etre crypté avant de l'enregistrer)

6. creer un endpoint qui renvoie tous les utilisateurs

### Exercice 5: Authentification

**Objectif**: Créer un endpoint qui permet de s'authentifier

1. creer un endpoint qui renvoie true si l'utilisateur existe et que le mot de passe est correct

### Exercice 6 Middleware
Objectif: Mettre en place une validation des données pour assurer l'intégrité des informations reçues par votre API.

Utilisez 'zod' pour définir un schéma de validation pour les données entrantes.
Créez un endpoint qui accepte des données d'utilisateur et utilisez le schéma de validation pour vous assurer que les données sont correctes avant de les traiter ou de les enregistrer dans la base de données.

### Exercice 8: Gestion des autorisations
Objectif: Implémenter un système d'autorisation pour contrôler l'accès aux ressources de votre API.

Créez un système de gestion des rôles et des autorisations basique. Par exemple, définissez des rôles comme "utilisateur" et "administrateur".

Ajoutez des middleware d'authentification et d'autorisation pour protéger certains endpoints ou ressources sensibles. Assurez-vous que seuls les utilisateurs autorisés peuvent accéder à ces ressources.

### Exercice 9: Tests unitaires
Objectif: Mettre en place des tests unitaires pour garantir le bon fonctionnement de votre application.

Utilisez un framework de test comme Jest ou Mocha pour écrire des tests unitaires pour vos endpoints.
Testez chaque endpoint avec différentes entrées et assurez-vous que les réponses sont correctes et que les erreurs sont gérées comme prévu.
