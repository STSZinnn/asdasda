# FrostPVP Reborn v4.1.3-beta1 — dropped-item performance safeguard

- Optimized Chosen One relic cleanup: records only relic entities created during the active event instead of scanning every item entity in every loaded world when the event ends or the relic changes ownership.
- Tracks relic entities through ItemSpawnEvent and cleans tracking on pickup/despawn.
- Preserves all v4.1.2 grace-period features, weapon abilities, armor, commands, and resource-pack styles.
- This removes a potentially expensive source of lag. It does not prove that this code was responsible for the reported spike when dropping arbitrary items. Use Paper's built-in spark profiler to establish the exact source if the lag persists.
- Build is NOT compiled or tested on a live Paper server in this environment.
