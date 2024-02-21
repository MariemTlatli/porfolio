# média querry et transitions :  
# Média querry : 
## 1. Introduction
Les Media Queries sont une fonctionnalité CSS3 qui permettent d'appliquer des styles différents en fonction des caractéristiques du média sur lequel la page web est affichée, telles que la taille de l'écran, l'orientation ou le type de périphérique.

## 2. Syntaxe de base
   ```
  /* Syntaxe générale */
@media type and (expression) {
  /* Styles à appliquer */
}
   ```
## 3. Exemples simples
   Media Queries pour les tailles d'écran :
 ```
/* Appliquer des styles si la largeur de l'écran est inférieure à 600px */
@media screen and (max-width: 600px) {
  body {
    font-size: 14px;
  }
}
 ```
Media Queries pour les orientations :
 ```
/* Appliquer des styles spécifiques en mode paysage */
@media screen and (orientation: landscape) {
  .container {
    width: 80%;
  }
}
 ```
Media Queries pour les types de périphériques :
   ```  
/* Appliquer des styles uniquement pour les appareils mobiles */
@media only screen and (max-device-width: 480px) {
  .menu {
    display: none;
  }
}
 ```
## 4. Travail d'aujourd'hui : 
![Jumia](https://github.com/MariemTlatli/porfolio/assets/127855946/25a9c65a-35d9-4739-9f2f-d7e5e84961d7)(https://www.jumia.com.tn/mlp-telephone-tablette/smartphones/)
![cothings](https://github.com/MariemTlatli/porfolio/assets/127855946/87ce637d-9750-47d4-93ee-0b864dc5abdf)(https://cothings.net/collections/robotique)
![Portfolio](https://github.com/MariemTlatli/porfolio/assets/127855946/e70e9515-3cb7-4062-800f-33694b1345fb)
index.html : 
 ```
<div class="flex">
        <div class="child">child one</div>
        <div class="child">child two</div>
        <div class="child">child three</div>
        <div class="child">child four</div>
        <div class="child">child five</div>
        <div class="child">child six</div>
        <div class="child">child seven</div>
        <div class="child">child eight</div>
        <div class="child">child nine</div>
    </div>
 ```
styles.css : 
 ```
/* Styles pour le conteneur flexible */
.flex {
    display: flex; /* Conteneur flexible */
    flex-wrap: wrap; /* Permet aux éléments enfants de passer à la ligne */
    justify-content: space-between; /* Répartit les éléments enfants avec un espacement égal */
}

/* Styles pour les éléments enfants */
.flex .child {
    background-color: #f0f0f0; /* Couleur d'arrière-plan gris clair */
    padding: 20px; /* Ajoute de l'espace à l'intérieur de chaque élément enfant */
    margin-bottom: 10px; /* Ajoute un espacement en bas de chaque élément enfant */
    width: 100%; /* Par défaut, chaque élément occupe toute la largeur disponible */
}

/* Styles pour les écrans entre 769 et 992 pixels */
@media (min-width: 769px) and (max-width: 992px) {
    .flex .child {
        width: calc(50% - 50px); /* Chaque élément occupe la moitié de la largeur moins 50 pixels */
    }
}

/* Styles pour les écrans entre 993 et 1200 pixels */
@media (min-width: 993px) and (max-width: 1200px) {
    .flex .child {
        width: calc(33.33% - 50px); /* Chaque élément occupe environ un tiers de la largeur moins 50 pixels */
    }
}

/* Styles pour les écrans plus larges que 1200 pixels */
@media (min-width: 1201px) and (max-width: 1400px) {
    .flex .child {
        width: calc(25% - 50px); /* Chaque élément occupe environ un quart de la largeur moins 50 pixels */
    }
}

 ```
## Les Transitions :
Les transitions CSS permettent de créer des effets d'animation fluides lorsqu'un élément change d'état, comme lors du survol d'un lien, d'un changement de couleur, ou d'un déplacement d'un élément. Elles permettent de contrôler comment les propriétés CSS changent au fil du temps.
# 2. syntaxe de base : 

transition-property : Cette propriété spécifie la ou les propriétés CSS auxquelles appliquer la transition

transition-duration : Cette propriété définit la durée de l'animation

transition-delay : Optionnel, définit un délai avant le début de la transition.

transition-timing-function : Cette propriété spécifie la fonction de temporisation utilisée pour contrôler la vitesse de la transition.

Les valeurs possibles incluent :

ease: Démarre lentement, accélère au milieu, puis ralentit à la fin (effet fluide par défaut).
    
linear: La transition se produit à une vitesse constante.
    
ease-in: Démarre lentement puis accélère.
    
ease-out: Démarre rapidement puis ralentit.
    
ease-in-out: Démarre lentement, accélère au milieu, puis ralentit à la fin.

# 3. exemple :     
 ```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Transformation au survol en CSS</title>
<style>
    .boite {
        width: 100px;
        height: 100px;
        background-color: red;
        transition-property: transform; /* Spécifie la propriété CSS à laquelle appliquer la transition */
        transition-duration: 1s; /* Durée de l'animation */
        transition-timing-function: ease; /* Fonction de temporisation (facultatif, ici 'ease' pour une transition fluide) */
    }
    .boite:hover {
        transform: rotate(45deg) scale(1.5) translate(50px, 50px); /* Transformation lorsque survolé */
    }
</style>
</head>
<body>
<div class="boite"></div>
</body>
</html>

```
La propriété transform est utilisée pour appliquer différentes transformations à un élément HTML.
Voici quelques exemples de transformations couramment utilisées :

    Rotation (rotate(angle)): Fait pivoter l'élément autour de son point d'origine selon un angle spécifié.

    Redimensionnement (scale(x, y)): Modifie la taille de l'élément selon les facteurs de mise à l'échelle x et y. Si seulement un paramètre est fourni, l'élément est redimensionné de manière égale horizontalement et verticalement.

    Translation (translate(x, y)): Déplace l'élément horizontalement de x pixels et verticalement de y pixels.

# Workshop : 

