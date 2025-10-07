# Récapitulatif du cours du 30/09

## Introduction

* **JavaScript** a été créé en **1995** par **Brendan Eich**.
* Son nom a évolué : *Mocha* → *LiveScript* → *JavaScript* (choisi pour surfer sur la popularité de Java à l’époque).
* Aujourd’hui, JavaScript (souvent abrégé **JS**) est le langage principal pour rendre les pages web interactives.

---

## Variables

En JavaScript, une variable permet de stocker une valeur. On peut la déclarer avec trois mots-clés :

* `let` → variable avec une portée limitée au **bloc** (`block scope`).
* `const` → variable **constante**, on ne peut pas réaffecter sa valeur.
* `var` → ancienne façon de déclarer une variable, aujourd’hui à éviter (portée globale ou de fonction).

### Exemple de déclaration

```js
let firstname = 'Charles';
let lastname = 'Zecevic';
let total = firstname + " " + lastname;
```

* `let` → mot-clé de déclaration.
* `firstname` → nom de la variable.
* `=` → opérateur d’affectation.
* `'Charles'` → valeur de type **string**.
* `total` → contiendra la **concaténation** des deux chaînes.

---

## Types de données

* `'Charles'` → **string** (chaîne de caractères).
* `123` → **number** (nombre entier ou décimal).
* `true / false` → **boolean** (valeurs logiques).
* `null` → représente une valeur vide volontairement.
* `undefined` → signifie qu’une variable existe mais n’a **aucune valeur définie**.

---

## Affichage dans la console

```js
console.log(variable);
```

* `console.log` → méthode permettant d’afficher une valeur dans la console du navigateur.
* `(variable)` → contenu que l’on veut afficher.

---

## Opérateurs

### Mathématiques

* `+ - * /` → addition, soustraction, multiplication, division.
* `+= -= *= /=` → opérations combinées (incrémentation / décrémentation).
* `%` → **modulo** : reste d’une division.

  * Exemple : `20 % 4 = 0`, `23 % 6 = 5`.

### Comparaison

* `> < >= <=` → supérieur, inférieur, supérieur ou égal, inférieur ou égal.
* `==` → égalité (compare les valeurs sans vérifier les types).
* `===` → stricte égalité (compare les valeurs **et** les types).

### Logiques

* `&&` → ET : `true && false` → `false`.
* `||` → OU : `true || false` → `true`.
* `!` → NON : `!true` → `false`.

---

## Conditions

Les conditions permettent d’exécuter du code seulement si certaines règles sont respectées.

### if / else if / else

```js
if (condition) {
  // Code exécuté si la condition est vraie
} else if (autreCondition) {
  // Code exécuté si la 1ère condition est fausse mais celle-ci vraie
} else {
  // Code exécuté si aucune condition n’est remplie
}
```

Exemple :

```js
let age = 18;

if (age < 18) {
  console.log("Mineur");
} else if (age === 18) {
  console.log("Tout juste majeur !");
} else {
  console.log("Adulte");
}
```
