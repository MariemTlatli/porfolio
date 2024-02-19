
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
![image](https://github.com/MariemTlatli/porfolio/assets/127855946/315637bd-05db-499c-a908-ee26f4d419b8)
![image](https://github.com/MariemTlatli/porfolio/assets/127855946/8f63830c-504c-4869-8259-c29fc92b4337)


