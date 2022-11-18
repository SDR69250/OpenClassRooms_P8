# OC Data Scientist - Projet 8 : Déployez un modèle dans le cloud

## Contexte & Mission

Une start-up de l'AgriTech, nommée  "Fruits!", souhaite proposer proposer des solutions innovantes pour la récolte des fruits.

Pour préserver la biodiversité l'entreprise veut développer des robots cueilleurs intelligents aux traitement spécifiques pour chaque espèce de fruits.
La première étape consiste à produire une appli qui permette de reconnaitre un fruit et de fournir des informations à partir d'une photo faite par l'utilisateur.
En partant d'un jeu de données constitué d'images de fruits et de labels associés, il faut construire une partie de la chaine de traitement des données (préprocessing et réduction de dimension).

Comme il s'agit de volumes de données importants et appelés à croitre, il faut développer dans un environnement Big Data pour pouvoir passer à l'échelle, mais sans entrainer de modèle pour le moment.

## Données

https://www.kaggle.com/moltean/fruits

## Contraintes
-  Le volume de données va augmenter très rapidement après la livraison de ce projet.
-  Les scripts seront développés en Pyspark et le cloud AWS sera utilisé pour profiter d’une architecture Big Data (EC2, S3, IAM), basée sur un serveur EC2 Linux.

## Livrables

1. Développement du modèle de classification
-  P8_01_notebook.ipynb : notebook sur le cloud contenant les scripts en Pyspark exécutables (le preprocessing et une étape de réduction de dimension, ici on utilise le modèle VGG16 sans la dernière couche)
2. P8_02_Images_Features : images du jeu de données initial (.jpg) ainsi que la sortie de la réduction de dimension (matrice .csv) toutes stockées sur AWS S3
3. Documentation projet :
-  P8_03_presentation.pdf : support de présentation