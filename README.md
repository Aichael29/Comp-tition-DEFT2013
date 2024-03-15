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

### Analyse des Résultats
#### Baseline vs Modèle SVM:

La baseline a prédit uniquement la classe majoritaire (Plat principal), aboutissant à une précision de 46%, reflétant la distribution déséquilibrée des classes. Ce résultat était attendu et sert de point de départ pour évaluer l'efficacité d'autres modèles.
Le modèle SVM, utilisant la vectorisation TF-IDF, a significativement surperformé la baseline avec une précision globale d'environ 86% sur les ensembles de validation et de test. Cela indique une forte capacité à distinguer entre les catégories de recettes.
#### Performances Détailées
Dessert: Exceptionnellement bien classé par le modèle SVM, avec presque 98% de précision sur l'ensemble de test, indiquant une excellente identification des caractéristiques spécifiques des desserts.
Entrée et Plat principal: Performances solides mais légèrement inférieures à celle des desserts, avec une précision d'environ 75-84%. Cela peut suggérer une plus grande difficulté à différencier ces catégories, possiblement à cause de chevauchements dans le vocabulaire utilisé.
#### Implications
La performance élevée du modèle SVM montre l'efficacité de la vectorisation TF-IDF pour transformer le texte en caractéristiques utiles à la classification, et le potentiel du SVM pour traiter ces caractéristiques. Cela démontre aussi l'importance de choisir des méthodes de prétraitement et des modèles adaptés à la nature des données et à la tâche spécifique.

## Conclusion

Les résultats montrent une nette amélioration dans la classification des recettes de cuisine à travers l'utilisation de modèles avancés comme SVM et RNN par rapport à un modèle de base.

