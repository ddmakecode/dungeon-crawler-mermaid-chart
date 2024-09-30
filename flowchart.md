```mermaid
flowchart TD
```

# Basic layout
```mermaid
Start(Game start) --> enemy([Player spots enemy])
Start --> chest([Player spots chest])
death --> Restart([Game restart])
demise --> Restart
loot --> Restart
```

# Player vs Enemy experience
# In this theoretical game, the Player and all enemies are one-hit (please never do this when making a dungeon crawler)
```mermaid
enemy([Player spots enemy]) --> melee([Player melee attack])
melee --> hit([Player does damage])
melee --> miss([Player misses])
miss --> demise([Player dies])
hit --> death([Enemy dies])
enemy --> spell([Player casts a spell])
spell --> hit
spell --> miss
```

# Evil chest (evil) leads to an Unfortunate fate
```mermaid
chest --> normal([Normal chest])
chest --> evil([Evil chest])
evil --> demise
normal --> loot([cool loot])
```
