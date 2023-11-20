# Tchatche - Hack A Tech Bordeaux, 15-17 Novembre 2023

## À Propos du Projet
"Tchatche" est un projet novateur développé lors du Hack A Tech de Bordeaux, ayant pour objectif d'explorer les frontières de l'analyse audio et de la prédiction de notes basées sur des extraits de discours. Ce projet multidisciplinaire combine des techniques avancées de machine learning et de traitement du langage naturel pour évaluer des discours sur une échelle de 1 à 10.

## Exploration Scientifique
Nous avons abordé ce défi avec une approche exploratoire, testant un large éventail de méthodes et d'algorithmes :

- **Machine Learning Classique** : Utilisation de modèles tels que XGBoost, KNN, CatBoost, etc., en extrayant des features des MFCCs (moyenne, variance, médiane, mode, maximum, minimum, etc.).
- **Features de wav2vec 2.0** : Extraction de features profondes à partir de wav2vec 2.0, un modèle de transformation de l'audio en représentations utiles pour la prédiction.
- **Intégration avec ReservoirPy** : Expérimentation avec ReservoirPy pour améliorer la prédiction en utilisant les features de wav2vec 2.0.
- **Transcription Audio avec Whisper** : Tentatives d'utiliser Whisper pour la transcription audio, combinées à Mistral (un modèle de langage à grande échelle) pour l'analyse sémantique.

### Défis Rencontrés
Notre principal défi a été de trouver des features audio corrélées de manière significative avec les notes attribuées. Après plusieurs essais, les meilleurs résultats de corrélation ont été obtenus avec les features extraites de wav2vec 2.0.

## Ressources et Notebooks
L'ensemble de nos tentatives, expériences et résultats sont documentés dans divers notebooks Jupyter (`.ipynb`) disponibles dans ce dépôt.

## Installation et Utilisation
Pour reproduire nos expériences ou explorer nos modèles :

1. **Cloner le Dépôt** :
   ```
   git clone git@github.com:Naowak/HackATech-Tchatche.git
   ```
2. **Créer un Environnement Virtuel** (recommandé) :
   ```
   python -m venv env
   source env/bin/activate  # Sur Windows utilisez 'env\Scripts\activate'
   ```

## Licence
Ce projet est distribué sous la licence MIT. Pour plus de détails, voir le fichier `LICENSE`.

## Citation
Si ce travail vous inspire ou contribue à vos propres recherches, nous apprécierions une citation de notre projet.

## Partenaire du Projet
Ce projet a été porté par [StudioVR](https://studiovr.ai) lors du hackathon.
