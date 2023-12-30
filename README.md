# PROJET PYTHON DATA SCIENCE 

Ce dépot réuni notre travail au cours de l'UE Python pour la data science enseigné à l'ENSAE (Membres : Zakaria BOULLIAIRE, Massyle DENDENE, Brian RAMESH)

# **<span style="color: #CC146C">Analyse de sentiments sur les critiques allocine </span>** 🎥


Ce projet est réalisé dans le cadre pédagogique du cours de Python pour Data Science de 2A à l’ENSAE.

## Présentation


Lorsque nous décidons de regarder un film, nous regardons souvent la note du film et même les critiques associées à ce film. Cela nous permet de nous faire un premier avis et peut même parfois influencer notre approche sur le film. Les critiques sont donc des éléments clés dans l’analyse d’un film.


## Question et Structure 


Ce projet essaie donc de voir si les critiques d’un film arrive à prédire la performance au box-office d’un film. Le but est donc d’analyser les sentiments que renvoient les critiques et essayer de tester le pouvoir de prédiction de cette information par la suite. 

Notre projet s’axe autour des éléments clés de l’analyse des données : récupération et nettoyage des données, analyse visuelle et modélisation/application. Ces étapes structurent notre raisonnement et nous guideront jusqu’à la fin du projet.


## Contenu 


Au niveau du code nous avons décidé de séparer (pour plus de lisibilité) notre rapport en deux avec :

notebook final 
Modélisation

Les bases de données étant très volumineuses et les processus de récupération prenant beaucoup de temps, nous fournissons les données dans le dossier dataframes pour les informations concernant les films selon l’organisation suivante :

de
De
De
De

La base des critiques se trouve à ce lien :

Mettre le lien ici 

On peut y accéder à travers le code 



## Recommandation d'exécution


Pour effectuer le code de manière optimale, nous vous conseillons de suivre les étapes suivantes. 

```sh

# Download repo and its dependencies 

git clone https://github.com/TheophileBlard/french-sentiment-analysis-with-bert/

cd french-sentiment-analysis-with-bert

pipenv install


# Extract dataset

pushd allocine_dataset && tar xvjf data.tar.bz2 && popd


# Activate virtualenv and open-up BERT notebook

pipenv shell

jupyter notebook 03_bert.ipynb 

```