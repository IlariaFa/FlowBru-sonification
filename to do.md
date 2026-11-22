 19.11.26

#### Choses à corriger dans les notebook du debut (jusqu'au 08) 
- Ordre des stations : sur ta carte, l’ordre le long de la Senne est Q01, Q04, Q03, Q02 (de l’amont vers l’aval, à confirmer).
Or ta position stéréo suit l’ordre des numéros, de 0,25 à 0,75. Ton oreille entendrait donc un ordre gauche-droite 
qui ne correspond pas à la rivière.
- Échelles incohérentes : les barres et les cercles n’ont pas la même échelle entre les notebooks 06 et 07.
- Gain de la pluie : le notebook 04 normalise le son par son maximum, ce qui rendrait un clip presque sec aussi fort qu’un orage.
- Nombre de clips : j’ai figé 16 clips, soit 8 avec événement et 8 sans. Auparavant je disais « 4 à 8 sans », 
ce qui donnait entre 12 et 16.
- Limite à écrire dans le mémoire : comme le son porte la pluie et l’oxygène, on ne peut pas dire laquelle des deux aide.

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
Les extraits expérimentaux ont été sélectionnés à partir d'une analyse automatisée des mesures historiques de 2025. Les épisodes de faible oxygénation ont été identifiés à l'aide d'un seuil de 3 mg/L maintenu pendant au moins 15 minutes. Les extraits ont ensuite été sélectionnés pour représenter différentes situations : épisodes localisés ou touchant plusieurs stations, avec ou sans précipitations. Des périodes sans baisse d'oxygène ont également été retenues pour évaluer les fausses alertes.
Je ne vais pas choisir automatiquement les 8 baisses les plus fortes. Ce serait trop facile pour les participants et peu représentatif. Je vais inclure des cas plus subtils, tout en vérifiant qu'ils restent perceptibles dans les vidéos.

Fichiers du 1er juillet au 30 septembre 2025. Sélection concrète de 16 extraits de **2 heures**.
Dans le première exemple du 24 juillet: choix de 24h (une journée) mais risque de rendre trop dilué et donc peu percevables des variations d'oxygène sur 15min donc choix d'un laps de temps plus courte pour l'analyse.

##### 8 extraits avec baisse d’oxygène
Date et heure, 	Stations concernées,	Pourquoi
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
Date et heure,	Pourquoi
- 10 juillet, 12–14 h	Situation stable, sans pluie
- 17 juillet, 6–8 h	Pluie légère sans baisse
- 24 juillet, 12–14 h	Même journée qu'un événement, mais sans baisse
- 10 août, 12–14 h	Faible pluie, oxygène normal
- 20 août, 12–14 h	Situation stable
- 31 août, 6–8 h	Pluie sur les 16 pluviomètres, sans baisse
- 22 septembre, 12–14 h	Pluie faible sans baisse
- 25 septembre, 12–14 h	Oxygène élevé et stable

###### Code python pour verifier les données et choisir ces dates: aller dans le ficher iphnb

20.11.26

#### Ajouter des questions secondaires 
- Le son aide-t-il à repérer la succession temporelle entre les épisodes de pluie et la baisse d'oxygène?
- La sonification aide-t-elle à distinguer une pluie localisée d'une pluie généralisée ?
- La sonification aide-t-elle à détecter et localiser les baisses d'oxygène ?

Ces 3 questions supplementaires portent sur 3 dimensions differentes mais interessantes: la chronologie, la répartition spatiale de la pluie et la détection des baisses d'oxygène

22.11

#### Ecriture d'un planning provisoire
Étape 1 — Terminer le code du notebook 10 pour sonifier automatiquement les 16 événements avec les paramètres provisoires.  
Étape 2 — Choisir les sons définitifs, confirmer l'ordre des stations et corriger le gain de la pluie.  
Étape 3 — Avant l'expérience: Corriger les échelles des cartes si nécessaire, générer les 16 extraits audiovisuels définitifs et vérifier qu'ils sont comparables.  
Étape 4 — Expérience et mémoire: Faire les tests avec les participants, analyser les réponses et rédiger les limites méthodologiques.

Les verifications à faire dans la phase finale:

##### Corrections à effectuer avant l'expérience

| Point | Correction à faire | Moment |
|---|---|---|
| Ordre des stations | Vérifier l'ordre géographique Q01, Q04, Q03, Q02 et adapter les positions stéréo. | Avant les sons définitifs |
| Échelles des cartes | Harmoniser les échelles des barres et des cercles dans les notebooks 06 et 07. | Avant les vidéos définitives |
| Gain de la pluie | Éviter de normaliser chaque extrait par son maximum afin de conserver les différences d'intensité entre les événements. | Avant les tests |
| Choix des sons | Comparer les timbres et choisir les sons définitifs pour la pluie et l'oxygène. | Après le notebook 10 |
| Nombre d'extraits | Conserver 16 extraits : 8 avec baisse d'oxygène et 8 sans. | Déjà validé |
| Limite méthodologique | Si la pluie et l'oxygène sont sonifiés ensemble, il n'est pas possible d'attribuer séparément l'effet de chaque variable. | Dans le mémoire |
