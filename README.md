# Explications 
## Texte  
- J'ai utilisé le `text-tranform: uppercase` histoire de bien que j'aurais pu mettre directement ça en MAJ dans le html
- J'ai augmenté la taille de la police à `12px` pour avoir un texte beaucoup plus grand

## Couleurs 
- J'ai prit à l'identique les couleurs de l'image en le cherchant sur l'outil pipette de Photoshop
- Les autres couleurs ont été prise sur le site [color hunt]("https://colorhunt.co")

## Div 
- Choix de mettre des `<p></p>` pour mettre en évidence les textes mais j'aurais pu laissé les textes dans les div

## Animation & transition 
- POssiblité de mettre des animations à la place des transitions 

> Même chose pour les autres éléments (juste une réflexion lors du DM) après je valide qu'on a un code plus court avec `transition`

Au final, j'ai comprit que j'ai juste mal lu la consigne et que la vraie réponse était `transition` 
````css
/* Pour la bannière */
.banniere:active {
    color: white;
    animation-name: texteCouleur;
    animation-duration: 2s;
    animation-timing-function: linear;
}

@keyframes texteCouleur {
    from {
        color: white;
    }
    50% {
        color: #808080;
    }
    to {
        color: black;
    }
}
````
> Code review > Retrait de ces lignes de code inutile car on peut combiner les deux avec les bons css sélecteurs
````css
.article3Colonne2 {
    height: 200px;
    width: 25%;
    color: white;
    background-color: #d35400;
    display: flex;
    align-items: center;
    justify-content: center;
    border: dotted 2px grey;
    box-sizing: border-box;
    text-transform: uppercase;
}
````