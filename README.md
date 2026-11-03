# Map LFG for Raidcore Nexus

A Guild Wars 2 addon that opens the native Looking For Group (LFG) window directly to your current map's category and subcategory.


# Disclaimer
> [!CAUTION]
> ## Modifying Guild Wars 2 through any third party software is not supported by ArenaNet nor by any of its partners.
> ## You are using this addon at your own risk.

> [!IMPORTANT]
> This addon was built with appropriate limitations to ensure that it is within the official [Third Party Program Policy](https://help.guildwars2.com/hc/en-us/articles/360013625034-Policy-Third-Party-Programs).  
> If you believe this addon is violating the third party policy, please [create an issue](../../issues) here on this repository voicing your concerns.  
>   
> **Portions or the entirety of the codebase remain closed-source in compliance with requests by ArenaNet.**

## To ArenaNet
### Please reach out to us by [creating an issue](../../issues) for concerns, takedown requests or review requests for the codebase.


## ✨ Features
- **Instant Map Navigation:** Press `ALT+L` (or click the Quick-Access icon) to open the GW2 LFG panel straight to the category and subcategory of your current zone.
- **Direct Engine Integration:** Native, zero-delay UI opening with zero mouse-click interference and full compatibility with ArcDPS and Unofficial Extras.
- **In-Game Map Overrides:** Easily redirect any map (e.g. Mistlock Sanctuary -> Raids) via in-game dropdown menus or `map_overrides.txt`.
- **Smart World Boss Detection (v2.2.5):** Optionally switches Central Tyria LFG automatically to World Bosses during active event windows across all 14 Core Tyria World Bosses and the rotating Ley-Line Anomaly.
- **Toggle-Close Keypress:** Pressing your hotkey again shortly after opening can optionally close the contacts/LFG window.
- **Nexus Localization Support (v2.2.5):** Default English UI with automatic German translation when Nexus is set to German.
- **Custom Shortcut Slots:** Up to 5 user-configurable quick-access slots in the settings window with dedicated Nexus keybinds.
- **PvP & Lobby Support:**
  - In PvP match maps (e.g., Skyhammer, Kyhlo), LFG opening is safely disabled to respect game restrictions.
  - In the **Heart of the Mists** lobby, opens directly to *Player vs. Player -> Structured PvP*.
- **Quickplay Shortcuts:** One-click navigation to Fractal and Raid LFGs directly from the context menu.
- **In-Game Mail to Author:** Click *"Mail to Arronax.5471"* in the context menu to send a message or tip in-game.


## ⚙️ Map Overrides (In-Game GUI & `map_overrides.txt`)
You can redirect any map to open a custom LFG section of your choice directly in-game from the Settings menu (`ALT + SHIFT + L`) via the **Map Override for Current Zone** dropdowns, or manually by editing `map_overrides.txt` in your `Guild Wars 2/addons/MapLFG/` folder.

**Format:** `<MapID> <NativeEntryIndex>`

Lines starting with `#` are ignored as comments.

### Common Examples:
```txt
# Redirect Mistlock Sanctuary (Map 1206) to Raid LFG:
1206 71    # Raids (Experienced)
# 1206 72  # Raids (Training)
# 1206 91  # Raids Quickplay

# Redirect Mistlock Sanctuary (Map 1206) to Fractals:
# 1206 76  # Fractals (Master, Scale 76-100)
# 1206 90  # Fractals Quickplay
```
*(Tip: All available native entry numbers are exported to `lfg_dump.txt` in your addon folder.)*

Alternatively, you can configure a **Custom Slot** in `Map LFG Settings` (`ALT + SHIFT + L`) and assign a dedicated keybind to open Raid LFG from any zone!


## ⌨️ Controls & Keybinds
| Action | Default Keybind | Description |
| :--- | :--- | :--- |
| **Open Current Map LFG** | `ALT + L` | Opens LFG directly to your current zone |
| **Map LFG Settings** | `ALT + SHIFT + L` | Opens settings & calibration overlay |
| **Quick-Access Icon** | Left Click | Opens current map LFG |
| **Quick-Access Context** | Right Click | Opens shortcut menu & settings |

Keybinds can be customized at any time in the Raidcore Nexus overlay (`CTRL + O`).


## 📥 Installation

### Method 1: In-Game Addon Library (Recommended)
1. Open the **Nexus** menu in-game (`CTRL + O`).
2. Navigate to the **Addon Library** tab.
3. Search for **Map LFG** and click **Install**.

### Method 2: Manual Installation
1. Ensure [Raidcore Nexus](https://raidcore.gg/Nexus) is installed.
2. Download `Map_LFG.dll` from the latest [Release](../../releases).
3. Place `Map_LFG.dll` into your `Guild Wars 2/addons/` folder.
4. Restart Guild Wars 2 or load the addon via Nexus (`CTRL + O`).


## 👤 Author & Support
- **Author:** Arronax.5471
- **Community:** [Xytels Modding Community](https://discord.gg/BPXw54Dghq)
