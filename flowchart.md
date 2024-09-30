```mermaid
flowchart TD
Start(Game start) --> enemy([Player spots enemy])
Start --> chest([Player spots chest])
death --> Restart([Game restart])
demise --> Restart
loot --> Restart
enemy([Player spots enemy]) --> melee([Player melee attack])
melee --> hit([Player does damage])
melee --> miss([Player misses])
miss --> demise([Player dies])
hit --> death([Enemy dies])
enemy --> spell([Player casts a spell])
spell --> hit
spell --> miss
chest --> normal([Normal chest])
chest --> evil([Evil chest])
evil --> demise
normal --> loot([cool loot])
```

# Dungeon Crawler Feedback Loop
