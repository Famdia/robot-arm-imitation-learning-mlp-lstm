# Prédiction de commandes robotiques avec MLP et LSTM (Imitation Learning)
Ce projet démontre comment prédire les commandes de déplacement d’un bras robotique à partir de ses états observés, en utilisant des données de démonstrations issues de RoboTurk.
Deux approches sont explorées :

* MLP (Multi-Layer Perceptron) : modèle simple, sans mémoire temporelle
* LSTM (Long Short-Term Memory) : modèle séquentiel capable de capturer les dépendances temporelles

L’objectif est de fournir une base pédagogique pour comprendre la préparation des données, la mise en place d’architectures et l’évaluation dans un contexte d’imitation learning.

## Contenu du projet

* Robotique.ipynb → Code complet du prétraitement, de l’entraînement et de l’évaluation (exécuté sous Google Colab)
* Exploration du dataset : lecture et analyse du fichier demo.hdf5 de la tâche bins-Milk
* Implémentation MLP : entraînement sur états bruts
* Implémentation LSTM : prise en compte des séquences temporelles
* Visualisation : comparaison des trajectoires prédites et réelles en 3D

## Résultats

Les résultats actuels montrent qu’il reste une marge d’amélioration importante.
Mais, le but de ce projet est de servir de point de départ : vous pouvez tenter d’optimiser l’architecture, la taille des séquences, ou les hyperparamètres pour obtenir de meilleures performances.

## Comment utiliser

1. Cloner le dépôt
`git clone https://github.com/Famdia/robot-arm-imitation-learning-mlp-lstm.git
`
2. Télécharger les données RoboTurk (sur ce notebook, vous travaillerez sur tâche bins-Milk) disponible ici → https://roboturk.stanford.edu/
3. Ouvrir le notebook sur Google Colab ou localement
4. Modifier le  chemin d'accès au dataset que vous venez de télécharger
5. Exécuter le notebook pour reproduire les résultats

## Améliorations possibles

* Utiliser DAgger (Dataset Aggregation) pour collecter de nouvelles démonstrations interactives
* Intégrer la vision par ordinateur pour exploiter les images de la simulation
* Augmenter la taille des séquences pour capturer plus de contexte temporel
* Tester des modèles transformers pour séries temporelles
