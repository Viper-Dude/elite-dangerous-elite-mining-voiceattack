# EliteMining - VoiceAttack Profile for Almost Hands-free Mining operations in Elite Dangerous

This repository contains EliteMining, a VoiceAttack profile designed to make mining operations in Elite Dangerous smoother, faster, and more immersive — with minimal manual input.

## Features
- Custom voice commands to automate mining operations (e.g., deploying limpets, activating and firing mining lasers).
- Customizable ship presets.
- Streamlined controls for an efficient mining workflow.
- Works alongside EliteAPI by Somfic for automatic in-game data reading.

## Requirements
- [EliteVA (API) by Somfic](https://docs.somfic.dev/projects/eliteva)
- [VoiceAttack](https://voiceattack.com/) – Paid version
- A working microphone for voice commands
- Elite Dangerous (PC version)

## Installation
1. Download the latest release from this repository.
2. Extract all contents of the downloaded `.rar` file into your VoiceAttack app folder.
3. In VoiceAttack, go to **Profile > Import Profile** (in your VoiceAttack app folder).
4. Select **EliteMining-Profile.vap**.

## Update
1. Download the EliteMining.vap file from the latest release.
2. Replace the existing file in your `\VoiceAttack\App\EliteMining` folder.
3. Update your Elite Dangerous keybindings and joystick/HOTAS buttons as needed.

Info. Sometimes updates require you to update both the Elitemining.vap and the folder Variables

## Getting Started

### Set Your Firegroup (FG) as Follows

| Component | FG  | Primary or Secondary fire button | Notes | 
|-----------|------------|----------------------------------|-------|
| Discovery Scanner |Set by command or presets| Secondary fire button |  |  |
| Surface Scanner |A| Primary fire button |  |
| Mining Lasers |Set by command or presets| Primary fire button |  |
| Collector Limpet Controller |Set by command or presets| Same as Mining Lasers (and Sub-surface Displacement Missile if installed) | Must be set manually |
| Pulse Wave Analyser |Set by command or presets| Primary fire button   |  |
| Sub-surface Displacement Missile |Set by command or presets| Primary fire button | |
| Prospector Limpet Controller |Same as Pulse Wave Analyser (recommended) | Secondary fire button | Must be set manually |

**Note:** FG for Collector and Prospector Limpet Controllers are **not** set automatically by the profile. You must set them manually as shown above. 

### Recommended Key/HOTAS Buttons

| Action | Description |
|--------|------------|
| Stop All VA Processes | Immediately stops all VoiceAttack commands currently running |
| Start Mining | Starts the Laser Mining Sequence |
| Reset Mining | Stops and resets the mining sequence if needed |
| Deploy seismic charge launcher | Setting FG for Seismic Charge Launcher |
| Start Scanning for Cores | Start Sequence for scanning cores (Setting FG,Continuous boost and pulsewave|
| Stop Scanning for Cores | Stopping Scanning for core|
| Clear and Jump | Clear your ship from mass lock and activates Supercruise or an FSD jump (if a system is selected). This same button can also be used to enter a destination from supercruise, Activate/disable Supercruise and FDS jump to another system |
| TrackIR integration | Set your pause toggle in the TrackIR software to f9 and TrackIR will pause/unpause when your ship is docked/undocked. You can also change the keybind to your liking in the command "Toggle TrackIR" |

Tips: For a command that have both a start and stop (reset) function you can set the reset/stop key/button
to the same function as your start key/button with enabling "Shortcut is invoked when long-pressed" when long-pressed". (Short press = start command,Long Press = stop/reset the same command)


## Commands

The **EliteMining** profile contains **553 commands** in total, organized into categories. Below are two important categories directly related to firegroup and mining operations.

### Check – Status
These commands let you check what FG or toggles are currently active. They are useful for troubleshooting or confirming that the correct setup is in place before starting a mining sequence.  

| Spoken Command | Description |
|----------------|-------------|
| Say firegroup for weapons | Reports the FG assigned to weapons |
| Say firegroup for mining lasers | Reports the FG assigned to mining lasers |
| Say firegroup for Sub-surface Displacement Missile | Reports the FG assigned to Sub-surface Missiles |
| Say firegroup for Pulse Wave Analyser | Reports the FG assigned to the Pulse Wave Analyser |
| Say Toggle for cargo scoop / power / mining / etc. | Confirms current toggle status for the specified system |
| Say timer for laser mining / target / pause | Reads back the current timer values used in mining sequences |

These commands directly reflect the **FG setup** you configured earlier — see [Firegroup Table](#set-your-firegroup-fg-as-follows).

---

### Set – FG 
These commands allow you to directly set or change FG by voice command, without opening your right-hand panel manually.  

| Spoken Command | Description |
|----------------|-------------|
| Set firegroup for mining lasers to [A–H] | Assigns mining lasers to the chosen FG |
| Set firegroup for weapons to [A–H] | Assigns weapons to the chosen FG |
| Set firegroup for Sub-surface Displacement Missile to [A–H] | Assigns SSD missiles to the chosen FG |
| Set firegroup for Pulse Wave Analyser to [A–H] | Assigns PWA to the chosen FG |

Use these if you want to *quickly apply* or *reconfigure* the FG defined earlier in the [FG Table](#set-your-firegroup-fg-as-follows).

### Misc

| Spoken Command | Description |
|----------------|-------------|
| Landing Request | Asking for docking and extend landing gear after 5 seconds.  |
| Enable/Disable Autohonk (enabled by default) |If enable, Start honk (discovery scan) after a jump |

## Mining - Presets example

This section of the profile provides quick ship configuration presets for different mining situations. Instead of manually toggling modules every time, you can use voice commands or keys/joystick to switch between optimized loadouts.

### Ship Presets (example)

**Hazardous Mining**  
*Set mining configuration for 3 x haz*  
- Setting firegroup for mining lasers to charlie  (setting FGs )
- Setting firegroup for discovery scanner to alpha (setting FGs )
- Setting firegroup for Pulse Wave Analyser to bravo (setting FGs )
- Setting firegroup for Sub-surface Displacement Missile to foxtrot (setting FGs )
- Setting firegroup for weapons to echo (setting FGs )
- Setting timer for laser mining to 38 seconds (Duration for firing lasers)
- Setting timer for laser mining extra to 9 seconds (Duration for firing lasers second time
(after charging power to weapons) if toggle for laser mining extra is set to 1 )
- Setting timer for pause to 4 seconds (Pauses for charging weapons after firing lasers is completed)
- Setting timer for cargo scoop to 8 seconds (If toggle for cargo scoop to 1, time before retract cargo scoop after firing lasers is completed)
- Setting timer for target to 8 seconds (If toggle for target is 1, time before target prospector is unselected after firing lasers is completed)
- Setting toggle for cargo scoop to 1
- Setting toggle for laser mining extra to 0 ( 1 = firing lasers for a second time after a pause)
- Setting toggle for mining to 1 (1= select prospector as target after firing a prospector)
- Setting toggle for power settings to 1 ( 0 = Balancing power 1 = Max power to engines)
- Setting toggle for target to 1 ( 1 = unselected prospector after firing lasers is completed)
- Setting toggle for Pulse Wave Analyser to 0 ( 1 = After firing laser is completed, setting FG to Pulswave analyser ) 

### You can easily customize this section to match your own ship builds or preferences. 
- Add new presets for your own build ships with FG 
- Change FG for laser,scanner and weapons,set timers for firing lasers and much more with build in "called commands" for FGs,toggles and timers.  

### How to Use

1. Say the command for the preset (for example: "Set mining configuration for 3 x haz or 3 x haz" or Set mining configuration for 3 x none haz multiminer or3 x none haz multiminer`).  
2. VoiceAttack will automatically toggle your ship’s modules to the appropriate configuration.  
3. Switch back and forth at any time depending on the mining site.
4. On-the-fly changes e.g., say "Set timer for laser mining to 1-50 seconds" this command will change the time duration of lasers firing at the rock. another example is  Say "Set Toggle for cargo scoop to 0- 1", this command will enabel (1) or disable (0) "Stop (Mining " command is set) if the cargo scoop should be retracted or not after a duration of time set in the command when the "Timer for cargo scoop set to * seconds. 


## Usage
Once installed and your FG are set:

- **Laser Mining Sequence** – Runs the full laser-mining process for you: switches modes if needed, sets power to weapons, turns on mining lasers, fires Collector limpets, opens and closes the cargo scoop, times your laser firing (mining), and finishes by resetting your ship for the next mining run.
- Use voice commands or your chosen keybinds.
- EliteVA will automatically read your in-game keybindings from Elite Dangerous (keyboard-only, not HOTAS).
  
## Known Limitations/issues
- Works only with in game custom keyboard keybindings. HOTAS/joystick buttons are not supported for automated reads and therefore need to be set manually inside the profile.
- Requires [EliteVA (API) by Somfic](https://docs.somfic.dev/projects/eliteva)

- This profile works together with HCS Voicepack with some conflicting commands.
If you use HCS voicepack as you main profile be sure to change the commands for "Start and Stop mining inside the  EliteMining profile.
- There are no known issues in use together with EDcopilot.

  ## Training Speech Recognition

VoiceAttack includes built-in tools to help improve how well it understands your voice. Taking a few minutes to train the recognition engine makes commands trigger more reliably.

### How to Train
1. Open VoiceAttack.  
2. Go to **Help** → **Utilities** → **Recognition Training**.  
3. Follow the on-screen prompts and read the provided text passages.  

### Tips
By using the built-in utilities, you can adapt the profile to your own voice and ensure your custom commands work smoothly.
- Train in a quiet environment using the same microphone you play with.  
- Be consistent in how you say your commands.  
- If a command is often misheard, you can edit its phrase directly in the VoiceAttack profile and choose words that are easier for you to say.
- Remember to back up your speech engine training file with this tool: [SpProfileMgr.zip](https://voiceattack.com/filesend.aspx?id=SpProfileMgr.zip) 

By using the built-in utilities, you can adapt the profile to your own voice and ensure your custom commands work smoothly.

## Missing features
- Add a switch for core/laser mining
- Add commands and presets for Core mining.


## Disclaimer
This Profile is Work-in-progress and is subject for changes. (still in beta) 
This profile is a fan-made tool and is not affiliated with Frontier Developments. Use at your own risk and in accordance with the game’s terms of service.

## Credits

- Somfic – Creator of EliteVA (API) used for automatic in-game data reading.

CMDR ViperDude


