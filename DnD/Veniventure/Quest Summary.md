---
world: Veniventure
---

< [[World of Veniventure]]
# Quest Summary
<small>Dashboard dedicado a las sesiones de Veniventure.</small>

## Quests
### Tracked Quests

```dataview
TASK
FROM "DnD/Veniventure/Quests" AND #Dnd/Quest
WHERE !completed and world = "Veniventure"
GROUP BY file.link
```

### Untracked Quests and Questions
<small>Objetivos menores definidos en sesiones</small>

```dataview
TASK
FROM "DnD/Veniventure/Sessions"
WHERE !completed and world = "Veniventure"
GROUP BY file.link
```

### Completed

```dataview
TASK
FROM !"Config/Veniventure/Templates" AND ("DnD/Quests" OR #Dnd/Quest)
WHERE completed and world = "Veniventure"
GROUP BY file.link
```
