# AntiLogout

**Originally by samo_lego, maintained/modified by OBRONI312.**[cite: 1]

*If samo_lego does not want this fork to be public, I (OBRONI312) will take it down upon request.*[cite: 1]

---

## Overview

**AntiLogout** is a server-side mod that prevents players from escaping combat by logging out[cite: 1]. When a player logs out during combat, their "body" remains online for a configurable amount of time, making combat logging impossible[cite: 1]. The mod also provides a flexible `/afk` command to safely go AFK for farming or other purposes[cite: 1].

**Supported Minecraft version:** Fabric servers running Minecraft 26.3[cite: 1].

---

## Features

- Prevents combat logging: players who log out during combat remain in the world[cite: 1].
- `/afk` command: lets players logout with the account still online, with optional time limits[cite: 1].
- Configurable messages and timeouts[cite: 1].
- Permission-based command and feature access[cite: 1].

---

## Installation

1. Download the mod JAR and place it in your server's `mods` folder[cite: 1].
2. Start the server to generate the config file[cite: 1].
3. Edit `config/antilogout.toml` to customize settings[cite: 1].

---

## Configuration

All options are in `config/antilogout.toml`[cite: 1].

**Key options:**
- `disableAllLogouts`: Disable all logout protection features[cite: 1].
- `debug`: Enable debug logging[cite: 1].
- `afkMessage`: Message shown when a player is AFK[cite: 1].
- `afkCombatMessage`: Message shown if a player tries to go AFK while in combat[cite: 1].
- `afkBroadcastMessage`: Broadcast when a player goes AFK (`{player}` = name)[cite: 1].
- `combatEnterMessage`: Message when entering combat[cite: 1].
- `combatEndMessage`: Message when leaving combat[cite: 1].
- `combatTimeout`: How long a player is considered in combat (seconds)[cite: 1].
- `combatDisconnectMessage`: Message when a player disconnects during combat[cite: 1].

---

## Commands

- `/afk`  
  Set yourself AFK for the max time. (Permission level 0)[cite: 1]
- `/afk time <seconds>`  
  Set yourself AFK for a specific time (`-1` for unlimited). (Permission level 0)[cite: 1]
- `/afk players <targets> [time <seconds>]`  
  Set other players AFK. (Admin only, permission level 4)[cite: 1]
- `/antilogout reload`  
  Reload the config file. (Admin only, permission level 4)[cite: 1]
- `/antilogout status`  
  Show current config summary. (Admin only, permission level 4)[cite: 1]

---

## Permissions

- `antilogout.bypass.combat` — Bypass combat tagging[cite: 1].
- `antilogout.command.afk` — Use `/afk` (level 0)[cite: 1].
- `antilogout.command.afk.time` — Set AFK time for yourself (level 0)[cite: 1].
- `antilogout.command.afk.players` — Set other players AFK (admin only, level 4)[cite: 1].
- `antilogout.command.antilogout` — Use `/antilogout` admin commands (level 4)[cite: 1].
- `antilogout.command.antilogout.reload` — Reload config (level 4)[cite: 1].
- `antilogout.command.antilogout.edit` — Edit config in-game (if enabled, level 4)[cite: 1].

---

## Examples

**Combat log prevention:**  
Players who log out during combat remain in the world for the configured timeout[cite: 1].

**AFK farming:**  
Use `/afk` to safely go AFK for farming or other purposes[cite: 1].

---

## Video Showcase

- [Combat log prevention demo](https://user-images.githubusercontent.com/34912839/213432960-15d54218-8313-4470-868b-10eb78357764.mp4)[cite: 1]
- [AFK farming demo](https://user-images.githubusercontent.com/34912839/213676495-f3125d24-d42d-4ee9-80d2-55f33d313aae.mp4)[cite: 1]

---

For questions, suggestions, or issues, please open an issue on GitHub or contact OBRONI312[cite: 1].