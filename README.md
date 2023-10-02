# TransportData

### 1. **Description des Données :**

- **Nom de Données** : TransportData
- **Description** : Ce jeu de données contient des enregistrements sur les transports publics.
- **Colonnes** : 
  - Date, TransportType, Route, DepartureTime, ArrivalTime, Passengers, DepartureStation, ArrivalStation, Delay
- **Types de Données** : 
  - Date, Chaîne de caractères, Chaîne de caractères, Heure, Heure, Entier, Chaîne de caractères, Chaîne de caractères, Entier
- **Exemples d'Enregistrements** : 

```
| Date       | TransportType | Route   | DepartureTime | ArrivalTime | Passengers | DepartureStation | ArrivalStation | Delay |
|------------|---------------|---------|---------------|-------------|------------|------------------|----------------|-------|
| 01/01/2023 | Train         | Route_5 | 7:38:00 AM    | 9:29:00 AM  | 98         | Station_14       | Station_15     | 0     |
| 01/01/2023 | Metro         | Route_2 | 8:47:00 AM    | 9:58:00 AM  | 65         | Station_8        | Station_4      | 7     |
... (autres enregistrements)
```

### 2. **Transformations :**

- **Nom de la Transformation** : Calcul de la durée du voyage.
- **Données d'Entrée** : Les données avec les colonnes DepartureTime et ArrivalTime.
- **Données de Sortie** : Les mêmes données avec une nouvelle colonne Duration.
- **Étapes de Transformation** : Utilisation de PySpark pour calculer la durée du voyage.

### 3. **Lignage des Données :**

- **Source des Données** : Données provenant de l'Agence de Transport inDATA.
- **Étapes de Traitement** : Lecture des données brutes, transformation à l'aide d'Azure Databricks.
- **Outils Utilisés** : Azure Databricks, PySpark, Azure Data Factory.

### 4. **Directives d'Utilisation :**

- **Cas d'Utilisation** : Analyse des retards et des tendances de passagers.
- **Directives d'Utilisation** : Utilisez ces données pour comprendre les flux de passagers et les retards des transports publics.
- **Précautions** : les retards sont catégorisés en groupes pour faciliter l'analyse.
