---
tags: DnD/Location
world: Veniventure
type: Place
subtype: Continent
location: Toril
wiki: https://forgottenrealms.fandom.com/wiki/Faer%C3%BBn
description: Continente del Planeta Toril
---

# Faerûn

## Summary

- Uno de los principales continentes del planeta Toril.

## Factions

```dataview
TABLE description AS "Description", subtype as "Type" 
FROM ("DnD/Veniventure" AND #DnD/Faction)
WHERE type = "Faction" AND contains(location,"Faerûn")
SORT file.name
```
## Places

```dataview
TABLE description AS "Description", subtype as "Type" 
FROM ("DnD/Veniventure" AND #DnD/Location)
WHERE type = "Place" AND contains(location,"Faerûn")
SORT file.name
```

## Shops

```dataview
TABLE description AS "Description", subtype as "Type" 
FROM ("DnD/Veniventure" AND #DnD/Location)
WHERE type = "Shop" AND contains(location,"Faerûn")
SORT file.name
```

## People

```dataview
TABLE description AS "Description"
FROM ("DnD/Veniventure" AND #DnD/NPC)
WHERE type = "NPC" AND contains(location,"Faerûn")
SORT file.name
```