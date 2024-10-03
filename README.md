M1 : Données Climatiques Ouvertes
===================================

> Comment les satellites de la NASA, les données de terrain et les modèles sont-ils utilisés pour diagnostiquer et prédire le système climatique terrestre ? Comment la variabilité climatique est-elle mesurée et modélisée ?

Le premier module de notre [programme d'études en sciences du climat ouvert](https://openclimatescience.github.io/curriculum) se concentre sur la familiarisation des apprenants avec NASA Earthdata Search et avec la variété des ensembles de données climatiques offerts par la NASA. **À la fin de ce module, vous devriez être capable de :**

- Comprendre comment les données climatiques issues des ensembles de réanalyse, des Modèles de Circulation Générale et des Modèles du Système Terrestre sont générées et en quoi ces modèles diffèrent.
- Savoir où trouver différentes variables climatiques (par exemple, les précipitations, la température) aux échelles spatiales et temporelles appropriées.
- Démontrer l'utilisation de plusieurs variables climatiques issues de différents ensembles de données climatiques.

Contenu
---------------

1. [Sources de données climatiques](https://github.com/OpenClimateScience/M1-Open-Climate-Data-FR/blob/main/notebooks/01_Sources_de_donn%C3%A9es_climatiques.ipynb)
2. [Introduction à NASA Earthdata Search et aux données de ré-analyse](https://github.com/OpenClimateScience/M1-Open-Climate-Data-FR/blob/main/notebooks/02_Introduction_%C3%A0_NASA_Earthdata_Search_et_aux_donn%C3%A9es_de_r%C3%A9-analyse.ipynb)
3. [Lecture des données climatiques maillées de MERRA-2](https://github.com/OpenClimateScience/M1-Open-Climate-Data-FR/blob/main/notebooks/03_Lecture_des_donn%C3%A9es_climatiques_maill%C3%A9es_de_MERRA2.ipynb)
4. [Accès aux données MERRA-2 dans le cloud](https://github.com/OpenClimateScience/M1-Open-Climate-Data-FR/blob/main/notebooks/04_Acc%C3%A8s_aux_donn%C3%A9es_MERRA-2_dans_le_cloud.ipynb)
5. [Introduction aux données d’observation de la Terre](https://github.com/OpenClimateScience/M1-Open-Climate-Data-FR/blob/main/notebooks/05_Introduction_aux_donn%C3%A9es_d%E2%80%99observation_de_la_Terre.ipynb)
6. [Introduction aux modèles climatiques](https://github.com/OpenClimateScience/M1-Open-Climate-Data-FR/blob/main/notebooks/06_Introduction_aux_mod%C3%A8les_climatiques.ipynb)
7. [Utilisation des données de ré-analyse pour étudier la sécheresse](https://github.com/OpenClimateScience/M1-Open-Climate-Data-FR/blob/main/notebooks/07_Utilisation_des_donn%C3%A9es_de_r%C3%A9-analyse_pour_%C3%A9tudier_la_s%C3%A9cheresse.ipynb)
8. [Utilisation des observations de la Terre de la NASA](https://github.com/OpenClimateScience/M1-Open-Climate-Data-FR/blob/main/notebooks/08_Utilisation_des_observations_de_la_Terre_de_la_NASA.ipynb)

Commencer
---------------

[Voir notre guide d'installation ici.](https://github.com/OpenClimateScience/M1-Open-Climate-Data-FR/blob/main/HOW_TO_INSTALL_FR.md)

Vous pouvez exécuter les notebooks de ce dépôt en utilisant [Github Codespaces](https://docs.github.com/en/codespaces/overview) ou en tant que [conteneur de développement VSCode](https://code.visualstudio.com/docs/devcontainers/containers). Une fois que votre conteneur est en cours d'exécution, lancez Jupyter Notebook en procédant comme suit :

```sh
# Créez votre propre mot de passe lorsque vous y êtes invité
jupyter server password

# Ensuite, lancez Jupyter Notebook et entrez votre mot de passe lorsque demandé
jupyter notebook

```

Objectifs d'apprentissage
-----------------

Ce cours couvre les [compétences de base en science des données computationnelles :](https://github.com/OpenClimateScience/Core-Competencies/blob/main/ScienceCore-Competencies.md)

- Les données brutes sont non modifiées et conservées séparément de tout dérivé traité ou des résultats d'analyse. (CC1.1)
- Les fichiers d’un projet sont organisés de manière hiérarchique et sémantique. Les données brutes, les données traitées, le code et les résultats sont stockés dans des dossiers distincts. (CC1.2)
- Créer des métadonnées appropriées pour tous les ensembles de données, incluant, mais sans s'y limiter : la date de création, les sources de données principales, les valeurs de remplissage ou plages valides, et les unités. (CC1.9)
- Comprendre les tableaux multidimensionnels et leur utilisation pour représenter des ensembles de données structurés par l'espace, le temps et plusieurs variables. (CC2.3)
- Connaître les différents types d’ensembles de données structurées utilisés dans les applications scientifiques, notamment les ensembles de données spatiales (raster et vecteur) et les ensembles de données hiérarchiques (par exemple, HDF5, netCDF4) ; savoir comment les lire et comment créer des fichiers de données auto-documentés. (CC2.8)
- Choisir des échelles de couleurs linéaires perceptuellement et adaptées aux daltoniens. Comprendre comment les échelles visuelles se rapportent aux différents types de données quantitatives et qualitatives. (CC3.10)
- Les flux de travail computationnels sont documentés à la fois avec des commentaires en ligne et une documentation externe (un README ou une documentation API). (CC4.3)

Ensembles de données climatiques utilisés
---------------------

- Températures de l'air quotidiennes de [l'ensemble de réanalyse MERRA-2 du NASA Global Modeling and Assimilation Office](https://gmao.gsfc.nasa.gov/reanalysis/MERRA-2/)
- Totaux quotidiens de précipitations de [NASA IMERG-Final](https://disc.gsfc.nasa.gov/datasets/GPM_3IMERGDF_06/summary)
- Données sur l'évapotranspiration, le rayonnement et l'humidité des sols issues de [l'ensemble de réanalyse NLDAS de la NASA](https://disc.gsfc.nasa.gov/datasets/NLDAS_NOAH0125_M_2.0/summary?keywords=NLDAS)
- Température de l'air, pression et humidité issues des [données de forçage NLDAS de la NASA](https://disc.gsfc.nasa.gov/datasets/NLDAS_FORA0125_M_2.0/summary?keywords=NLDAS)
- Humidité des sols de la mission [NASA Soil Moisture Active Passive](https://nsidc.org/data/spl3smp/versions/8)

Remerciements
----------------

Ce programme a été rendu possible grâce à une subvention du programme de formation Transition to Open Science (TOPS) de la NASA (80NSSC23K0864), faisant partie du [programme TOPS de la NASA](https://nasa.github.io/Transform-to-Open-Science/)
