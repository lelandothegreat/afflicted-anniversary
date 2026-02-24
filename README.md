# Afflicted

> Enemy spell and cooldown tracker for PvP. Built for **World of Warcraft: The Burning Crusade Anniversary** (BCC).

Track enemy interrupts, defensives, and key cooldowns in arenas and battlegrounds. See when spells are used, when they expire, and when they’re back up—so you know when it’s safe to cast or when to hold.

| | |
|---|---|
| **Game** | WoW TBC Anniversary (BCC) |
| **Open UI** | `/afflicted ui` |
| **Original** | [Afflicted 3 on CurseForge](https://www.curseforge.com/wow/addons/afflicted3) |

---

## Contents

- [Installation](#installation)
- [Features](#features)
- [Configuration](#configuration)
- [Troubleshooting](#troubleshooting)

---

## Installation

1. Download the addon (clone the repo or download the ZIP and extract it).
2. Put the addon folder into your TBC Anniversary **AddOns** folder:
   ```
   <TBC Anniversary install>\Interface\AddOns\
   ```
   The folder inside `AddOns` must be named **Afflicted** (rename it if you got e.g. `afflicted-anniversary`).
3. At the character select screen, open **AddOns** and enable **Afflicted**.
4. Enter the world and run `/afflicted ui` to open settings.

---

## Features

- **Enemy timers** — Cooldowns and buff durations on your current target (or all hostile units).
- **Totem tracking** — Timers and tick indicators for totems (e.g. Tremor, fire totems).
- **Two display modes** — Bars or icons; choose per anchor.
- **Announcements** — Optional messages when spells are used or expire (party, raid, raid warning, combat text, or a chat frame).
- **Six anchors** — Organize timers by category: **Damage**, **Defensive**, **Interrupts**, **Cooldowns**, **Spells**, **Buffs**. Drag and lock anchors in-game.
- **Extensible** — Add custom spells and timers via the in-game config.

---

## Configuration

- Open the options with:
  ```
  /afflicted ui
  ```
- From the config you can change display type (bars/icons), anchors, announcements, and add or edit tracked spells.

---

## Troubleshooting

**New or custom spells don’t show or track**

The addon can cache spell data. To force a refresh:

1. Exit the game completely.
2. In your TBC Anniversary install, go to:
   ```
   WTF\Account\<your_account>\SavedVariables
   ```
3. Delete the Afflicted save files (e.g. `AfflictedDB.lua` and `AfflictedDB.lua.bak`).
4. Start the game again and enable Afflicted.

Your addon settings will be reset; reconfigure as needed.

---

## Credits

This version is adapted for TBC Anniversary from the original **Afflicted 3** by Shadowed:  
[https://www.curseforge.com/wow/addons/afflicted3](https://www.curseforge.com/wow/addons/afflicted3)
