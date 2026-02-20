# Guide utilisateur  
## Sources de données – TADAO

Ce module présente les différentes sources de données utilisées dans les projets SIG du réseau TADAO (Artois Mobilités).

Chaque section correspond à un onglet du site.

---

# La page des projets  
## Base GTFS (General Transit Feed Specification)

### Description
La base GTFS constitue la donnée principale du réseau de transport.  
Elle contient :

- routes.txt → lignes commerciales
- stops.txt → arrêts
- trips.txt → trajets
- stop_times.txt → horaires théoriques
- calendar.txt → jours de circulation

### Format
Fichiers texte normalisés (.txt) regroupés dans une archive .zip.

### Utilisation chez TADAO
- Cartographie des lignes
- Analyse d’accessibilité
- Étude des correspondances
- Intégration dans QGIS / PostGIS
- Développement d’applications web mobilité

### Mise à jour
À chaque modification d’offre (nouvelle ligne, ajustement horaire).

---

# L’authentification  
## Données OpenStreetMap (OSM)

### Description
Base de données géographique collaborative mondiale utilisée comme fond cartographique et réseau viaire.

### Contenu exploité
- Voirie
- Bâtiments
- Points d’intérêt
- Réseau cyclable
- Réseau piéton

### Format
- .osm
- .pbf
- Export en Shapefile ou GeoJSON

### Utilisation chez TADAO
- Fond cartographique web
- Calcul d’itinéraires
- Analyse réseau
- Isochrones
- Croisement avec les tracés GTFS

### Source
https://www.openstreetmap.org

---

# Une carte simple  
## Données IGN (BD TOPO / BD ORTHO)

### Description
Données de référence produites par l’Institut national de l’information géographique et forestière.

### Contenu exploité
- Réseau routier structuré
- Bâtiments précis
- Limites administratives
- Orthophotographies

### Format
- Shapefile
- GeoPackage
- WMS / WFS

### Utilisation chez TADAO
- Référentiel officiel
- Production cartographique institutionnelle
- Vérification qualité OSM
- Support aux études territoriales

---

# Analyse avancée  
## Données internes TADAO

### Description
Données produites par l’exploitation et le service mobilité.

### Contenu exploité
- Tracés réels des lignes
- Localisation terrain des arrêts
- Données de fréquentation
- Données billettiques
- Statistiques d’exploitation

### Format
- CSV
- Excel
- Base PostgreSQL/PostGIS

### Utilisation
- Analyse de performance réseau
- Optimisation des itinéraires
- Tableaux de bord décisionnels

### Sensibilité
Données internes – diffusion restreinte.

---

# Base technique  
## Modèle PostGIS

### Description
Base de données spatiale centralisée.

### Technologies
- PostgreSQL
- PostGIS
- Requêtes SQL spatiales

### Utilisation
- Stockage des couches SIG
- Jointures spatiales
- Backend d’applications cartographiques
- Scripts Python automatisés

---

# Architecture du menu

Guide utilisateur  
├── La page des projets → GTFS  
├── L’authentification → OpenStreetMap  
├── Une carte simple → IGN  
├── Analyse avancée → Données internes  
└── Base technique → PostGIS  

---

Service géomatique – TADAO  
Technicien / Chef de projet en géomatique