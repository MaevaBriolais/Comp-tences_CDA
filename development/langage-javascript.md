# Langage Javascript

> ❌ A travailler

> ✅ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- #### Les `structures` de base du langage ✅ 
    * Variables : 
        * let / const / (var)
    * Types de données : 
        * Simples : string / number / boolean / undifined / null
        * Complexes : object / array / function
    * Opérateurs :
        * Arithmétiques : + _ * /
        * Comparaison : === / == / < / >
        * Logique : && / || / !
    * Structures conditionelles :
        * if / else / else if 
    * Les boucles : 
        * for / while / do ... while 

- #### Les normes `ecmascript` ✅ 
    * C'est la norme qui définit le langage JS, elle évolue et ajoute des fonctionnalités comme par exemple :
        * ES5 :
            * Compatibilité avec les anciens navigateurs
            * Méthode Array.map() / Array.forEach()
        * ES6 :
            * Arrivée de let / const / class / fonctions fléchées / promesse
    
- #### L'utilisation de l'`asynchrone` ✅ 

    JavaScript est mono-thread = executer une seule tâche à la fois dans l'ordre du code. Cependant sans asynchronisme il existe des opérations qui peuvent bloquer l'exécution du reste du code donc l'asynchronisme permet de lancer ces tâches "en arrière plan" sans bloquer la suite.

        * Callback function : C'est une fonction passée en argument, appelée après une tâche 

            ```javascript
            setTimeout(() => {
                console.log("Fin");
            }, 1000);
            ```
        * Promesses : C'est une abstraction pour gérer l'asynchrone

            ```javascript 
            fetch("https://api.xxx.com")
                .then(response => response.json())
                .then(data => console.log(data))
                .catch(error => console.error(error));
            ```
        * Async / Await : Utilisé pour simplifier les promesses avec une syntaxe plus lisible

            ```javascript
            async function fetchData() {
                try {
                    const response = await fetch("https://api.xxx.com");
                    const data = await response.json();
                    console.log(data);
                } catch (error) {
                    console.error(error);
                }
            }
            ```

- #### Les spécifités du mot-clef `this` ❌ (A REVOIR pas tout à fait à l'aise sur le sujet)
    * Fait référence à l'object courant dans lequel le code est exécuté, suivant le contexte :
        * Global : Dans un navigateur, this pointe vers l'object global window

        ```javascript
        console.log(this);
        ```

        * Object/méhode : Dans une méthode d'oject this va pointer vers lui même

        ```javascript
        const obj = {
            name: "Alice",
            sayName() {
                console.log(this.name);
            }
        };
        obj.sayName(); // "Alice"
        ```

        * Fonctions fléchées : this hérite du contexte parent

        ```javascript 
        const obj = {
            name: "Alice",
            sayName: () => {
                console.log(this.name);
            }
        };
        obj.sayName(); // undefined
        ```


## 💻 Je code en Javascript

### Un exemple de code commenté ❌ / ✔️

```javascript
(e) => mc2;
```

### Utilisation dans un projet ❌ / ✔️

[lien github](...)

Description :

### J'ai utilisé ce langage en production ❌ / ✔️

[lien du projet](...)

Description :

### J'ai utilisé ce langage en environement professionnel ❌ / ✔️

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

