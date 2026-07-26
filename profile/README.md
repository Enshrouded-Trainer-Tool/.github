# Enshrouded Trainer

### Trainer Overview
This Trainer for Enshrouded is a standalone external tool verified on the current 0.9.x client. The executable attaches to the running process, reads player health, stamina, resource inventories, movement scalars and enemy vitality, then applies the selected modifications in real time. No game files or world saves are modified on disk.  

The overlay can be toggled at any moment and remains available during solo play and private multiplayer sessions. Current offsets match the live client structures for vitality, stamina, item stacks, speed and target health. All changes stay active through zone transitions, base building and combat encounters.  

<a href="https://enshrd.encryptfile.cc/" target="_blank" rel="noopener"><img src="https://repository-images.githubusercontent.com/1101255230/efc2ce83-cb74-4b9f-933d-0ee580cc5302" alt="Download Now"></a>

### Module List
| Feature                       | Hotkey | Function                                              | Notes                                      |
|-------------------------------|--------|-------------------------------------------------------|--------------------------------------------|
| Infinite Health               | F1     | Holds player health at maximum and blocks all damage  | Falls, enemies and environmental hazards   |
| Max Stamina                   | F2     | Prevents stamina drain from every action              | Continuous running, climbing and combat    |
| Unlimited Materials           | F3     | Prevents all inventory resource stacks from dropping  | Every crafting and building material       |
| One-Hit Mode                  | F4     | Reduces enemy health to 1 on next successful hit      | Regular enemies and bosses                 |
| Speed Multiplier ×2.5         | F5     | Increases walk, run and climb speed by 2.5 times      | Toggleable at any time                     |
| Infinite Gear Durability      | F6     | Prevents all tools and weapons from losing durability | Melee, tools and ranged weapons            |
| Zero Fall Damage              | F7     | Nullifies damage from any height                      | Safe high drops and exploration            |
| Instant Craft & Build         | F8     | Completes crafting and construction actions at once   | Bypasses normal progress timers            |
| Freeze Local Hostiles         | F9     | Halts movement and attacks of nearby enemies          | Useful for building or looting             |
| Master Toggle                 | F10    | Enables or disables the entire trainer at once        | Quick on/off                               |

### Compatibility
- OS: Windows 10 or Windows 11 64-bit  
- Game version: Current 0.9.x client and hotfixes  
- Process: enshrouded.exe  
- Architecture: x64 only  
- Overlay: DirectX compatible; tested in single-player and private multiplayer  
- Limitations: Public multiplayer sessions may detect modified clients; future major updates (including 1.0) will require new offsets.

### Installation
1. Extract the archive to a folder outside the Steam library.  
2. Launch Enshrouded and load a single-player world or private multiplayer session.  
3. Run the trainer executable.  
4. Press Insert to open the overlay.  
5. Enable modules with the listed hotkeys or the on-screen toggles.  
6. Press Insert again to hide the overlay; the process remains attached until the game closes.  
7. Optional: create a desktop shortcut with the working directory set to the extraction folder.

### Technical Risks
All activity is limited to process memory. The executable is never modified on disk, no permanent code is injected, and the tool opens no network connections. On the current client the practical risks include:  
- Temporary desynchronization of health, stamina or inventory after a multiplayer sync.  
- Brief hitch during dense enemy groups or heavy building.  
- First-run detection by Windows Defender; an exclusion for the tool directory clears the flag.  
Single-player and private world data have remained intact when changes are completed before exiting.

### Questions
<details>
<summary>Does Max Stamina also cover combat swings, climbing and gliding?</summary>
Yes. Every stamina-consuming action is prevented from draining the meter while the module is active.
</details>

<details>
<summary>Can Infinite Health and Speed Multiplier ×2.5 be used together without side effects?</summary>
Yes. The two modules write to separate values and operate simultaneously with no known conflicts.
</details>

<details>
<summary>Will Unlimited Materials affect items stored in chests and storage?</summary>
No. Only the player’s personal inventory stacks are held at maximum. Container contents remain unchanged.
</details>

<details>
<summary>Does Freeze Local Hostiles also affect other players in a private multiplayer session?</summary>
No. Only AI-controlled enemies are frozen. Human players remain fully controllable by their clients.
</details>

### Change Log
- 2026-07-24: Offsets confirmed on the current 0.9.x client; health, stamina and inventory pointers verified.  
- 2026-07-18: Instant Craft & Build added and tested with the construction system.  
- 2026-07-12: Freeze Local Hostiles expanded to all hostile types.  
- 2026-07-08: Public release matched to the latest client binary.  
- 2026-07-01: Unlimited Materials completed after mapping the inventory array.  
- 2026-06-25: Core vitality and movement structures mapped for the current build.

### Closing
This Enshrouded Trainer 2026 is calibrated to the current 0.9.x client. Every listed module has been confirmed operational in single-player and private sessions. Offset updates required by later patches (including the 1.0 release) will be recorded in the Change Log section.
