# titre 

# 1. Introduction
Les Media Queries sont une fonctionnalité CSS3 qui permettent d'appliquer des styles différents en fonction des caractéristiques du média sur lequel la page web est affichée, telles que la taille de l'écran, l'orientation ou le type de périphérique.

# 2. Syntaxe de base
   ```
  /* Syntaxe générale */
@media type and (expression) {
  /* Styles à appliquer */
}
   ```
# 3. Exemples simples
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
# 4. Travail d'aujourd'hui : 
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
.flex {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
.flex .child {
  background-color: #f0f0f0;
  padding: 20px;
  margin-bottom: 10px;
  width: 100%;
}
/* styles for screens between 769 and 992 pixels */
@media (min-width: 769px) and (max-width: 992px) {
  .flex .child {
    width: calc(50% - 50px);
  }
}

/* styles for screens between 993 and 1200 pixels */
@media (min-width: 993px) and (max-width: 1200px) {
  .flex .child {
    width: calc(33.33% - 50px);
  }
}

/* styles for screens larger than 1200 pixels */
@media (min-width: 1201px) and (max-width: 1400px) {
  .flex .child {
    width: calc(25% - 50px);
  }
}
