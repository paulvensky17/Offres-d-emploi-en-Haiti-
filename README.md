# Offres-d-emploi-en-Haiti- [Consulter le rapport interactif](https://fykyg6-paul-ralph.shinyapps.io/app_doc_emploi/)

Ce projet propose une analyse descriptive du marché du travail en Haïti, basée sur un échantillon d'offres d'emploi collectées en ligne. Il s'inscrit dans une démarche visant à évaluer le potentiel des modèles de langage (LLM) pour la création de données structurées à partir de sources non structurées, dans des contextes où les données officielles sont rares.

## Objectif
L'objectif principal est double :
- Illustrer une méthodologie utilisant le web scraping et les modèles de langage (LLM) pour transformer du texte brut en données structurées et analysables.
- Produire une analyse exploratoire des caractéristiques des offres d'emploi en Haïti.

## Méthodologie
- Collecte des données : Les pages web des annonces ont été collectées via des requêtes HTTP (Requests) depuis le site JobPaw, puis analysées avec Beautiful Soup pour en extraire le contenu textuel.

- Extraction et structuration : Le texte brut de chaque offre a été traité par un LLM via l'API OpenAI, à l'aide d'un prompt conçu pour extraire des champs structurés (titre, domaine, diplôme, expérience, type de contrat, compétences, etc.).

- Analyse : Les données générées ont été agrégées et analysées pour dégager des tendances descriptives.


##  Principaux Résultats (Exploratoires)
L'analyse d'environ 959 offres fait ressortir les tendances suivantes :

- Domaines majoritaires : Management/gestion, finance/comptabilité/commerce (~37% des offres).

- Type de contrat : Prépondérance des CDD (50,1%) sur les CDI (44,2%).

- Diplôme requis : Le niveau Licence est le plus demandé (51% des offres).

- Expérience : La majorité des offres ciblent des profils confirmés (2 à 5 ans d'expérience). Les opportunités pour les juniors (< 2 ans) sont très limitées (6,26%).

- Variations sectorielles : Les exigences en expérience et diplôme varient significativement selon les domaines d'activité.


## Stack Technique
- Collecte de données : Requests, Beautiful Soup

- Traitement & Structuration : OpenAI API 

- Analyse & Visualisation : dplyr, plotly

- Rapport & Publication : Quarto

