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

#### Checklist — Finalisation du mémoire

##### Préparation

- [ ] **Corrections techniques** : vérifier l'ordre géographique (Q01, Q04, Q03, Q02), la spatialisation stéréo, le gain de la pluie (sans normalisation individuelle) et les échelles des cartes (notebooks 06–07).
- [ ] **Sons définitifs** : comparer les timbres pluie/oxygène après le notebook 10 et fixer les paramètres.
- [ ] **Visualisation / Figma** : finaliser l'interface et produire les supports audiovisuels synchronisés.
- [ ] **16 stimuli** : générer 8 extraits avec baisse d'oxygène et 8 sans ; vérifier durée, synchronisation, lisibilité et volume.

### Expérience

- [ ] **Questionnaire et protocole** : définir les questions, les conditions avec/sans son, l'ordre de présentation et les critères de réussite.
- [ ] **Test pilote** : tester avec 2–3 personnes (compréhension, difficulté, son, durée).
- [ ] **Expérience** : faire passer les tests et collecter les réponses.

### Analyse et rédaction

- [ ] **Résultats** : comparer avec/sans son (précision, erreurs, détection, localisation) à partir des réponses attendues.
- [ ] **Mémoire** : rédiger méthodologie, résultats, discussion, limites et conclusion.

**Points de vigilance**
- Figma ne remplace pas les supports finaux synchronisés.
- Prévoir les mesures d'analyse dès la conception du questionnaire.
- Si pluie et oxygène sont sonifiés ensemble, leurs effets individuels ne peuvent pas être isolés.

__________

24.11.26

Choix

## 2. Application directe à ton mémoire

Tu dois partir de tes questions de recherche pour déterminer tes choix visuels.

| Ce que le participant doit percevoir | Encodage visuel possible |
| --- | --- |
| Une diminution de l'oxygène | Hauteur des barres |
| La station touchée par une baisse | Position géographique |
| L'intensité de la pluie | Surface des cercles |
| Une pluie localisée ou généralisée | Répartition spatiale des cercles |
| La succession entre pluie et baisse d'oxygène | Animation synchronisée et indication temporelle |
| Une concentration critique d'oxygène | Repère visuel du seuil de 3 mg/L, si pertinent pour la tâche |

Á faire: recherches/visualisation et choix/ sonification et choix/ reste dans le notebook