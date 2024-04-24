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


- target directory: my-app
- Which template do you want to use?: bun
- Which package manager do you want to use? bun

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
