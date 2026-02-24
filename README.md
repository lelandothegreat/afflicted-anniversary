# Afflicted

Afflicted is an enemy spell timer mod for PvP (mainly arenas). **Currently supported only for TBC Anniversary (BCC).** The game loads `Afflicted-BCC.toc` when running the TBC Anniversary client.

This addon is for players who want useful information such as when an interrupt is on cooldown and you're safe to cast a heal, or when Blessing of Freedom will be back up on an enemy Paladin. New timers for abilities not included by default can be added in the configuration. The system is flexible enough to track any enemy timer, including traps and totems.

Alerts for when a spell is triggered (or ends), and when you interrupt or dispel an enemy, are included. Alerts can be shown in party, raid, raid warning, combat text, or a specified chat frame.

**Slash command:** `/afflicted ui`

---

## Installation

1. **Download** the addon (clone this repo or download and extract the ZIP).
2. **Copy the addon folder** into your TBC Anniversary (BCC) game directory: `Interface\AddOns\` (e.g. inside your BCC game install folder).
3. Ensure the folder name is **Afflicted** (e.g. if you downloaded as `afflicted-anniversary`, rename it to `Afflicted`).
4. Restart the game or log out and back in. The addon should appear in the AddOns list on the character select screen.
5. Enable **Afflicted** in the AddOns list, then enter the world and use `/afflicted ui` to open the options.

---

## Features

- Tracks cooldown and buff timers on enemies
- Tracks totem timers (including ticks for Tremor, fire totems, etc.)
- Icons and bars display modes
- Announcements for when spells are used and when they’re back up
- Six anchors to organize spells: Damage, Defensive, Interrupts, Cooldowns, Spells, Buffs

![Bars view](https://user-images.githubusercontent.com/85767653/158212715-d7aac821-2403-4a57-8083-d70abd11f61e.png)

![Icons view](https://user-images.githubusercontent.com/85767653/158212807-d702611f-a3ee-4e42-9fd7-31ad74be878e.png)

![Configuration](https://user-images.githubusercontent.com/85767653/158213771-5ec98e8c-90f5-4b87-927f-6f15f1cd00a0.png)

---

## Known bug

If you add spells in the code and they don’t appear or get tracked in game:

1. Close the game.
2. Go to `WTF\Account\<your_account>\SavedVariables` inside your TBC Anniversary (BCC) game folder.
3. Delete the Afflicted-related files (e.g. `AfflictedDB.lua` and `AfflictedDB.lua.bak`).
4. Launch the game again.

The new spells should then appear. This resets the addon’s saved settings.
