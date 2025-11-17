Catalogue Films et Séries via une BDD (base de données)

Contexte du projet

Ce projet consiste à créer une application qui permet de rechercher des films et des séries grâce à l’API OMDB.

Le but était de pouvoir taper un titre, filtrer les résultats, voir les détails et ajouter certains contenus en favoris.

Les favoris sont sauvegardés dans le navigateur pour pouvoir les retrouver plus tard.

Fonctionnalités

- Recherche de films et séries avec un champ de texte.
- Plusieurs filtres : genre, note minimale, année, type (film ou série).
- Affichage des résultats avec le titre, l’année et l’affiche.
- Possibilité d’ajouter ou retirer un film/série des favoris.
- Une section dédiée pour afficher les favoris.
- Les favoris sont enregistrés dans le localStorage.

Fonctionnement du projet

1) HTML

Le fichier index.html contient :

un champ de recherche
un bouton pour lancer la recherche
des filtres (genre, note, année, type)
un bouton pour afficher les favoris
un espace pour afficher les résultats
une zone séparée pour les favoris

La structure est simple pour rester claire et facile à utiliser.

2. CSS

Le fichier style.css met en place :

- un fond sombre
- une mise en page centrée
- des cartes pour afficher les films
- des boutons pour liker ou retirer des favoris

Le but était d’avoir une interface propre et agréable à lire.

3) JavaScript

Le fichier app.js contient toute la logique :

- connexion à l’API OMDB avec la clé API
- récupération des résultats selon la recherche
- récupération des détails complets de chaque film ou série
- application des filtres (genre, note, année..)
- affichage des résultats dans des cartes
- système de favoris avec localStorage
- mise à jour des boutons Like selon si un film est favori ou non

La fonction searchMovies() gère toute la recherche et les filtres.

La fonction displayResults() affiche les résultats à l’écran.

La fonction toggleFavorite() ajoute ou retire un film/une série des favoris.

Objectifs atteints

Ce projet permet :

- de chercher facilement des films et séries
- d’appliquer plusieurs filtres
- de garder des favoris enregistrés
- de gérer les données dynamiquement avec JavaScript

Il montre l’utilisation d’une API, la manipulation du DOM, la gestion d’événements et l’utilisation du localStorage.

Structure du projet

/

|-- index.html

|-- style.css

|-- app.js
