# sentiments-analysis-using-machine-and-deep-learning-models-and-BERT
This project focuses on sentiment analysis by leveraging both traditional machine learning models and advanced deep learning techniques, including BERT. Our approach combines multiple algorithms to achieve high accuracy in understanding and predicting sentiment from text data, with BERT achieving an accuracy of 95%.
Structure du Projet
Le projet est structuré comme suit :

datasets/ : Contient les jeux de données utilisés pour l'analyse.
notebooks/ : Contient les notebooks Jupyter pour le traitement et l'analyse des données.
models/ : Contient les modèles entraînés et les scripts pour leur utilisation.
src/ : Contient les scripts de traitement des données et les implémentations des modèles.
README.md : Ce fichier.
Méthodologie
Jeux de Données
Nous avons utilisé un ensemble de données contenant des commentaires des clients sur divers produits disponibles sur Amazon. Les données sont collectées et fusionnées à partir de différentes catégories pour garantir une diversité et une représentativité adéquates.

Structure des Données :

product_title : Titre du produit évalué.
product_category : Catégorie du produit.
star_rating : Note attribuée par le client (1 à 5 étoiles).
helpful_votes : Nombre de votes jugés utiles pour l'avis donné.
review_body : Texte intégral de l'avis laissé par le client.
normalized_review_body : Texte de l'avis après normalisation.
review_body_compound_score : Score composite attribué au texte de l'avis basé sur une analyse de sentiments.
review_body_sentiment_label : Étiquette de sentiment attribuée à l'avis (positif, neutre, négatif).
Prétraitement des Données
Les étapes de prétraitement incluent :

Conversion en minuscules : Assure une uniformité accrue.
Suppression des mentions, hashtags et URL : Élimine le bruit inutile.
Élimination des emojis : Simplifie le texte.
Remplacement des caractères spéciaux : Maintient la cohérence du texte.
Suppression des chiffres : Se concentre sur le contenu textuel pertinent.
Tokenisation : Divise le texte en tokens.
Padding des séquences : Uniformise la longueur des séquences.
Vectorisation : Utilise la méthode TF-IDF pour convertir le texte en représentations numériques.
Modèles Utilisés
Modèles de Machine Learning Classiques
Régression Logistique : Utilisée pour la classification binaire et multi-classe.
Support Vector Classifier (SVC) : Utilise un noyau linéaire pour séparer les classes.
Gradient Boosting Classifier : Combine des arbres de décision pour améliorer la précision des prédictions.
Modèles de Deep Learning
LSTM (Long Short-Term Memory) : Capture les dépendances à long terme dans les données séquentielles, crucial pour l'analyse des sentiments.
