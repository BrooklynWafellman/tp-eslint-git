## 1.
### 3.

J'ai utilisé la configuration suivante :

 - Javascript
 - problems
 - commonJS
 - None of these
 - No
 - Yes
 - npm 

## 2.
### 1.

Je n'ai pas rencontré d'erreur, je n'ait donc pas pu faire le --fix

## 3.
### 1.

la commande `npx husky install` étant DEPRECATED j'ai utilisé `npx husky init` à la place pour mon installation

### 2.

La commande `npx husky add .husky/pre-commit "npx eslint ."` étant DEPRECATED à cause de add j'ai utilisé `node ./node_modules/husky/lib/bin.js add .husky/pre-commit "npx eslint ."` à la place


### 3.

git commit -m "Test du hook ESLint"

> tp-eslint-git@1.0.0 test
> echo "Error: no test specified" && exit 1

"Error: no test specified" 
husky - pre-commit script failed (code 1)

Cela vient du script test de package.json

## 4.

### 2.

"scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "prepare": "husky",
    "lint": "eslint ."
  },

### 3.

npm run lint

> tp-eslint-git@1.0.0 lint
> eslint .