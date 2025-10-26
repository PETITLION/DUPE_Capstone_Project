# Credit Card Fraud Detection - Machine Learning Project

## Overview
Ce projet vise à développer un système intelligent de détection de fraude par carte de crédit à partir de données transactionnelles réelles.
L’objectif est de prédire automatiquement les transactions potentiellement frauduleuses tout en minimisant les fausses alertes, pour préserver l’expérience client.

## Objectifs du projet
    •	Prétraiter et nettoyer un large volume de données transactionnelles.
    •	Explorer et comprendre les comportements normaux vs frauduleux.
    •	Concevoir des features comportementales et temporelles pertinentes.
    •	Implémenter et comparer plusieurs modèles de classification supervisée.
    •	Optimiser les modèles en tenant compte du déséquilibre massif des classes (fraudes très rares).
    •	Fournir des recommandations exploitables en contexte réel (banque, fintech, sécurité).

## Contenu du projet
Fichier non technique / Dossier	Description
notebooks/	Contient les notebooks Jupyter (EDA, Feature Engineering, Modélisation)
data/	Données sources
models/	Sauvegarde potentielle des modèles entraînés
README.md	Ce fichier

## Modèles testés
    •	✅ Régression Logistique (baseline)
    •	✅ DecisionTree
    •	✅ Random Forest Classifier
    •	✅ XGBoost Classifier (meilleure performance observée)
    •	✅ KNN et modèles hybrides (en validation)

## Résultats principaux
Modèle	AUC	Précision	Rappel (fraude détectée)
  Logistic Regression	    ~0.92	    ~0.78	    ~0.81
  Random Forest	          ~0.95	    0.93	    0.84
  XGBoost	                0.971	    0.91	    0.88
  
  ✅ Les modèles optimisés atteignent un équilibre optimal entre sécurité et faux positifs
  
  ✅ Les features comportementales (montant vs historique carte, séquence temporelle, jour/heure) ont eu un impact majeur

## Technologies utilisées
    •	Python 3.x
    •	pandas, numpy, matplotlib, seaborn
    •	scikit-learn
    •	xgboost
    •	imbalanced-learn
    •	jupyter notebook
    •	knn
    •	...
    
## Prochaines améliorations
    •	Intégration d’un système de mise à jour automatique du modèle (apprentissage continu)
    •	Déploiement sous forme d’API REST pour détection en temps réel
    •	Dashboard interactif (Streamlit ou Dash) pour monitoring opérationnel

## Auteurs
Projet réalisé par :
        DUVERSEAU Jeff Lwear et PETIOTE Lionel - dans le cadre d’un projet de fin d’études en Data Science / IA.
