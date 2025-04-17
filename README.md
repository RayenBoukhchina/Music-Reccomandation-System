# Music Recommendation System

Un système de recommandation musicale basé sur le contenu qui suggère des chansons similaires à celles que l'utilisateur aime.

## Fonctionnalités

- Recommande 5 chansons similaires basées sur :
  - Album/Film
  - Artiste(s)
  - Genre musical
  - Note utilisateur
- Interface simple avec une fonction de recherche

## Technologies utilisées

- Python 3
- Pandas (traitement des données)
- Scikit-learn (vectorisation et similarité cosinus)
- Matplotlib/Seaborn (visualisation - non utilisé dans la version finale)
- Pickle (sérialisation du modèle)

## Dataset
Le dataset contient 2391 chansons avec les colonnes suivantes :

Song-Name : Nom de la chanson

Singer/Artists : Artiste(s)

Genre : Genre musical

Album/Movie : Album ou film associé

User-Rating : Note utilisateur (sur 10)

Exemple de données :

Song-Name	Singer/Artists	Genre	Album/Movie	User-Rating
Aankh Marey	KumarSanu MikaSingh NehaKakkar	BollywoodDance	Simmba	8.8
Coca Cola	NehaKakkar TonyKakkar	BollywoodDanceRomantic	LukaChuppi	9.0

## Méthodologie
Prétraitement des données :

Nettoyage des valeurs manquantes

Suppression des doublons

Formatage des notes utilisateur

Création de tags combinant les caractéristiques

Vectorisation :

Utilisation de CountVectorizer avec 2000 features max

Suppression des stopwords anglais

Calcul de similarité :

Similarité cosinus entre les vecteurs de caractéristiques

Recommandation :

Trouve les 5 chansons les plus similaires à la requête

  ## Résultats
Exemple de recommandation pour "Coca Cola" :

Mile Ho Tum (Reprise)

La La La (Baazaar)

Sawan Aaya Hai (Unplugged Version)

Mohabbat Nasha Hai

Helicopter

## Améliorations possibles
Intégration d'un front-end web/mobile

Ajout de fonctionnalités audio (analyse spectrale)

Système hybride combinant filtrage collaboratif

Mise à jour dynamique du dataset
