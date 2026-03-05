| File | Domain |
|---|---|
| `Admin.txt` | Admin commands, cheat manager, RCON |
| `Bosses.txt` | Boss encounters and arena logic |
| `Chat.txt` | Chat messages, send modes, chat UI |
| `Combat.txt` | Damage, death, combat state |
| `Crafting.txt` | Crafting queues, engrams, stations |
| `DinoBreeding.txt` | Breeding, imprinting, gestation |
| `Dinos.txt` | Dino state, taming, orders, AI |
| `DinoStorage.txt` | Cryopod and dino storage systems |
| `Economy.txt` | Points, currency, shop interfaces |
| `Engine.txt` | Core UE engine symbols |
| `Equipment.txt` | Armor, saddles, worn items |
| `Inventory.txt` | Inventory containers, item transfer |
| `Items.txt` | Item definitions, net info, pickup |
| `Misc.txt` | Uncategorized or multi-domain symbols |
| `Mods.txt` | Mod framework, custom game mode hooks |
| `Networking.txt` | RPC, replication, connection lifecycle |
| `PlayerLifecycle.txt` | Spawn, death, respawn, session join |
| `PlayerMovement.txt` | Movement, velocity, input |
| `PlayerStats.txt` | Health, stamina, XP, level, attributes |
| `PlayerUI.txt` | HUD, widgets, menus, notifications |
| `Server.txt` | Server init, tick, game mode, settings |
| `Structures.txt` | Structure placement, decay, snap |
| `Tek.txt` | Tek tier items, suits, teleporters |
| `Tribe.txt` | Tribe creation, alliances, logs, ranks |
| `Vehicles.txt` | Boats, rafts, platform saddles |
| `World.txt` | Weather, time, world settings, zones |

---

Each file is a flat list of engine symbols extracted from the ASA binary. Use these as the lookup source when:

- Identifying which function to hook for a given feature
- Verifying a symbol exists before referencing it in plugin code
- Mapping a new plugin's scope to one or more categories

---

## Notes

- Symbols include functions, fields, delegates, exec wrappers, lambda captures, and parameter structs
- `Engine.txt` is the largest file (~23MB) and covers low-level UE internals
- All files reflect the ASA binary as of **February 2026**
