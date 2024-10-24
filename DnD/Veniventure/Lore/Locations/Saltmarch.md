---
tags:
  - DnD/Location
world: Veniventure
type: Place
subtype: Settlement
location: Faerûn
wiki: ""
description: Puerto mercantil
---

# Saltmarch

## Summary

- Ciudad puerto, gobernada por el [[Consejo de Saltmarch]].
- Miguelios notó que no tiene mucha seguridad. 
- Solia ser parte del reino del norte

## Factions

```dataview
TABLE description AS "Description", subtype as "Type" 
FROM ("DnD/Veniventure" AND #DnD/Faction)
WHERE type = "Faction" AND contains(location,"Saltmarch")
SORT file.name
```

## Places

```dataview
TABLE description AS "Description", subtype as "Type" 
FROM ("DnD/Veniventure" AND #DnD/Location)
WHERE type = "Place" AND contains(location,"Saltmarch")
SORT file.name
```

## Shops

```dataview
TABLE owner AS "Owner", shop-type as "Type" 
FROM ("DnD/Veniventure" AND #DnD/Location)
WHERE type = "Shop" AND contains(location,"Saltmarch")
SORT file.name
```

## People

```dataview
TABLE description AS "Description"
FROM ("DnD/Veniventure" AND #DnD/NPC)
WHERE type = "NPC" AND contains(location,"Saltmarch")
SORT file.name
```