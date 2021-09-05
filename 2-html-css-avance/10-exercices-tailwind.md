<!-- omit in toc -->
# Exercices Tailwind

Parcourons ensemble [la documentation de Tailwind](https://tailwindcss.com/docs) pour apprendre à l'utiliser.

Malheureusement celle-ci est en anglais. N'hésite pas à utiliser Google Traduction si besoin.

Je vais te guider pas à pas.

<!-- omit in toc -->
## Table des matières

- [Mise en place](#mise-en-place)
- [Concept de base](#concept-de-base)
  - [Utility-First](#utility-first)
  - [Responsive Design](#responsive-design)
  - [Hover, Focus, & Other States](#hover-focus--other-states)
- [Première page](#première-page)
  - [Le début](#le-début)
  - [Allons plus loins](#allons-plus-loins)

## Mise en place

1. Crée donc une énième page `html` avec pour nom: `tailwind.html`
2. Copie-colle le code suivant dans ta balise `<head>` pour intégrer la feuille de style CSS Tailwind par défaut.

```html
<link href="https://unpkg.com/tailwindcss@^2/dist/tailwind.min.css" rel="stylesheet">
```

3. Maintenant suit le pas à pas pour réaliser ta première page avec Tailwind

## Concept de base

### Utility-First

1. Consulte la page [utility-first](https://tailwindcss.com/docs/utility-first)

**Ce qu'il faut retenir:**

- On applique des styles directement via des classes, sans écrire de CSS
- On ne perd pas de temps à inventer des noms de classes
- Ton CSS ne grossit plus, plus besoin de dupliquer tes valeurs, tu utilise celle de Tailwind
- C'est plus sûr, quand tu agis sur ton CSS c'est global et tu peux à tout moment tout casser. Avec les classes, tout se passe sur ta page et ton élément.

[:arrow_up: Revenir au top](#table-des-matières)

### Responsive Design

1. Consulte la page [responsive design](https://tailwindcss.com/docs/responsive-design)

**Ce qu'il faut retenir:**

- Les différents breakpoints (sm, md, lg, xl et 2xl)
- Il suffit d'écrire un breakpoint suivi de 2 points et la nouvelle valeur pour appliquer un nouveau style à ton élément.
- Il faut penser son design en mobile-first
- Il est possible de customiser ses breakpoint

[:arrow_up: Revenir au top](#table-des-matières)

### Hover, Focus, & Other States

1. Consulte la page [Hover, Focus, & Other States](https://tailwindcss.com/docs/hover-focus-and-other-states)

**Ce qu'il faut retenir:**

- Un peu comme les breakpoints, il suffit d'écrire l'état voulu suivi de 2 points puis du nouveau style.
- Il est possible de cibler les éléments enfants avec `first`, `last`, `even`, `odd`,...

[:arrow_up: Revenir au top](#table-des-matières)

## Première page

Voyons maintenant un peu comment on peut commencer notre page.

Je vais décrire ici mon processus de réflexion pour créer cette page en imaginant que je n'y connais rien à Tailwind.

### Le début

1. J'aimerai commencer par mettre un block qui contiendra un titre avec un fond de couleur.
2. Je consulte la page [container](https://tailwindcss.com/docs/container)
3. Dans la page `tailwind.html` j'insère une `<div>` avec la classe `container`. J'ajoute un simple `Bienvenue`.
4. Je consulte ensuite la page [background-color](https://tailwindcss.com/docs/background-color)
5. J'aimerai un fond rouge, j'insère alors dans ma classe de ma `<div>` le nom suivant: `bg-red-700`
6. Je me rends compte que mon container n'est pas centré, je consulte donc la page [margin](https://tailwindcss.com/docs/margin) car j'aimerai avoir des marges automatiques de chaque côté.
7. J'ajoute la classe `mx-auto` pour ajouter une Marge auto sur l'axe X (gauche et droite)
8. Ajoutons maintenant un fond à notre page. Dans la balise `<body>` j'ajoute une classe `bg-red-100`.
9. Le texte de mon container est noir et j'aimerai bien qu'il ressorte un peu plus. Je consulte la page [text-color](https://tailwindcss.com/docs/text-color)
10. J'ajoute à mon container la classe `text-white`.
11. J'aimerai que toutes les lettres soient en majuscules, je consulte la page [text-transform](https://tailwindcss.com/docs/text-transform) et j'ajoute `uppercase` à la suite de ma classe.
12. Il faudrait augmenter un peu la taille de mon texte, je consulte donc la page [font-size](https://tailwindcss.com/docs/font-size) et j'ajoute `text-4xl`.
13. Augmentons la weight de notre police en consultant [font-weight](https://tailwindcss.com/docs/font-weight) et en ajoutant `font-bold`
14. Maintenant il faudrait centrer le texte, voyons voir ce qu'on trouve sur la page [text-align](https://tailwindcss.com/docs/text-align). On peut donc utiliser `text-center`
15. Ajoutons maintenant un peu de [padding](https://tailwindcss.com/docs/padding) et margin à notre container. On va ajouter `p-5 my-5`.
16. Finissons par donner un petit côté un peu plus doux à notre container avec un [border-radius](https://tailwindcss.com/docs/border-radius): `rounded-3xl`

Voilà déjà un élément mis en place très facilement. Tu vois, c'est simple, il suffit d'allez voir la documentation et d'expérimenter.

[:arrow_up: Revenir au top](#table-des-matières)

**Ce qu'il faut retenir:**

- La documentation est bien fichue et se sert du noms des propriétés CSS qu'on connaît déjà pour nous indiquer quoi faire.
- La documentation c'est le bien absolu!

### Allons plus loins

:hammer_and_wrench: *J'y travaille...*