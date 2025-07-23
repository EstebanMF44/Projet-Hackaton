# Prédiction de Flux de Transactions à partir de Données de Marché
## Description du projet
Ce projet vise à prédire les flux de transactions financières à partir de données de marché brutes (contenues dans le fichier data.parquet du repo), en s’appuyant sur des modèles de machine learning.
Les données sont traitées depuis des fichiers parquet contenant les infos de chaque transaction. Après préparation des features, nous entraînons différents modèles pour prédire des indicateurs agrégés de flux à court terme (l'objectif étant de prédire sur une fenêtre de 5 minutes).

## Choix techniques
Prétraitement des données : chargement de fichiers parquet avec PyArrow et Pandas, création de features dérivées, puis agrégation par fenêtres temporelles.

Modèles de machine learning utilisés :

Régression linéaire (LinearRegression)

Forêt aléatoire (RandomForestRegressor)

Évaluation à l'aide du score R² et visualisation des performances prédictives via matplotlib.

## Librairies et environnement
Ce projet a été réalisé en Python. Voici les principales bibliothèques utilisées:
numpy	
pandas
scikit-learn
matplotlib
pyarrow

## Rendu
Le rendu final est le dernier commit du fichier projet_hackaton.ipynb, à noter que certains test ont aussi été menés dans le fichier hackaton.ipynb mais non concluants. 
