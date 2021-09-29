# Premiers pas

## Exercice 1

1. Créez une page `index.html` et `script.js`
2. Lier la page JS à votre page HTML
```html
<script src="script.js">
```
3. Insérez la balise suivante
```html
<div id="exercice"></div>
```
4. Insérez la chaine de caractère suivante dans la balise div à l'aide de votre page `script.js`

`Hello, World!`

<details>
  <summary><strong>Réponse</strong></summary>

  ```js
  document.getElementById("exercice").innerHTML = "Hello, World"
  ```

</details>

