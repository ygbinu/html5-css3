## Classes (.) et id(#) CSS
Les classes css sont utilisées sur plusieurs tags tandis qu'un id css s'utilise sur un seul tag
la bonne pratique est de souvent utiliser les classes car les la plupart des framworks front comme angular ou react écrase les valeurs des id

## Organisation d'une page 
Les div permettent de structer la page. Si un div contient plusieurs autres div, les div contenus sont comme des colonnes du div conteneur.
Un div est une balise block c'est à dire occupe toute la ligne disponible sur laquelle il se trouve.

## CSS Flexbox
CSS Flexbox, ou Flexible Box Layout, est un modèle de mise en page en CSS conçu pour organiser et aligner les éléments dans un conteneur de manière efficace, quelle que soit leur taille ou leur position.

| **Catégorie**               | **Propriété**                | **Rôle**                                                                                     | **Exemple**                                                                                                    |
|-----------------------------|------------------------------|---------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------|
| **Conteneur (Parent)**      | `display`                    | Active le mode Flexbox (`flex` ou `inline-flex`).                                            | `display: flex;`                                                                                             |
|                             | `flex-direction`             | Définit l'orientation principale des éléments (horizontal, vertical, etc.).                 | `flex-direction: row;`                                                                                         |
|                             | `flex-wrap`                  | Permet aux éléments de se placer sur plusieurs lignes si nécessaire.                        | `flex-wrap: wrap;`                                                                                             |
|                             | `flex-flow`                  | Abréviation de `flex-direction` et `flex-wrap`.                                              | `flex-flow: row wrap;`                                                                                         |
|                             | `justify-content`            | Aligne les éléments enfants horizontalement dans le conteneur (alignement sur l'axe principal).| `justify-content: center;`                                                                                     |
|                             | `align-items`                | Aligne les éléments enfants verticalement dans le conteneur (alignement sur l'axe transversal).| `align-items: stretch;`                                                                                      |
|                             | `align-content`              | Aligne les lignes de la grille de flexbox lorsque plusieurs lignes existent.                | `align-content: space-between;`                                                                                |
| **Élément (Enfant)**        | `flex-grow`                  | Détermine la capacité d'un élément à grandir par rapport aux autres éléments.                | `flex-grow: 1;`                                                                                               |
|                             | `flex-shrink`                | Définit la capacité d'un élément à se rétrécir par rapport aux autres éléments.              | `flex-shrink: 1;`                                                                                             |
|                             | `flex-basis`                 | Définit la taille initiale d'un élément avant qu'il ne soit redimensionné par `flex-grow` ou `flex-shrink`. | `flex-basis: 100px;`                                                                                          |
|                             | `flex`                       | Abréviation de `flex-grow`, `flex-shrink`, et `flex-basis`.                                 | `flex: 1 1 100px;`                                                                                           |
|                             | `align-self`                 | Aligne un élément individuellement sur l'axe transversal (verticalement).                   | `align-self: center;`                                                                                         |
|                             | `order`                      | Définit l'ordre dans lequel un élément apparaît dans le conteneur (par défaut 0).           | `order: 2;`                                                                                                    |


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

| **Catégorie**               | **Propriété**                | **Rôle**                                                                                     | **Exemple**                                                                                                    |
|-----------------------------|------------------------------|---------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------|
| **Conteneur (Parent)**      | `display`                    | Active le mode Grid Layout (`grid` ou `inline-grid`).                                        | `display: grid;`                                                                                             |
|                             | `grid-template-columns`      | Définit le nombre, la largeur et la disposition des colonnes de la grille.                  | `grid-template-columns: 100px 200px 100px;`                                                                   |
|                             | `grid-template-rows`         | Définit le nombre, la hauteur et la disposition des lignes de la grille.                    | `grid-template-rows: 50px auto 50px;`                                                                         |
|                             | `grid-template-areas`        | Définit des zones nommées pour positionner les éléments enfants facilement.                 | `grid-template-areas: "header header header" "main main sidebar" "footer footer footer";`                    |
|                             | `grid-column-gap` ou `column-gap` | Définit l'espace entre les colonnes.                                                       | `column-gap: 20px;`                                                                                            |
|                             | `grid-row-gap` ou `row-gap`  | Définit l'espace entre les lignes.                                                         | `row-gap: 10px;`                                                                                                |
|                             | `gap`                        | Combinaison de `row-gap` et `column-gap`.                                                   | `gap: 10px 20px;`                                                                                             |
|                             | `justify-items`              | Aligne les éléments enfants horizontalement dans leurs cellules (`start`, `center`, etc.).  | `justify-items: center;`                                                                                        |
|                             | `align-items`                | Aligne les éléments enfants verticalement dans leurs cellules (`start`, `center`, etc.).    | `align-items: start;`                                                                                           |
|                             | `place-items`                | Abréviation pour `justify-items` et `align-items`.                                          | `place-items: center;`                                                                                         |
|                             | `justify-content`            | Aligne la grille entière horizontalement dans le conteneur (`start`, `space-between`, etc.).| `justify-content: space-between;`                                                                              |
|                             | `align-content`              | Aligne la grille entière verticalement dans le conteneur (`start`, `space-around`, etc.).   | `align-content: center;`                                                                                       |
|                             | `place-content`              | Abréviation pour `justify-content` et `align-content`.                                      | `place-content: center;`                                                                                       |
|                             | `grid-auto-rows`             | Définit la hauteur des lignes générées automatiquement.                                     | `grid-auto-rows: 100px;`                                                                                      |
|                             | `grid-auto-columns`          | Définit la largeur des colonnes générées automatiquement.                                   | `grid-auto-columns: 150px;`                                                                                   |
|                             | `grid-auto-flow`             | Contrôle l’ordre de placement des éléments auto-ajoutés (`row`, `column`, `dense`).         | `grid-auto-flow: row dense;`                                                                                   |
| **Élément (Enfant)**        | `grid-column-start`          | Définit la colonne où commence un élément.                                                 | `grid-column-start: 1;`                                                                                        |
|                             | `grid-column-end`            | Définit la colonne où se termine un élément.                                               | `grid-column-end: 3;`                                                                                          |
|                             | `grid-column`                | Abréviation pour `grid-column-start` et `grid-column-end`.                                  | `grid-column: 1 / 3;`                                                                                         |
|                             | `grid-row-start`             | Définit la ligne où commence un élément.                                                   | `grid-row-start: 2;`                                                                                           |
|                             | `grid-row-end`               | Définit la ligne où se termine un élément.                                                 | `grid-row-end: 4;`                                                                                             |
|                             | `grid-row`                   | Abréviation pour `grid-row-start` et `grid-row-end`.                                        | `grid-row: 2 / 4;`                                                                                             |
|                             | `grid-area`                  | Place un élément dans une zone nommée définie par `grid-template-areas`.                    | `grid-area: header;`                                                                                           |
|                             | `justify-self`               | Aligne un élément individuellement horizontalement (`start`, `center`, etc.).              | `justify-self: end;`                                                                                           |
|                             | `align-self`                 | Aligne un élément individuellement verticalement (`start`, `center`, etc.).                | `align-self: center;`                                                                                          |
|                             | `place-self`                 | Abréviation pour `justify-self` et `align-self`.                                           | `place-self: center;`                                                                                         |
