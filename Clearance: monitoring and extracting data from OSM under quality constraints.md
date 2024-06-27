---
title: 2024 - Clearance, contrôler collaborativement des données OpenStreetMap pour des usages thématiques 
css: 'style.css'
---

# Clearance
## contrôler collaborativement des données OpenStreetMap pour des usages thématiques 

## SotM FR 2024

- Vincent Bergeot - v.bergeot@teritorio.fr
- Frédéric Rodrigo - f.rodrigo@teritorio.fr

[Teritorio](https://www.teritorio.fr/)

---

## Contexte

Besoins
- Exposer et diffuser des données OSM
  - site web, carte papier
- Qualité et responsabilité contenu
  - par ex. DAE

Souhait
- Contribuer à OSM
- Améliorer les données d'abord dans OSM
- Collaborer

---

# Clearance

----

## Projet Clearance

1 instance Clearance, plusieurs projets.

Un projet. Une communauté.
- Une zone
- Une thématique
- Règles de validation

Par ex : le tourisme, les stations ferroviaires, la randonnée …

----

### Clearance dans un projet

- formation dans les OT
- contributions pour arriver à un niveau accepté de qualité
- Clearance accompagne la montée en qualité des données OSM
- mise en ligne de la cartographie publique
- Clearance permet de maintenir la qualité des données OSM

----

### Des objets filtrés

- base *réputée juste* (un extract)
- les modifications (diff) arrivent
  - par défaut dans la base sauf sur la zone d'intérêt si
      - effacement d'objets
      - déplacement d'objets selon une distance personalisable
      - des attributs surveillés
      - des listes de contributeurs
- à chaque recalcul suite à des modifications (diff) les objets signalés sont réévalués

----

### Local Changeset (LoCha)

Regroupement de modifications faites localement (proximité géographique) :
- actuellement pour permettre une validation manuelle contextualisé
- ensuite pour avoir des validations automatiques sur des LoCha (un objet (node) effacé et recréé (way) avec les mêmes attributs, ...)

----

### validation manuelle

- validation collaborative par projet basé sur les comptes OSM
- les objets filtrés sont :
  - aggrégés (3 modifications faites dans OSM, cela passe de la version X à la version X+3)
  - contextualisés avec les LoCha,
  - filtrables selon le territoire, l'utilisateur, la date de modifications, les attributs
  - associés à des outils pour mieux comprendre les modifications,
  - liés à vos éditeurs préférés pour aller modifier OSM,
  - acceptés (individuellement ou par lots)

----

### une api "overpass" partielle

- la base "filtrée" en sortie de Clearance est interrogeable,
- des requêtes overpass peuvent être faites
  - [Présentation Underpass-API requêtes Overpass sur une base de données SQL Vendredi 17h salle 325](https://pretalx.com/sotm-fr-2024/talk/A3TRQ8/) ...)
- permet de garder les requêtes overpass en interrogeant une base "vérifiée",

---

## Clearance en prod

- ✅ Import / Export + diff
- ⌛ Jeux de règle de validation
- ⏳ Interface de contrôle et validation manuelle
- ⌛ Validation par LoCha

[Démo](https://clearance.teritorio.xyz/)

---

## Et la suite pour Clearance

- Les améliorations
    - l'interface, signalement RSS, ...
    - anotations sur les signalements (à mofifier, besoin d'aide, ...)
    - les LoCha,
    - les validations automatiques de LoCha
    - des règles de qualité pour valider automatiquement des objets (opening_hours, téléphone, https://, ...),
    - réputation des contributrices, contributeurs

---

## En savoir plus

- https://github.com/teritorio/clearance
- https://github.com/teritorio/clearance-frontend
- [State of the Map France 2023](https://peertube.openstreetmap.fr/w/7YynqrJXDzM9K1V9gKWCf7)
- [State of the Map Europe 2023](https://2023.stateofthemap.eu/program/clearance-monitoring-and-extracting-data-from-osm-under-quality-constraints)

---
