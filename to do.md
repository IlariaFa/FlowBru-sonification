 19.11.26

#### Choses à corriger dans les notebook du debut (jusqu'au 08) 
- Ordre des stations : sur ta carte, l’ordre le long de la Senne est Q01, Q04, Q03, Q02 (de l’amont vers l’aval, à confirmer).
Or ta position stéréo suit l’ordre des numéros, de 0,25 à 0,75. Ton oreille entendrait donc un ordre gauche-droite 
qui ne correspond pas à la rivière.
- Échelles incohérentes : les barres et les cercles n’ont pas la même échelle entre les notebooks 06 et 07.
- Gain de la pluie : le notebook 04 normalise le son par son maximum, ce qui rendrait un clip presque sec aussi fort qu’un orage.
- Nombre de clips : j’ai figé 16 clips, soit 8 avec événement et 8 sans. Auparavant je disais « 4 à 8 sans », 
ce qui donnait entre 12 et 16.
- Limite à écrire dans le mémoire : comme le son porte la pluie et l’oxygène, tu ne pourras pas dire laquelle des deux aide.

#### Choses faites
-  verification seulle oxygéne:  seuil critique pour la vie piscicole est de 3 mg/l dans l'article : 
https://environnement.brussels/citoyen/documentation-et-outils/etat-des-lieux-de-lenvironnement/eaux-usees-epuration?utm_source=chatgpt.com
En revanche, l'article ne justifie pas une durée de 15 minutes. 
Cette durée minimale est un choix méthodologique visant à écarter les fluctuations ponctuelles.
Pour justifier ce choix:

##### Nombre d’épisodes détectés

| Station | ≥ 10 min | ≥ 15 min | ≥ 30 min |
|---------|----------|----------|----------|
| Q01 | 20 | 14 | 11 |
| Q02 | 176 | 108 | 72 |
| Q03 | 32 | 28 | 20 |
| Q04 | 60 | 49 | 37 |
| **Total par station** | **288** | **199** | **140** |

Un épisode correspond à des mesures consécutives sous 3 mg/L, sans interruption. Un même événement touchant plusieurs stations peut être compté plusieurs fois.

##### Épisodes regroupés entre stations

En regroupant les épisodes simultanés entre stations :

| Durée minimale | Nombre d'épisodes |
|----------------|-------------------|
| ≥ 10 min | **218** |
| ≥ 15 min | **141** |
| ≥ 30 min | **92** |

#### Choix des evenement apres analyse des fichers contenant les données 
Fichiers du 1er juillet au 30 septembre 2025. Sélection concrète de 16 extraits de 2 heures.

##### 8 extraits avec baisse d’oxygène
Date et heure	Stations concernées	Pourquoi
- 6 juillet, 12–14 h	Q01, Q02, Q03, Q04	Plusieurs baisses, fortes pluies généralisées
- 20 juillet, 17–19 h	Q01, Q03, Q04	Baisses importantes, presque sans pluie
- 24 juillet, 19–21 h	Q02, Q04	Réutilise ton prototype existant
- 2 août, 14–16 h	Q02	Baisse principalement localisée
- 31 août, 17–19 h	Q03	Forte baisse à une station, après un épisode pluvieux
- 3 septembre, 22–00 h	Q01, Q02, Q04	Plusieurs stations touchées, pluie présente
- 15 septembre, 7–9 h	Q02, Q04	Deux stations touchées, pluie présente
- 19 septembre, 21–23 h	Q04	Baisse isolée, sans pluie enregistrée pendant l'extrait

##### 8 extraits sans baisse
Toutes les stations restent au-dessus de 3 mg/L pendant ces fenêtres.
Date et heure	Pourquoi
- 10 juillet, 12–14 h	Situation stable, sans pluie
- 17 juillet, 6–8 h	Pluie légère sans baisse
- 24 juillet, 12–14 h	Même journée qu'un événement, mais sans baisse
- 10 août, 12–14 h	Faible pluie, oxygène normal
- 20 août, 12–14 h	Situation stable
- 31 août, 6–8 h	Pluie sur les 16 pluviomètres, sans baisse
 -22 septembre, 12–14 h	Pluie faible sans baisse
- 25 septembre, 12–14 h	Oxygène élevé et stable
