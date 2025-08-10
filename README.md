# Prédiction de commandes robotiques avec MLP et LSTM (Imitation Learning)
Ce projet démontre comment prédire les commandes de déplacement d’un bras robotique à partir de ses états observés, en utilisant des données de démonstrations issues de RoboTurk.
Deux approches sont explorées :

* MLP (Multi-Layer Perceptron) : modèle simple, sans mémoire temporelle
* LSTM (Long Short-Term Memory) : modèle séquentiel capable de capturer les dépendances temporelles

L’objectif est de fournir une base pédagogique pour comprendre la préparation des données, la mise en place d’architectures et l’évaluation dans un contexte d’imitation learning.

## Contenu du projet

* notebook.ipynb → Code complet du prétraitement, de l’entraînement et de l’évaluation (exécuté sous Google Colab)
* Exploration du dataset : lecture et analyse du fichier demo.hdf5 de la tâche bins-Milk
* Implémentation MLP : entraînement sur états bruts
* Implémentation LSTM : prise en compte des séquences temporelles
* Visualisation : comparaison des trajectoires prédites et réelles en 3D
