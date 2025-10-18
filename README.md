## Demo 
Try the online version here:  
[https://earzalien.github.io/website-multilanguage/](https://earzalien.github.io/website-multilanguage/)


# website-multilanguage

This project provides simple multilingual management for static websites.  
It allows switching the content language using flag buttons and saves the chosen language in the browser.

## Repository Content

- `index.html`: HTML page with `data-key` attributes for managing translated texts.  
- `script.js`: JavaScript script to load and apply translations from the JSON file.  
- `lang.json`: JSON file containing translations (to be created as needed).  
- `css/`, `img/` folders for styles and images.

## Usage

1. Clone the repository or download the files.  
2. Add your translations to the `lang.json` file in the following format:
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

3. Update HTML elements with the `data-key` attribute corresponding to the keys in `lang.json`.  
4. Load the page in a modern browser.  
5. Click a flag to change the language; the selection will be saved.

## Adding Other Languages

- To add a language:
- Add the language identifier (e.g., `de` for German, `it` for Italian...) to each key in the `lang.json` file, including the necessary translations.
- Create a corresponding flag button in the `index.html` file with the appropriate `data-lang` attribute:
 ```
&lt;button data-lang="de"&gt;
  &lt;img src="img/flag-de.png" alt="Deutsch" /&gt;
&lt;/button&gt;

 ```
- Place the new flag image file in the `img/` folder (e.g., `img/flag-de.png`).

- Make sure the image filename, `data-lang` attribute, and language identifier in the JSON all match.

## Adding Flag Image Files

- Place the flag image in the `img/` folder:
- Example: `img/flag-it.png` for Italy
- Add an HTML button in `index.html` corresponding to the new language:
&lt;button data-lang="it"&gt; &lt;img src="img/flag-it.png" alt="Italiano" /&gt; &lt;/button&gt; ```
- It is recommended to use images of similar size and format for a better appearance.

# Features
Asynchronous loading of translations from a JSON file.
Dynamic updating of text content and placeholders.
Saving the selected language with localStorage.
Easy support for adding new languages and flag images.

# Customization
Add other languages in lang.json.
Add as many flags as needed in the img/ folder and update the HTML.
Modify the CSS style as needed.

Integrate into any static HTML project.

----------------------------------------------------------------------------------------------------------------
## Démo

Essayez la version en ligne ici :
[https://earzalien.github.io/website-multilanguage/](https://earzalien.github.io/website-multilanguage/)


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
  
 ``` &lt;button data-lang="de"&gt;  &lt;img src="img/flag-de.png" alt="Deutsch" /&gt; &lt;/button&gt; ```
  
  - De placer le fichier image du nouveau drapeau dans le dossier `img/` (par exemple `img/flag-de.png`).

- Veillez à maintenir la cohérence entre le nom de l’image, l’attribut `data-lang` et l’identifiant de langue dans le JSON.

## Ajouter des fichiers d’image drapeau

- Placez l’image du drapeau dans le dossier `img/` :  
  - Exemple : `img/flag-it.png` pour l’Italie
- Ajoutez un bouton HTML dans `index.html` correspondant à la nouvelle langue :  

&lt;button data-lang="it"&gt; &lt;img src="img/flag-it.png" alt="Italiano" /&gt; &lt;/button&gt;


- Il est recommandé d’utiliser des images à taille et format similaires pour une meilleure apparence.

# Fonctionnalités

Chargement asynchrone des traductions depuis un fichier JSON.
Modification dynamique du contenu textuel et des placeholders.
Sauvegarde de la langue sélectionnée avec localStorage.
Prise en charge facile de l’ajout de nouvelles langues et images de drapeaux.

# Personnalisation

Ajoutez d’autres langues dans lang.json.
Ajoutez autant de drapeaux que nécessaire dans le dossier img/ et mettez à jour le HTML.
Modifiez le style CSS selon vos besoins.

Intégrez dans tout projet HTML statique.
