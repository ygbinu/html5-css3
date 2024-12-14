## Classes (.) et id(#) CSS
Les classes css sont utilisées sur plusieurs tags tandis qu'un id css s'utilise sur un seul tag
la bonne pratique est de souvent utiliser les classes car les la plupart des framworks front comme angular ou react écrase les valeurs des id

## Organisation d'une page 
Les div permettent de structer la page. Si un div contient plusieurs autres div, les div contenus sont comme des colonnes du div conteneur.
Un div est une balise block c'est à dire occupe toute la ligne disponible sur laquelle il se trouve.

## CSS Flexbox
CSS Flexbox, ou Flexible Box Layout, est un modèle de mise en page en CSS conçu pour organiser et aligner les éléments dans un conteneur de manière efficace, quelle que soit leur taille ou leur position.

| **Catégorie**               | **Propriété**                | **Rôle**                                                                                     |
|-----------------------------|------------------------------|---------------------------------------------------------------------------------------------|
| **Conteneur (Parent)**      | `display`                   | Active le mode Flexbox (`flex` ou `inline-flex`).                                           |
|                             | `flex-direction`            | Définit l'axe principal (`row`, `row-reverse`, `column`, `column-reverse`).                |
|                             | `flex-wrap`                 | Permet aux éléments de passer à la ligne (`nowrap`, `wrap`, `wrap-reverse`).               |
|                             | `flex-flow`                 | Abréviation pour `flex-direction` et `flex-wrap`.                                           |
|                             | `justify-content`           | Aligne les éléments sur l'axe principal (`flex-start`, `center`, `space-between`, etc.).    |
|                             | `align-items`               | Aligne les éléments sur l'axe transversal (`flex-start`, `center`, `stretch`, etc.).        |
|                             | `align-content`             | Aligne les lignes dans un conteneur multi-lignes (`flex-start`, `center`, etc.).            |
| **Élément (Enfant)**        | `order`                    | Définit l'ordre des éléments (par défaut `0`, plus petit ordre affiché en premier).         |
|                             | `flex-grow`                | Contrôle la capacité d'un élément à grandir (par rapport aux autres).                      |
|                             | `flex-shrink`              | Contrôle la capacité d'un élément à rétrécir (par rapport aux autres).                     |
|                             | `flex-basis`               | Définit la taille initiale de l'élément avant que l'espace restant soit distribué.          |
|                             | `flex`                     | Abréviation pour `flex-grow`, `flex-shrink`, et `flex-basis`.                              |
|                             | `align-self`                | Aligne un élément individuellement sur l'axe transversal (`auto`, `flex-start`, etc.).      |

Active le mode Flexbox sur un conteneur et rend flexibile la mise en page de ses enfants car à différentes propriétés flex.
## Padding
Espace entre un conteneur et son contenu. S'exprime en padding-top, padding-right, padding-bottom padding-left.
La bonne pratique est d'exprimer la même valeure pour top et bottom et la même valeure pour right et left.
```css
/*60px top et bottom et 100px right et left*/
padding: 60px 100px;
```
## Margin
Espace entre un conteneur et son environnement extérieur.

## Selection et styles des tags enfants

## Propriétés CSS Grid
CSS Grid Layout, ou simplement CSS Grid, est un système de mise en page puissant qui vous permet de créer des structures complexes en organisant les éléments dans un grille bidimensionnelle. Contrairement à Flexbox, qui est conçu pour travailler sur un axe principal (ligne ou colonne), CSS Grid travaille simultanément sur les axes ligne et colonne, ce qui en fait une solution idéale pour des mises en page plus sophistiquées.

| **Catégorie**               | **Propriété**                | **Rôle**                                                                                     |
|-----------------------------|------------------------------|---------------------------------------------------------------------------------------------|
| **Conteneur (Parent)**      | `display`                   | Active le mode Grid Layout (`grid` ou `inline-grid`).                                        |
|                             | `grid-template-columns`     | Définit le nombre, la largeur et la disposition des colonnes de la grille.                  |
|                             | `grid-template-rows`        | Définit le nombre, la hauteur et la disposition des lignes de la grille.                    |
|                             | `grid-template-areas`       | Définit des zones nommées pour positionner les éléments enfants facilement.                 |
|                             | `grid-column-gap` ou `column-gap` | Définit l'espace entre les colonnes.                                                       |
|                             | `grid-row-gap` ou `row-gap` | Définit l'espace entre les lignes.                                                         |
|                             | `gap`                      | Combinaison de `row-gap` et `column-gap`.                                                   |
|                             | `justify-items`             | Aligne les éléments enfants horizontalement dans leurs cellules (`start`, `center`, etc.).  |
|                             | `align-items`               | Aligne les éléments enfants verticalement dans leurs cellules (`start`, `center`, etc.).    |
|                             | `place-items`               | Abréviation pour `justify-items` et `align-items`.                                          |
|                             | `justify-content`           | Aligne la grille entière horizontalement dans le conteneur (`start`, `space-between`, etc.).|
|                             | `align-content`             | Aligne la grille entière verticalement dans le conteneur (`start`, `space-around`, etc.).   |
|                             | `place-content`             | Abréviation pour `justify-content` et `align-content`.                                      |
|                             | `grid-auto-rows`            | Définit la hauteur des lignes générées automatiquement.                                     |
|                             | `grid-auto-columns`         | Définit la largeur des colonnes générées automatiquement.                                   |
|                             | `grid-auto-flow`            | Contrôle l’ordre de placement des éléments auto-ajoutés (`row`, `column`, `dense`).         |
| **Élément (Enfant)**        | `grid-column-start`         | Définit la colonne où commence un élément.                                                 |
|                             | `grid-column-end`           | Définit la colonne où se termine un élément.                                               |
|                             | `grid-column`               | Abréviation pour `grid-column-start` et `grid-column-end`.                                  |
|                             | `grid-row-start`            | Définit la ligne où commence un élément.                                                   |
|                             | `grid-row-end`              | Définit la ligne où se termine un élément.                                                 |
|                             | `grid-row`                  | Abréviation pour `grid-row-start` et `grid-row-end`.                                        |
|                             | `grid-area`                 | Place un élément dans une zone nommée définie par `grid-template-areas`.                   |
|                             | `justify-self`              | Aligne un élément individuellement horizontalement (`start`, `center`, etc.).              |
|                             | `align-self`                | Aligne un élément individuellement verticalement (`start`, `center`, etc.).                |
|                             | `place-self`                | Abréviation pour `justify-self` et `align-self`.                                           |
