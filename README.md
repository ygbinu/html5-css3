## Classes (.) et id(#) CSS
Les classes css sont utilisées sur plusieurs tags tandis qu'un id css s'utilise sur un seul tag
la bonne pratique est de souvent utiliser les classes car les la plupart des framworks front comme angular ou react écrase les valeurs des id

## Organisation d'une page 
Les div permettent de structer la page. Si un div contient plusieurs autres div, les div contenus sont comme des colonnes du div conteneur.
Un div est une balise block c'est à dire occupe toute la ligne disponible sur laquelle il se trouve.
## Flex box
Technique CSS pour faire des mises en page. 
```css
display: flex;
```
Active le mode Flexbox sur un conteneur et rend flexibile la mise en page de ses enfants car à différentes propriétés flex.
## Padding
Espace entre un conteneur et son contenu. S'exprime en padding-top, padding-right, padding-bottom padding-left.
La bonne pratique est d'exprimer la même valeure pour top et bottom et la même valeure pour right et left.
```css
/*60px top et bottom et 100px right et left*/
padding: 60px 100px;
```
## Margin
Espace entre le body et son contenu, par défaut il existe un marging 8px entre le body et son contenu.

## 