# Cyberpunk RED Character Sheet

A fan-made, browser-based character sheet for the Cyberpunk RED tabletop roleplaying game. Built as a single self-contained HTML file with no external dependencies beyond Google Fonts.

This project is unofficial and unaffiliated with R. Talsorian Games or CD PROJEKT RED. Cyberpunk RED is a trademark of R. Talsorian Games.

---

## Features

### Tab 1 - Main Sheet

- Full set of character stats: INT, REF, DEX, TECH, COOL, WILL, LUCK, MOVE, BODY, EMP.
- Skills organized by category: Awareness, Body, Control, Education, Fighting, Performance, Ranged Weapons, Social, and Technique.
- Each skill row tracks Modifier, Level, Stat, and Base values.
- Support for custom skills throughout the skill grid.
- Weapons table with up to 6 entries (name, damage, ammo, rate of fire, notes).
- Armor panel with left and right sections (location, stopping power, penalty).
- Hit Points panel with Max, Current, Seriously Wounded threshold, Death Save, Critical Wounds log, and Addictions.

### Tab 2 - Lifepath

- Character portrait upload: click the portrait area to upload any image from disk. The portrait is displayed inside the tab and persists across page reloads via local storage. A hover overlay allows replacing or removing the image. The portrait is also embedded in JSON exports.
- Lifepath fields: Cultural Origins, Personality, Clothes and Hair Style, What You Value Most, Feelings about People, Most Valued Person, Most Valued Possession, Family Background, Childhood Environment, Family Crisis, Life Goals, Tragic Love Affairs.
- Keepers and Career section: Friends, Enemies, Why, What Can They Throw at You, Role-specific Lifepath, Reputation and Events, Improvement.
- My Stuff section: Housing, Rent, Lifestyle, Fashion, Gear (8 slots), and Cash.

### Tab 3 - Cyberware

- Cyberware grid for all implant locations: Cybereye (Left and Right), Cyberaudio Suite, Neural Link, Cyber-arm/hand (Left and Right), Cyber-leg/foot (Left and Right), Internal, External, Fashionware, and Borgware.
- Humanity tracker with current Humanity and Total Loss fields.
- Cyberdeck panel with Deck name, PRG Slots, HDW Slots, and UNI Slots, plus two program/hardware tables (name, ATK, DEF, REZ, Class).

---

## Autosave System

All input fields are automatically saved to the browser's local storage after 500 milliseconds of inactivity. This means that if the page is closed and reopened in the same browser, all data is restored without any manual action required.

The topbar displays an "AUTOSAVE ON" indicator that briefly flashes green with "AUTOSAVED" after each write.

The character portrait is stored separately in local storage as a base64 data URL.

---

## JSON Import and Export

### Export

Clicking "SAVE JSON" in the topbar downloads a JSON file containing all field values and the character portrait (as a base64 string under the key `__portrait__`). The file is named using the character's handle.

### Import

Clicking "LOAD JSON" opens a file picker. Selecting a previously exported JSON file restores all field values and the portrait. If the loaded file does not contain a portrait, any existing portrait in local storage is cleared.

---

## Update Notes Popup

When the page detects a new version (tracked via local storage), a small slide-in panel appears in the bottom-left corner listing what changed in that release. Once acknowledged, it does not appear again until the next version update.

Current version: 1.0

---

## How to Use

No build step is required. Open `index.html` in any modern browser. An internet connection is needed only to load the fonts from Google Fonts; all other functionality is offline-capable.

---

## Project Structure

```
index.html    Single self-contained file containing all HTML, CSS, and JavaScript.
README.md     This file.
```

---

## Legal Notice

This is an unofficial fan project created for personal use. All game rules, terminology, and lore referenced belong to their respective rights holders. This sheet does not reproduce copyrighted game content.