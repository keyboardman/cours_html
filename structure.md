Cours Développement Web

Outils en ligne:
https://playcode.io/

https://codepen.io/
https://picsum.photos/


# HTML

## Introduction
- HTML : structure du document
- CSS: style du document
- Javascript: interaction avec le document

## La syntaxe 
- les balises (Tag HTML en anglais)
    On entoure notre texte de balise

- documentation
    https://developer.mozilla.org/fr/
    l’ensemble des balises surtout celles qui n’ont pas d’icône à gauche (obsolete ou experimentale)

- les attributs
    exemple class=« important»
- l’imbrication des éléments    
    bon : `<p>Hello <strong>Marc</strong> Bienvenue</p>`
    mauvais : `<p>Hello <strong>Marc</p>Bienvenue</strong>`		
- les elements vides:
    `<img src="" alt=""  />`
- structure d’une page web
    ```
    <!DOCTYPE html>
    <html>
        <head>
        </head>
        <body>
        </body>
    </html>		
    ```
    - le head
        informations non visible | pour moteur de recherche
    - body

## Editeur de page web
- VSC
- online: https://codepen.io/

## entête WEB
- titre dans l’onglet
  `<title></title>`
- encodage
	`<meta charset="UTF-8" />`
- description
    `<meta name="description" content="mon contenu" />`
- keywords
    `<meta name="keywords" content="...." />`
- autres
    pour les réseaux sociaux
    `<meta property="og:title" content="HTML (HyperText Markup Language) | MDN">`
- language
    `<html lang="fr">`
- la balise link
    elle permet de faire un lien vers une ressource externe à notre page
    - attribut href : url de la resource
    - attribut rel: type de lien (stylesheet)
- la balise style: elle a du contenu css
- la balise script: elle a du contenu javascript

## la balise BODY
- les titres `<h1..6>`
    le numéro définit le niveau d'importance de votre titre
- les paragraphes `<p></p>`
- retour à la ligne `<br>`
- le texte en gras:  `<strong></strong>` sens sémantique pour le moteur de recherche
- le texte en italique: `<em></em>` 
- les listes:
  - non ordonnées : `<ul></ul>`
  - ordonnées: `<ol></ol>`
  - imbriquer
    ```
    <ol>
        <li> 1ère ligne
            <ol>
                <li>....</li>
                <li>....</li>
            </ol>
        <li>
        <li></li>
    </ol>
    ```

- les entités:
    https://developer.mozilla.org/fr/docs/Glossary/Entity
    `& &amp;`
    `< &lt;`
    `> &gt;`
    `&nbsp;` espace insécable

- les séparateurs : `<hr>`

## les liens
- on met un chemin
    menu.html : `<a href="menu.html">Vers Menu</a>`
    index.html : `<a href="index.html">Vers Index</a>`
    menu/entree_1.html: `<a href="../index.html">Vers Index</a>`
- on peut mettre des URLS
    index.html : `<a href="https://www.youtube.com">Aller sur Youtube</a>`

- attribut target: comment va s'ouvrir le lien
  - par défaut: _self même page
  - _blank: nouvelle page
- lien interne: commence par #identifiant cible l'attribut id d'un l' élement
    scroll jusqu'à l'élément 
    il doit être unique dans la page

## les images
    - la balise <img >
    - avec deux principaux src="" et alt=""
    - src = lien qui pointe l'image
    - alt = décrit l'image
    - 4 formats de fichiers
      - jpeg/jpg : idéale pour les photos
      - png : supporte la transparence et qualitéÒ  
      - gif : supporte l'animation
      - svg : vectoriel / forme simple
    - attribut width et height : largeur et longueur en pixel
    - optimiser les images (réduire une image en 1920 en 600 ) si on n'affiche qu'une largeur de 600
      - https://imageresizer.com/

## les tables
    - la balise table
    - tr: ligne
    - td: cellule
    - th: cellule d'entête
    - le nombre de colonne doit être rigoureusement identique
    - attribut colspan fusion de colonne 
    - attribut rowspan fusion de ligne

## les iframes
    - attribut src
    - attribut width
    - attribut height
    - exemple: video youtube
  
## les div et les span et autre
    - div : diviser du contenu (bloc) et aucun sens sémantique
    - attribut class
    - span : diviser des phrases
    - div != span : retour à la ligne
    - balise article sens article
    - balise nav sens navigation
    - balise semantique (header, article, footer, aside)

## l'inspecteur
    - clique droit sur la page : Inspecteur
    - Onglet Element pour voir le code HTML
    - erreur possible une balise qui n'a pas sa balise fermante
    - Onglet console permet de voir les erreurs : image non trouvée

## W3C
    - organisation qui organise les standards du web
    - https://www.w3.org/
    - w3c validator : https://validator.w3.org/

## les formulaires
    - balise form 
      - attribut action : où seront envoyé les données du formulaire
      - attribut method : précise la méthode utiliser
    - <label></label> : Libellé du champ
        - attribut for : pointe vers l'id d'un champ et sélectionne le champ
    - <input type="text" name="prenom" value="valeur par défaut" placeholder="exemple">
    - <input type="checkbox">
    - <input type="radio">
    - <input type="hidden">
    - <input type="submit" value="Envoyer un email"> / <button type="submit">Envoyer un email</button>
    - <textarea cols="30" rows="30" placeholder="...." ></textarea>
    - <select><option value="m">Masculin</option><option value="f" selected>Féminin</option></select>
    - <optgroup>
## l'encodage

## TP
    - créer 3 pages pour 1 restaurant
      - créer 1 page accueil avec un texte de présentation du restaurant
        - https://unsplash.com/fr/photos/photo-dun-pub-dans-la-chambre-pendant-la-journee-poI7DelFiVA
      - créer 1 page menu avec un tableau de deux colonnes (entrée, plat, dessert)
        - 1ère colonne nom du plat et ingrédients
        - 2ème colonne le prix
      - créer une page de contact formulaire de 3 champs (email, nom, message)
        - avec l'adresse du restaurant + carte google
