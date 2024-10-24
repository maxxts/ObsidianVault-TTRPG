---
tags:
  - DnD/Location
world: Veniventure
type: Place
subtype: Landmark
location:
  - Saltmarch
wiki: ""
description: Pantanos al Norte de Saltmarch
---

# Pantanos de Marshwater

## Summary

- Zona pantanosa al Norte de [[Saltmarch]]
- Es habitada por una gran variedad de razas anfibias.

## Factions


```dataview
TABLE description AS "Description", subtype as "Type" 
FROM ("DnD/Veniventure" AND #DnD/Faction)
WHERE type = "Faction" AND contains(location,"Pantanos de Marshwater")
SORT file.name
```
## Places

```dataview
TABLE description AS "Description", subtype as "Type" 
FROM ("DnD/Veniventure" AND #DnD/Location)
WHERE type = "Place" AND contains(location,"Pantanos de Marshwater")
SORT file.name
```

## Shops

```dataview
TABLE owner AS "Owner", shop-type as "Type" 
FROM ("DnD/Veniventure" AND #DnD/Location)
WHERE type = "Shop" AND contains(location,"Pantanos de Saltmarch")
SORT file.name
```

## People

```dataview
TABLE description AS "Description"
FROM ("DnD/Veniventure" AND #DnD/NPC)
WHERE type = "NPC" AND contains(location,"Pantanos de Marshwater")
SORT file.name
```