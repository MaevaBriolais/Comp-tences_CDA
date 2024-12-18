# TypeScript

> ❌ A travailler

> ✅ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- ### L'intéret de `TypeScript` dans l'IDE ✅ 
    * Sans TypeScript : 
        * L'IDE n'a pas d'informations complètes sur le type des variables ou des fonctions. Cela peut rendre difficile la détection d'erreurs, le refactoring et l'autocomplétion.
        * Il est plus facile d'avoir des erreur de type qui vont entraîner des bug en production.
    * Avec TypeScript : 
        * Il permet d'ajouter des types explicites, ce qui va permettre à l'IDE de détecter plus tôt des erreurs de type et offrir une meilleure suggestion d'autocomplétion.
        * Va rendre l'architecture du code plus fiable et moins sujet aux erreurs car avec TypeScript l'IDE va faire des vérifications de type en temps réel, avertir en cas d'incohérence de type.
- ### Les `types de bases` ✅ 
    * `number` : pour les nombres (entier ou flottants)
    * `string` : pour les chaînes de caractères
    * `boolean` : pour les valeurs true ou false
    * `void` : pour les fonctions qui ne renvoie rien
    *  `null` & `undifined` : pour représenter l'absence de valeur
    * `any`: pour accepter tous les types (⚠️ à éviter) 
- ### Comment et pourquoi `étendre une interface` ✅ 
    * En utilisant le mot clé `extends`qui permet d'ajouter des propriétes à une interface existante sans la modifier directement.
        ```typescript 
        interface Person {
            name: string;
            age: number;
        }

        interface Employee extends Person {
            jobTitle: string;
        }
        ```

- ### Les `classes et les decorators` ✅ 
    * Classes : Typescript apporte des fonctionnalités orientée objet plus robuste à JS, comme `private` et `public` pour la visibilité des propriétés et des méthodes, ainsi que la gestion des constructeurs, héritages et méthodes statics.
        ```typescript
        class Animal {
            constructor(public name: string) {}
            speak() {
                console.log(`${this.name} makes a sound.`);
            }
        }
        class Dog extends Animal {
            speak() {
                console.log(`${this.name} barks.`);
            }
        }
        ```
    * Décorateurs : Ce sont des fonctions spéciales qui peuvent être appliquées à des classes, méthodes, propriétés ou paramètres. Ils sont utilisés pour modifier ou ajouter des comportements à des éléments de code.
        ```typescript
        function log(target: any, key: string) {
            let value = target[key];

            const getter = () => {
                console.log(`Get: ${key} => ${value}`);
                return value;
            };
            
            const setter = (newValue: any) => {
                console.log(`Set: ${key} => ${newValue}`);
                value = newValue;
            };

            Object.defineProperty(target, key, { get: getter, set: setter });
        }

        class Person {
            @log
            name: string;

            constructor(name: string) {
                this.name = name;
            }
        }
        ```

## 💻 J'utilise

### Un exemple personnel commenté ❌ / ✔️

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
