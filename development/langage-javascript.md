# Langage Javascript

> ❌ A travailler

> ✅ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- Les `structures` de base du langage ✅
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

- Les normes `ecmascript` ✅
    * C'est la norme qui définit le langage JS, elle évolue et ajoute des fonctionnalités comme par exemple :
        * ES5 :
            * Compatibilité avec les anciens navigateurs
            * Méthode Array.map() / Array.forEach()
        * ES6 :
            * Arrivée de let / const / class / fonctions fléchées / promesse
    
- L'utilisation de l'`asynchrone` ✅
    * Callback : C'est une fonction passée en argument, appelée après une tâche 
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

- les spécifités du mot-clef `this` ❌ / ✔️


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

