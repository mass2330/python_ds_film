# PROJET PYTHON DATA SCIENCE 

Ce dépôt réunit notre projet qui est réalisé dans le cadre pédagogique du cours de Python pour Data Science de 2A à l’ENSAE.
(**Membres du groupe** : Zakaria BOULLIAIRE, Massyle DENDENE, Brian RAMESH)

# **<span style="color: #CC146C">Analyse de sentiments sur les critiques allociné </span>** 🎥

## Présentation

Bienvenus dans notre projet de data science dédié à la prédiction des sentiments des commentaires de films et à l'évaluation de leur impact sur la performance au box office. En effet, lorsque nous décidons de regarder un film, nous regardons souvent la note du film et très souvent les critiques associées à ce film. Cela nous permet de nous faire un premier avis et peut même parfois influencer notre approche sur le film. Les critiques sont donc des éléments clés dans l’analyse d’un film.

## Objectifs du Projet 

L'objectif principal de ce projet est d'exploiter les techniques de traitement du langage naturel (NLP) pour développer un modèle de prédiction de sentiments capable d'analyser les réactions des spectateurs aux films, en se basant sur des données textuelles extraites de commentaires. En utilisant ces prédictions de sentiments, nous cherchons également à établir un lien avec la performance au box office des films. Cela pourrait permettre ainsi aux professionnels de l'industrie cinématographique d'avoir un aperçu préliminaire de la réception du public avant la sortie officielle.

## Méthodologie 

Le projet sera réalisé en plusieurs étapes clés qui vont structurer notre raisonnement :

**1. Collecte de Données** : Issues de scrapping et d'API, les données proviennent essentiellement d'Allociné et sont completées par les données de TMDB.

**2. Nettoyage des données** :  Nettoyage et préparation des informations sur les films mais aussi des données textuelles pour les rendre adaptées à l'analyse, en utilisant des techniques de NLP.

**3. Modélisation/Evaluation** : Entraînement d'un modèle de machine learning pour prédire les sentiments des commentaires de films. Évaluation de la précision et de la fiabilité du modèle de prédiction de sentiments. Établissement d'une corrélation entre les prédictions de sentiments et la performance. Une diversité de modèles est utilisée (Régression Logistique, Random Forest, BERT)

## Structure du projet  

Le projet est organisé en deux notebook, chacun correspondant à une étape spécifique du projet.

- Le notebook ***analyse.ipynb*** contient la partie sur la récupération et le nettoyage des données.

- Le notebook ***modelisation.ipynb*** contient la partie modélisation et conclusion du projet.

Les processus de récupération prennent beaucoup de temps, donc les données sont fournis de la manière suivante (*néanmoins le code pour récupérer les données est présent dans les notebook**): 

 Dans le dossier ***dataframes*** on retrouve : 

- ***df_film_ac.csv*** : les informations des films scrappées Allociné 

- ***df_tmdb.csv*** : les informations des films récupérées sur TMDB 

- ***df_merged.csv*** : le merge des deux tables ci_dessus 

- ***df_modified.csv*** : la version nettoyée de ***df_merged.csv***
    
Dans second temps nous avons également la base des critiques qui est la plus volumineuse, celle-ci est accessible à ce lien : 
     https://www.dropbox.com/scl/fi/oaj2pxpytau536krzjtqj/df_critiques.csv?rlkey=uemvi7feslmnta3mgg6ahtpen&dl=1

Les modèles entraînés sont également accessibles à : RAJOUTER OU.


## Prérequis et Recommandation d'exécution

Avant de commencer, nous vous conseillons de suivre les étapes suivantes. Il est conseillé également d'appliquer le code sur SSPCloud avec un environnement avec GPU pour une optimalité dans les calculs et la modélisation.

```sh

#Installation de l'environnement virtuel (code à appliquer sur le terminal)
    python -m pip install virtualenv
    python -m virtualenv .venv
# Activation de l'environnement virtuel
    source .venv/bin/activate
`
git clone https://github.com/mass2330/python_ds_film
cd python_ds_film

# Pour installer les dépendance dans son environnement

pip install - r requirements.txt

```

Nous vous souhaitons une bonne lecture. Nous sommes ouverts aux suggestions de développement des analyses plus approfondies et des modèles améliorés dans le cadre de cette étude. N'hésitez pas à nous faire part de vos retours, suggestions et contributions.