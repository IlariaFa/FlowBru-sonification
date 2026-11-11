# FlowBru — Sonification des données environnementales à Bruxelles

## Présentation

Ce projet explore différentes manières de représenter des données environnementales à travers le son et l'image. Il permet d'apprendre à transformer des données
en sons avec la bibliothèque Python STRAUSS. Les données utilisées pour analyser le rapport entre pluie et niveau d'oxygène dans la Senne proviennent de la platforme FlowBru (https://hydria.be/fr/carte-interactive-des-sites/). 

L'idée est de transformer les variations de ces données en sons et de les accompagner de visualisations, pour explorer d'autres façons de percevoir leur évolution dans le temps et voir si la sonification apporte une meilleure comprensions des données.

## Objectifs

- Comprendre les bases de STRAUSS
- Produire une sonification rigureuse sur les données hydrologique choisi et leurs rapports

## Les données

Les données utilisées concernent :

- Les précipitations mesurées à Bruxelles par les 16 pluviometres existants.
- Les concentrations d'oxygène dissous enregistrées par 4 capteurs le long de la Senne.
- Selection de 5 evenements differents pour tester l'efficacité (ou pas) de la sonification dans differetns situations
- Les premiers essais portent sur la journée du **24 juillet 2025**, avec des mesures toutes les cinq minutes. Cette date as été choisie car elle presente des précipitations irregulières et des changements de niveau d'oxygène hétèreogenes.

## Organisation du projet

Le travail est organisé dans plusieurs notebooks Python :

- **02_pluie_bruxelles.ipynb** : exploration des précipitations et premières sonifications.
- **03_oxygene_senne.ipynb** : exploration et sonification des concentrations d'oxygène.
- **04_pluie_oxygene.ipynb** : travail sur les données de pluie et d'oxygène ensemble.
- **05_carte_flowbru.ipynb** : premières visualisations cartographiques.
- **06_carte_oxygene_senne.ipynb** : visualisation des concentrations d'oxygène sur la Senne, avec deux essais graphiques (cercles et barres), puis création d'une vidéo associant l'animation et le son.

## Sonification et visualisation

J'utilise Python et la bibliothèque **STRAUSS** pour transformer les données en sons.

Je développe également des animations qui permettent de suivre les changements dans le temps.

Pour les concentrations d'oxygène, j'ai d'abord essayé des cercles dont la taille varie selon les mesures. J'ai ensuite testé des barres, qui rendent les changements plus visibles.

## Premiers résultats

Une première vidéo associe l'animation des concentrations d'oxygène dans la Senne à leur sonification.

[▶ Voir la vidéo de la Senne avec son](https://github.com/IlariaFa/FlowBru-sonification/blob/main/outputs/senne_oxygene_avec_son.mp4)

## Suite du projet

Les prochaines étapes consistent à :

- Explorer d'autres journées et comparer les variations observées.
- Réunir les précipitations et les concentrations d'oxygène dans une même animation.
- Associer les différentes sonifications aux visualisations.
- Améliorer progressivement les choix graphiques et sonores.

Le projet est en cours de développement. Les notebooks conservent les différentes étapes de recherche et d'expérimentation.

## Remarques

- Le mapping de la sonification (choix de caracteristiques osnores pour traduire les caracteristoques des données) n'est pas definitif; 
- La visualisation choisie n'est pas definitif mais just exploratoire
