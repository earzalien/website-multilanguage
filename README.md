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
2. Ajouter vos traductions dans le fichier `lang.json` au format suivant :  
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
5. Cliquer sur un drapeau pour changer la langue; la sélection sera mémorisée.

## Fonctionnalités

- Chargement asynchrone des traductions (JSON).  
- Modification dynamique du contenu textuel et des placeholders.  
- Sauvegarde de la langue sélectionnée avec `localStorage`.  

## Personnalisation

- Ajoutez d’autres langues dans `lang.json`.  
- Modifiez le style CSS selon vos besoins.  
- Intégrez dans tout projet HTML statique.

---

Ce README donne toutes les indications pour le démarrage rapide avec ce gestionnaire multilingue prêt à l’emploi.  
N’hésitez pas à étoffer selon les spécificités de votre projet !  
