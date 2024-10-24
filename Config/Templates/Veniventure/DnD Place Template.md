---
tags: DnD/Location
world: Veniventure
type: Place
subtype: 
location: 
wiki: ""
description: ""
---

# <% tp.file.title %>

## Summary

- <% tp.file.cursor() %>

## Factions


```dataview
TABLE description AS "Description", subtype as "Type" 
FROM ("DnD/Veniventure" AND #DnD/Faction)
WHERE type = "Faction" AND contains(location,"<% tp.file.title %>")
SORT file.name
```
## Places

```dataview
TABLE description AS "Description", subtype as "Type" 
FROM ("DnD/Veniventure" AND #DnD/Location)
WHERE type = "Place" AND contains(location,"<% tp.file.title %>")
SORT file.name
```

## Shops

```dataview
TABLE owner AS "Owner", shop-type as "Type" 
FROM ("DnD/Veniventure" AND #DnD/Location)
WHERE type = "Shop" AND contains(location,"<% tp.file.title %>")
SORT file.name
```

## People

```dataview
TABLE description AS "Description"
FROM ("DnD/Veniventure" AND #DnD/NPC)
WHERE type = "NPC" AND contains(location,"<% tp.file.title %>")
SORT file.name
```