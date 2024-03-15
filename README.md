# Tâche 2 DEFT2013 : 10

El felchaoui aicha - DS

## Vue d'ensemble

Ce projet concerne la classification automatique de recettes de cuisine en trois catégories : Entrée, Plat principal, ou Dessert. Il s'inscrit dans le cadre de la compétition DEFT2013 Tâche 2.

## Dataset

Le dataset contient 12 473 recettes, réparties comme suit :

### Distribution des Catégories

| Catégorie      | Proportion (%) |
|----------------|----------------|
| Plat principal | 46.52          |
| Dessert        | 30.16          |
| Entrée         | 23.32          |

## Méthodologie

Différents modèles de machine learning ont été évalués pour classer les recettes.

## Résultats

### Modèle de Base

- **Accuracy**: 0.46
- **Precision (Plat principal)**: 0.46
- **Recall (Plat principal)**: 1.00
- **F1-score (Plat principal)**: 0.63

### Naive Bayes

- **Accuracy**: 0.81
- **Precision moyenne**: 0.81
- **Recall moyen**: 0.79
- **F1-score moyen**: 0.79

### Régression Logistique

- **Accuracy**: 0.83
- **Precision moyenne**: 0.82
- **Recall moyen**: 0.81
- **F1-score moyen**: 0.81

### Forêt Aléatoire

- **Accuracy**: 0.78
- **Precision moyenne**: 0.78
- **Recall moyen**: 0.74
- **F1-score moyen**: 0.75

### SVM (Support Vector Machine)

- **Accuracy**: 0.82
- **Precision moyenne**: 0.81
- **Recall moyen**: 0.80
- **F1-score moyen**: 0.81

### RNN

- **Accuracy**: 0.826
- **Precision moyenne**: 0.818
- **Recall moyen**: 0.813
- **F1-score moyen**: 0.815

### SVM (Amélioré)

- **Accuracy**: 0.86
- **Precision moyenne**: 0.86
- **Recall moyen**: 0.84
- **F1-score moyen**: 0.85
- **Précision micro-moyenne**: 0.861

## Conclusion

Les résultats montrent une nette amélioration dans la classification des recettes de cuisine à travers l'utilisation de modèles avancés comme SVM et RNN par rapport à un modèle de base.

