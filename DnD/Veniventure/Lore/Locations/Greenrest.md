---
tags:
  - DnD/Location
world: Veniventure
type: Place
subtype: Settlement
location:
  - Faerûn
  - Greenfields
  - Western Heartlands
wiki: https://forgottenrealms.fandom.com/wiki/Greenest
description: Asentamiento gobernado por Nightfield
---

# Greenrest

## Summary

- Único asentamiento en la region de Greenfield, dentro del continente de [[Faerûn]]
- Gobernado por [[Tarbaw Nightfield]]
- Founded by half-dwarf (Darvas Estra-something)

## Factions

```dataview
TABLE description AS "Description", subtype as "Type" 
FROM ("DnD/Veniventure" AND #DnD/Faction)
WHERE type = "Faction" AND contains(location,"Greenrest")
SORT file.name
```
## Places

```dataview
TABLE description AS "Description", subtype as "Type" 
FROM ("DnD/Veniventure" AND #DnD/Location)
WHERE type = "Place" AND contains(location,"Greenrest")
SORT file.name
```

## Shops

```dataview
TABLE owner AS "Owner", subtype as "Type" 
FROM ("DnD/Veniventure" AND #DnD/Location)
WHERE type = "Shop" AND contains(location,"Greenrest")
SORT file.name
```

## People

```dataview
TABLE description AS "Description"
FROM ("DnD/Veniventure" AND #DnD/NPC)
WHERE type = "NPC" AND contains(location,"Greenrest")
SORT file.name
```