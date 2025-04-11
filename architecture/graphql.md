# GraphQL

> [ ] À travailler  
> [x] Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- [x] La différence entre `REST` et `GraphQL`  
    * **REST** : chaque ressource possède son propre endpoint (`/users`, `/posts`, etc.). Une requête renvoie des données prédéfinies.  
    * **GraphQL** : un seul endpoint pour interroger ou modifier les données. Le client précise exactement les données dont il a besoin.  
    * **Avantage de GraphQL** : évite l'overfetching (trop de données) ou l'underfetching (pas assez).  
    * Exemple : `GET /users/1` (REST) vs `query { user(id: 1) { name, email } }` (GraphQL)

- [x] Les besoins auxquels répond GraphQL  
    * Réduction du nombre de requêtes nécessaires (vs REST)  
    * Plus de flexibilité côté client  
    * Évolution plus simple du backend sans casser le frontend  

- [x] Définition d’un `schéma`  
    * C’est la structure du contrat entre client et serveur : il définit les types de données disponibles et comment y accéder.  
    ```graphql
    type User {
        id: ID!
        name: String!
        email: String!
    }

    type Query {
        user(id: ID!): User
    }
    ```

- [x] `Query`  
    * Permet de **lire** des données.  
    ```graphql
    query {
        users {
            id
            name
        }
    }
    ```

- [x] `Mutation`  
    * Permet de **modifier** les données (ajout, mise à jour, suppression).  
    ```graphql
    mutation {
        addUser(name: "Jean", email: "jean@example.com") {
            id
            name
        }
    }
    ```

- [ ] `Subscription`  
    * Sert à recevoir des **données en temps réel**, via WebSocket.  
    * Exemple typique : messages dans un chat, notifications, etc.  

---

## 💻 J'utilise

- [ ] Un exemple personnel commenté

- [ ] Utilisation dans un projet  
    [lien GitHub](...)  
    Description :

- [ ] Utilisation en production si applicable  
    [lien du projet](...)  
    Description :

- [ ] Utilisation en environnement professionnel  
    Description :

---

## 🌐 J'utilise des ressources

- [x] [GraphQL.org](https://graphql.org/) – Site officiel avec docs, guides et exemples  
- [x] [Apollo GraphQL](https://www.apollographql.com/docs/) – Documentation de la suite Apollo (client + serveur)

---

## 🚧 Je franchis les obstacles

- [ ] Point de blocage  
    Description :

- [ ] Plan d'action (à valider par le formateur) :
    - [ ] action 1  
    - [ ] action 2  
    - [ ] action 3  

- [ ] Résolution :

---

## 📽️ J'en fais la démonstration

- [ ] J’ai écrit un [tutoriel](...)  
- [ ] J’ai fait une [présentation](...)
