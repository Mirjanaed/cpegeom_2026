# Guide utilisateur  
## Sources de données – TADAO

Ce document présente les différentes sources de données utilisées dans le cadre des projets SIG et géomatiques du réseau TADAO (Artois Mobilités).

Chaque sous-section correspond à une source de données exploitable dans les projets cartographiques, analyses spatiales et applications web.

---

## 1. Base GTFS (General Transit Feed Specification)

### Description
La base GTFS contient l’ensemble des données théoriques du réseau de transport :
- Lignes
- Arrêts
- Horaires planifiés
- Calendriers de circulation
- Correspondances

### Format
- Fichiers texte (.txt)
- Structuration normalisée (stops.txt, routes.txt, trips.txt, stop_times.txt…)

### Usage
- Intégration dans SIG (QGIS / ArcGIS)
- Analyse d’accessibilité
- Cartographie des lignes
- Développement d’applications web de mobilité

### Fréquence de mise à jour
Selon les changements d’offre (nouveaux horaires, nouvelles lignes, adaptations saisonnières)

---

## 2. Données OpenStreetMap (OSM)

### Description
Base de données géographique collaborative utilisée pour :
- Voirie
- Bâtiments
- Points d’intérêt
- Réseau routier

### Format
- .osm
- .pbf
- Shapefile après extraction

### Usage
- Fond cartographique
- Analyse réseau (isochrones, calcul d’itinéraire)
- Croisement avec les lignes TADAO

### Source
https://www.openstreetmap.org

---

# 3. Données IGN (BD TOPO / BD ORTHO)

## Description
Données de référence produites par l’IGN :
- Réseau routier précis
- Bâtiments
- Limites administratives
- Orthophotographies

## Format
- Shapefile
- GeoPackage
- WMS/WFS

## Usage
- Référentiel spatial officiel
- Contrôle qualité des données OSM
- Production cartographique institutionnelle

## Producteur
Institut national de l'information géographique et forestière (IGN)

---

# 4. Données internes TADAO

## Description
Données produites en interne :
- Tracés réels des lignes
- Localisation des arrêts terrain
- Données d’exploitation
- Points de montée/descente
- Données billettiques (si accessibles)

## Format
- CSV
- Excel
- Base PostgreSQL/PostGIS
- Shapefile

## Usage
- Analyse de fréquentation
- Optimisation de lignes
- Études de performance réseau
- Tableaux de bord

## Sensibilité
Données internes – diffusion restreinte

---

# 5. Limites administratives (INSEE / IGN)

## Description
- Communes
- IRIS
- EPCI
- Découpages statistiques

## Format
- Shapefile
- GeoJSON

## Usage
- Analyse territoriale
- Études de couverture réseau
- Statistiques par commune

---

# 6. Données GPS / SAEIV

## Description
Données issues des véhicules :
- Position temps réel
- Retards
- Temps de parcours réel

## Format
- API
- Base SQL
- Flux temps réel

## Usage
- Analyse ponctualité
- Étude vitesse commerciale
- Optimisation exploitation
- Cartographie temps réel

---

# 7. Modèle de données PostGIS

## Description
Base de données spatiale centralisée utilisée pour :
- Stockage des couches SIG
- Jointures spatiales
- Requêtes SQL géographiques

## Technologies
- PostgreSQL
- PostGIS

## Usage
- Backend cartographique
- API géospatiale
- Traitement automatique Python

---

# Architecture du site

Guide utilisateur  
└── Sources de données TADAO  
    ├── GTFS  
    ├── OSM  
    ├── IGN  
    ├── Données internes  
    ├── Limites administratives  
    ├── GPS / SAEIV  
    └── PostGIS  

---

# Auteur

Service géomatique – TADAO  
Technicien / Chef de projet en géomatique