# FrostPVP Reborn 4.1.2-beta1 — Grace Period

## Added
- `/frost grace` (OP-only): starts one server-wide 30-minute PvP grace period.
- `/frost grace stop` (OP-only) and `/frost grace status` (any player).
- A blue boss bar shows the time remaining and announces that PvP is disabled.
- Every player online at grace start gets 16 cooked beef. Players joining late also receive 16 once per grace period.
- Big start title + Ender Dragon growl sound for each online player.
- PvP protection includes melee, projectiles, player-owned explosives, tameable mobs, Frost summons, thrown splash potions and lingering potion clouds.
- Frost active abilities cannot target other players while grace is active.
- `plugins/FrostPVP/grace.yml` stores the finish timestamp and UUID food records; grace continues after a server restart, without repeating food grants.

## Notes
- Starting `/frost grace` while a grace period is active does not reset it.
- Only the grace-period feature changed; existing weapons, events, and resource-pack style IDs are preserved.
- A successful Paper 1.21.11 compile and live server testing have **not** been performed in this environment. Build with GitHub Actions and test on a separate server first.
