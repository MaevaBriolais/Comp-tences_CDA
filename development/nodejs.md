# Node.js

> ❌ A travailler  
> ✅ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- ### Utilisation d’un système de *livereloading* (`nodemon`) ✅  
    * `nodemon` surveille les fichiers de ton projet et redémarre automatiquement le serveur à chaque modification.  
    * Commande typique :  
      ```bash
      npx nodemon index.js
      ```  
    * Utile pour éviter les redémarrages manuels fastidieux pendant le dev.

- ### Connexion à une base de données avec ou sans ORM/ODM ✅  
    * **Sans ORM/ODM** : utilisation directe de pilotes comme `mongodb` pour se connecter à MongoDB.  
      ```javascript
      const { MongoClient } = require('mongodb');
      const uri = 'mongodb://localhost:27017';
      const client = new MongoClient(uri);

      async function connect() {
          try {
              await client.connect();
              const db = client.db('maDB');
              console.log('Connecté à MongoDB');
          } catch (err) {
              console.error(err);
          }
      }

      connect();
      ```  
    * **Avec ORM/ODM** : `mongoose` permet de créer des modèles et de structurer les données plus proprement.  
      ```javascript
      const mongoose = require('mongoose');

      mongoose.connect('mongodb://localhost:27017/maDB')
          .then(() => console.log('Connecté à MongoDB via Mongoose'))
          .catch(err => console.error(err));
      ```

- ### Développement d’une API REST & GraphQL avec `express` et `graphql` ✅  
    * **REST avec Express** :  
      ```javascript
      const express = require('express');
      const app = express();
      const PORT = 3000;

      app.use(express.json());

      app.get('/users', (req, res) => {
          res.json([{ id: 1, name: 'Alice' }, { id: 2, name: 'Bob' }]);
      });

      app.listen(PORT, () => console.log(`Serveur démarré sur http://localhost:${PORT}`));
      ```  
    * **GraphQL avec express-graphql** :  
      ```javascript
      const express = require('express');
      const { graphqlHTTP } = require('express-graphql');
      const { buildSchema } = require('graphql');

      const schema = buildSchema(`
          type Query {
              hello: String
          }
      `);

      const root = {
          hello: () => 'Hello world!'
      };

      const app = express();
      app.use('/graphql', graphqlHTTP({
          schema,
          rootValue: root,
          graphiql: true,
      }));

      app.listen(4000, () => console.log('GraphQL dispo sur http://localhost:4000/graphql'));
      ```

- ### *Bonus : Manipulation de fichiers avec `fs` et les streams* ✅  
    * Lecture de fichier simple :  
      ```javascript
      const fs = require('fs');

      fs.readFile('monFichier.txt', 'utf8', (err, data) => {
          if (err) throw err;
          console.log(data);
      });
      ```  
    * Utilisation de streams :  
      ```javascript
      const fs = require('fs');

      const readStream = fs.createReadStream('grosFichier.txt', 'utf8');

      readStream.on('data', chunk => {
          console.log('Chunk reçu :');
          console.log(chunk);
      });
      ```

---

## 💻 J'utilise

### Un exemple personnel commenté ❌ / ✔️

```javascript
// this function takes a path to a .md file of the host system and write the HTML version of this file
// the .html file is given back
const convertMDFileToHTML = (pathToMDfile) => /* ... path to HTML file */
```

### Utilisation dans un projet ❌ / ✔️

[lien github](...)

Description :

### Utilisation en production si applicable❌ / ✔️

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources

### Titre

- lien
- description

## 🚧 Je franchis les obstacles

### Point de blocage ❌ / ✔️

Description:

Plan d'action : (à valider par le formateur)

- action 1 ❌ / ✔️
- action 2 ❌ / ✔️
- ...

Résolution :

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
