# Guide utilisateur  
## Sources de données – TADAO

Ce module présente les sources de données utilisées dans les projets géomatiques du réseau TADAO.

---



---

## Données extérieures  
### Données OpenStreetMap (OSM)

Base de données géographique collaborative.

**Contenu :**
- Voirie
- Bâtiments
- Points d’intérêt
- Réseaux piétons et cyclables

**Format :**
- .osm
- .pbf
- GeoJSON / Shapefile

**Utilisation :**
- Fond cartographique
- Analyse réseau
- Calcul d’itinéraires
- Croisement GTFS

---

## Une carte simple  
### Données IGN (BD TOPO / BD ORTHO)

Référentiel géographique national.

**Contenu :**
- Réseau routier structuré
- Bâtiments
- Limites administratives
- Orthophotographies

**Format :**
- Shapefile
- GeoPackage
- Flux WMS / WFS

**Utilisation :**
- Production cartographique officielle
- Vérification qualité
- Études territoriales

---

## Analyse avancée  
### Données internes TADAO

Données produites par l’exploitation et le service mobilité.

**Contenu :**
- Tracés réels des lignes
- Localisation terrain des arrêts
- Données de fréquentation
- Statistiques d’exploitation

**Format :**
- CSV
- Excel
- Base PostgreSQL/PostGIS

**Utilisation :**
- Analyse performance réseau
- Optimisation des lignes
- Tableaux de bord décisionnels

---

## Carte temps réel  
### Données GPS / SAEIV

Données issues du système d’aide à l’exploitation.

**Contenu :**
- Position des véhicules
- Retards
- Temps de parcours réel

**Format :**
- API
- Base SQL
- Flux temps réel

**Utilisation :**
- Analyse ponctualité
- Étude vitesse commerciale
- Visualisation dynamique

---

## Base technique  
### Base de données PostGIS

Base de données spatiale centralisée.

**Technologies :**
- PostgreSQL
- PostGIS
- Requêtes SQL spatiales

**Utilisation :**
- Stockage des couches SIG
- Jointures spatiales
- Backend cartographique
- Automatisation via scripts Python

---

Service géomatique – TADAO  
Technicien / Chef de projet en géomatique