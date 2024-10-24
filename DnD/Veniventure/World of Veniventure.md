---
tags: DnD/World
world: Veniventure
---
< [[Dungeons and Dragons]]
# World of Veniventure

## Player Characters

- [[Tulion]]
- [[Miguelios]]
- [[Barr-Barron]]
- [[Van Lumen]]
- [[Dror]]

## Quests

- Go to [[Quest Summary]]

## Last Sessions

```dataview
TABLE summary AS "Summary", dateformat(created, "DDDD") AS "Date"
FROM "DnD/Veniventure/Sessions"
WHERE world = "Veniventure"
SORT file.name DESC
```

## Places

## Factions

## Pending Organization

```dataview
TABLE campaign AS "Campaign", dateformat(file.ctime, "DDDD") AS "Date"
FROM "DnD/Veniventure/Sessions" AND !#DnD/Session
SORT file.ctime DESC
LIMIT 5
```

## Items Recap

```dataview
TABLE WITHOUT ID string(link(rows.file.link, rows.title)[0]) AS 
"Session", regexreplace(list(rows.L.text), "#DnD/Item", "") AS "Item"
FROM "DnD/Veniventure/Sessions"
FLATTEN file.lists AS L
WHERE contains(L.tags, "#DnD/Item")
GROUP BY file.link
```

## Changelog

- [ ] Obsidian Cleanup #TODO
	- [ ] Decide if this should be considered a 'world' or a 'campaign'
	- [ ] Is it worth it to show a list of places/factions here? If so, which ones?
	- [ ] Test Tag Summary and [Colored Tags](obsidian://show-plugin?id=colored-tags) Plugins





















