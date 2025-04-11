# REST API

> ❌ A travailler  
> ✅ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- ### Les `verbes HTTP` ✅  
    * `GET` : récupérer des données  
    * `POST` : créer une ressource  
    * `PUT` : mettre à jour une ressource existante entièrement  
    * `PATCH` : mettre à jour partiellement une ressource  
    * `DELETE` : supprimer une ressource

- ### Les `statuts HTTP` ✅  
    * `200 OK` : requête réussie  
    * `201 Created` : ressource créée  
    * `204 No Content` : requête réussie, mais pas de contenu à renvoyer  
    * `400 Bad Request` : requête invalide  
    * `401 Unauthorized` : accès non autorisé  
    * `403 Forbidden` : accès interdit  
    * `404 Not Found` : ressource inexistante  
    * `500 Internal Server Error` : erreur côté serveur

- ### Les `endpoints` ✅  
    * C’est l’URL d’accès à une ressource  
    * Exemple :  
      - `GET /users` → récupère tous les utilisateurs  
      - `GET /users/1` → récupère l’utilisateur avec l’id 1  
      - `POST /users` → ajoute un nouvel utilisateur

- ### Le `CORS` (Cross-Origin Resource Sharing) ✅  
    * C’est un mécanisme de sécurité qui bloque ou autorise des appels entre domaines différents.  
    * Exemple : frontend en `localhost:3000` qui appelle une API en `localhost:8000` → nécessite que le backend autorise cette origine avec des en-têtes spécifiques.

- ### La `nomenclature recommandée` pour les routes ✅  
    * REST encourage une structure claire et logique :  
        - Noms de ressources au **pluriel** (`/users`, `/posts`)  
        - Utilisation des **verbes HTTP** pour définir l'action (pas dans l’URL)  
        - Routes imbriquées si nécessaire : `/users/1/posts`  
    * ❌ Mauvais : `/getUsers`, `/createUser`  
    * ✅ Bon : `GET /users`, `POST /users`

---

## 💻 J'utilise

### Un exemple personnel commenté ❌ / ✔️

> Exemple : API CRUD pour une todo list en Express avec gestion des routes, statuts HTTP, CORS, etc.

### Utilisation dans un projet ❌ / ✔️

[lien GitHub](...)

Description :

### Utilisation en production si applicable ❌ / ✔️

[lien du projet](...)

Description :

### Utilisation en environnement professionnel ❌ / ✔️

Description :

---

## 🌐 J'utilise des ressources

### MDN – HTTP overview  
- [https://developer.mozilla.org/fr/docs/Web/HTTP](https://developer.mozilla.org/fr/docs/Web/HTTP)  
- Très bon récapitulatif des concepts HTTP (verbes, statuts, headers, etc.)

### RESTful API Design  
- [https://restfulapi.net/](https://restfulapi.net/)  
- Guide complet sur les bonnes pratiques REST

---

## 🚧 Je franchis les obstacles

### Point de blocage ❌ / ✔️

Description :

Plan d'action : (à valider par le formateur)

- action 1 ❌ / ✔️  
- action 2 ❌ / ✔️  
- ...

Résolution :

---

## 📽️ J'en fais la démonstration

- J’ai écrit un [tutoriel](...) ❌ / ✔️  
- J’ai fait une [présentation](...) ❌ / ✔️
