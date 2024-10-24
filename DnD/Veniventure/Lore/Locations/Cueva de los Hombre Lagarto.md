---
tags:
  - DnD/Location
world: Veniventure
type: Place
subtype: Settlement
location:
  - Saltmarch
  - Pantanos de Marshwater
wiki: ""
description: Sistema de Cavernas en los Pantanos al Norte de Saltmarch
---

# Cueva de los Hombre Lagarto

## Summary

- Sistema de cuevas, cavernas y túneles donde habitan los [[Hombre Lagarto]]
- Se encuentra en lo profundo de los [[Pantanos de Marshwater]], al Norte de [[Saltmarch]]

## Factions


```dataview
TABLE description AS "Description", subtype as "Type" 
FROM ("DnD/Veniventure" AND #DnD/Faction)
WHERE type = "Faction" AND contains(location,"Cueva de los Hombre Lagarto")
SORT file.name
```
## Places

```dataview
TABLE description AS "Description", subtype as "Type" 
FROM ("DnD/Veniventure" AND #DnD/Location)
WHERE type = "Place" AND contains(location,"Cueva de los Hombre Lagarto")
SORT file.name
```

## Shops

```dataview
TABLE owner AS "Owner", shop-type as "Type" 
FROM ("DnD/Veniventure" AND #DnD/Location)
WHERE type = "Shop" AND contains(location,"Cueva de los Hombre Lagarto")
SORT file.name
```

## People

```dataview
TABLE description AS "Description"
FROM ("DnD/Veniventure" AND #DnD/NPC)
WHERE type = "NPC" AND contains(location,"Cueva de los Hombre Lagarto")
SORT file.name
```