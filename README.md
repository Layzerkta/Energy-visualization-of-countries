# Analyse et Visualisation de la Consommation d'énergie Mondiale

Ce projet Python permet d'explorer et de visualiser la consommation d'énergie mondiale à travers des graphiques interactifs et des analyses statistiques. Le code est organisé en plusieurs sections pour réaliser des visualisations, extraire des indicateurs-clés et effectuer du clustering sur les énergies renouvelables.

## Prérequis

Assurez-vous d'avoir les bibliothèques Python suivantes installées :

- `pandas`
- `numpy`
- `plotly`
- `matplotlib`
- `scipy`
- `scikit-learn`

## Contenu du Projet

### 1. Préparation des Données

- Chargement des données à partir du fichier CSV : `World Energy Consumption.csv`.
- Sélection des colonnes pertinentes :
  - Exemple : `biofuel_consumption`, `coal_consumption`, `renewables_consumption`, etc.
- Nettoyage des données :
  - Suppression des lignes où le pays est égal à "World".
  - Remplacement des valeurs manquantes par `0`.

### 2. Visualisations Interactives

Deux graphiques principaux sont générés :

1. **Graphique Principal** :
   - Représente la consommation d'énergie par type pour chaque pays entre les années disponibles.
   - Des menus interactifs permettent de sélectionner le type d'énergie affiché (par exemple : biocarburants, énergie solaire, énergie éolienne).

2. **Carte Interactive** :
   - Affiche la consommation d'énergie par type sur une carte mondiale pour l'année 2020.
   - Les couleurs varient en fonction de la consommation (en TWh).

Les deux visualisations sont exportées en fichiers HTML nommés `energy_main.html` et `energy_map.html` respectivement.

### 3. Analyses Statistiques

#### a) Consommation Maximale de Biocarburant par Habitant

- Extraction de la consommation maximale de biocarburant par habitant pour chaque pays.
- Permet d'identifier les leaders en matière de consommation de biocarburant.

#### b) Scores Z pour la Demande d'Électricité

- Standardisation de la demande en électricité pour détecter les anomalies.
- Calcul des scores Z pour comparer les pays sur une base équivalente.

#### c) Évolution Temporelle de la Demande en Électricité

- Analyse des variations annuelles en pourcentage.
- Exemple d'observation : baisse de -31,67 % en 2022, probablement due à des événements globaux.

#### d) Clustering des Énergies Renouvelables

- Regroupement des pays en fonction de la consommation moyenne d'énergie renouvelable et de leur part dans le mix énergétique.
- Visualisation des clusters sur un graphique pour une interprétation aisée.

## Screenshots

Voici des exemples de visualisations générées :

### Graphique Principal

![Graphique Principal](screenshots/graphique_principal.png)

### Carte Interactive

![Carte Interactive](screenshots/carte_interactive.png)

### Clustering des Énergies Renouvelables

![Clustering](screenshots/clustering.png)

## Instructions

1. Exécutez le fichier notebook dans un environnement Python approprié.
2. Les fichiers HTML générés peuvent être ouverts dans n'importe quel navigateur.
3. Utilisez les menus déroulants pour explorer les différents types d'énergie.

## Conclusion

Ce projet offre une compréhension approfondie des tendances et modèles dans la consommation d'énergie mondiale. Il est particulièrement utile pour les chercheurs, analystes et décideurs politiques souhaitant promouvoir l'adoption des énergies renouvelables.

