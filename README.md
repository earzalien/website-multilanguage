# website-multilanguage

Ce projet est une gestion multilingue simple pour sites web statiques.  
Il permet de changer la langue du contenu via des boutons drapeaux, et sauvegarde la langue choisie dans le navigateur.

## Contenu du dépôt

- `index.html` : page HTML avec attributs `data-key` pour gérer les textes traduits.  
- `script.js` : script JavaScript pour charger et appliquer les traductions depuis le fichier JSON.  
- `lang.json` : fichier JSON contenant les traductions (à créer selon vos besoins).  
- Dossiers `css/`, `img/` pour styles et images.

## Utilisation

1. Cloner le dépôt ou télécharger les fichiers.  
2. Ajouter vos traductions dans le fichier `lang.json` au format suivant :  
{
"site-title": {
"fr": "Bienvenue sur notre site",
"en": "Welcome to our website",
"es": "Bienvenido a nuestro sitio web"
},
"menu-accueil": {
"fr": "Accueil",
"en": "Home",
"es": "Inicio"
}
}

3. Mettre à jour les éléments HTML avec l’attribut `data-key` correspondant aux clés dans `lang.json`.  
4. Charger la page dans un navigateur moderne.  
5. Cliquer sur un drapeau pour changer la langue ; la sélection sera mémorisée.

## Ajouter d'autres langues

- Pour ajouter une langue, il suffit :
  - D’ajouter l’identifiant de langue (exemple : `de` pour allemand, `it` pour italien...) dans chaque clé du fichier `lang.json` avec les traductions nécessaires.
  - De créer un bouton drapeau correspondant dans le fichier `index.html` avec l’attribut `data-lang` adéquat :
    
    <!-- code html à insérer -->
    <button data-lang="de">
      <img src="img/flag-de.png" alt="Deutsch" />
    </button>
   <!-- fin html -->
  
  - De placer le fichier image du nouveau drapeau dans le dossier `img/` (par exemple `img/flag-de.png`).

- Veillez à maintenir la cohérence entre le nom de l’image, l’attribut `data-lang` et l’identifiant de langue dans le JSON.

## Ajouter des fichiers d’image drapeau

- Placez l’image du drapeau dans le dossier `img/` :  
  - Exemple : `img/flag-it.png` pour l’Italie
- Ajoutez un bouton HTML dans `index.html` correspondant à la nouvelle langue :  

<button data-lang="it"> <img src="img/flag-it.png" alt="Italiano" /> </button>

- Il est recommandé d’utiliser des images à taille et format similaires pour une meilleure apparence.

#Fonctionnalités
Chargement asynchrone des traductions depuis un fichier JSON.

Modification dynamique du contenu textuel et des placeholders.

Sauvegarde de la langue sélectionnée avec localStorage.

Prise en charge facile de l’ajout de nouvelles langues et images de drapeaux.

#Personnalisation

Ajoutez d’autres langues dans lang.json.
Ajoutez autant de drapeaux que nécessaire dans le dossier img/ et mettez à jour le HTML.

Modifiez le style CSS selon vos besoins.

Intégrez dans tout projet HTML statique.
