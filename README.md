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

## Getting Started

### Set Your Firegroups as Follows

| Component | Firegroup | Notes |
|-----------|-----------|-------|
| Discovery Scanner | Secondary fire button |  |
| Mining Lasers | Primary fire button |  |
| Collector Limpet Controller | Same as Mining Laser (and Sub-surface Displacement Missile if installed) | Must be set manually |
| Pulse Wave Analyser | Primary fire button |  |
| Sub-surface Displacement Missile | Primary fire button |  |
| Prospector Limpet Controller | Secondary fire button | Must be set manually |

**Note:** Firegroups for Collector and Prospector Limpet Controllers are **not** set automatically by the profile. You must set them manually as shown above.
--

### Recommended Key/HOTAS Buttons

| Action | Description |
|--------|------------|
| Stop All VA Processes | Immediately stops all VoiceAttack commands currently running |
| Start Mining | Starts the Laser Mining Sequence |
| Reset Mining | Stops and resets the mining sequence if needed |
| Clear and Jump | Clear your ship from mass lock and activates Supercruise or an FSD jump (if a system is selected). This same button can also be used to enter a destination from supercruise, Activate/disable Supercruise and FDS jump to another system |
| Trackir integration | Set your pause toggle in the Trackir software to f9 and trackir will pause/unpause when your ship is docked/undocked. You can also change the keybind to you liking in the command "Toggle Trackir" |


## Commands

The **EliteMining** profile contains **553 commands** in total, organized into categories. Below are two important categories directly related to firegroup and mining operations.

### Check – Status
These commands let you check what firegroups or toggles are currently active. They are useful for troubleshooting or confirming that the correct setup is in place before starting a mining sequence.  

| Spoken Command | Description |
|----------------|-------------|
| Say firegroup for weapons | Reports the firegroup assigned to weapons |
| Say firegroup for mining lasers | Reports the firegroup assigned to mining lasers |
| Say firegroup for Sub-surface Displacement Missile | Reports the firegroup assigned to Sub-surface Missiles |
| Say firegroup for pulse wave analyser | Reports the firegroup assigned to the Pulse Wave Analyser |
| Say Toggle for cargo scoop / power / mining / etc. | Confirms current toggle status for the specified system |
| Say timer for laser mining / target / pause | Reads back the current timer values used in mining sequences |

These commands directly reflect the **Firegroups setup** you configured earlier see [Firegroups Table](#set-your-firegroups-as-follows). 

---

### Set – Firegroups (FG)
These commands allow you to directly set or change firegroups by voice command, without opening your right-hand panel manually.  

| Spoken Command | Description |
|----------------|-------------|
| Set firegroup for mining lasers to [A–H] | Assigns mining lasers to the chosen firegroup |
| Set firegroup for weapons to [A–H] | Assigns weapons to the chosen firegroup |
| Set firegroup for Sub-surface Displacement Missile to [A–H] | Assigns SSD missiles to the chosen firegroup |
| Set firegroup for pulse wave analyser to [A–H] | Assigns PWA to the chosen firegroup |
Use these if you want to *quickly apply* or *reconfigure* the firegroups defined earlier in the [Firegroups Table](#set-your-firegroups-as-follows).  

### Misc

| Spoken Command | Description |
|----------------|-------------|
| Landing Request | Asking for docking and extract landing gear after 5 seconds.  |
| Enable/Disable Autohonk (enablet by default) |If enable, Start honk (discovery scan) after a jump |

## Mining - Presets example

This section of the profile provides quick ship configuration presets for different mining situations. Instead of manually toggling modules every time, you can use voice commands or keys/hoystick to switch between optimized loadouts.

### Ship Presets (example)

**Hazardous Mining**  
*Set mining configuration for 3 x haz*  
- Setting firegroup for mining laser's to charlie  (setting FG )
- Setting firegroup for discovery scanner to alpha (setting FG )
- Setting firegroup for pulse wave analyser to bravo (setting FG )
- Setting firegroup for Sub-surface Displacement Missile to foxtrot (setting FG )
- Setting firegroup for weapons to echo (setting FG )
- Setting timer for laser mining to 38 seconds (Duration for firing laser's)
- Setting timer for laser mining extra to 9 seconds (Duration for firing laser's second time
(after charging power to weapons) if toggle for laser mining extra is set to 1 )
- Setting timer for pause to 4 seconds (Pauses for charging weapons after firing laser's is completed)
- Setting timer for cargo scoop to 8 seconds (If toggle for cargo scoop to 1, time before retract cargo scoop after firing laser's is completed)
- Setting timer for target to 8 seconds (If toggle for target is 1, time before target prospector is unselected after firing laser's is completed)
- Setting toggle for cargo scoop to 1
- Setting toggle for laser mining extra to 0 ( 1 = firing lasers for a second time after a pause)
- Setting toggle for mining to 1 (1= select prospector as target after firing a prospector)
- Setting toggle for power settings to 1 ( 0 = Balancing power 1 = Max power to engines)
- Setting toogle for target to 1 ( 1 = unselected prospector after firing laser's is completed)
- Setting toggle for pulse wave analyser to 0 ( 1 = After firing laser is completed, setting FG to Pulswave analyser ) 

### You can easily customize this section to match your own ship builds or preferences. 
- Add new presets for your own build ships with firegroups 
- Change Firegroups for laser,scanner and weapons,set timers for firing laser's and much more with build in "called commands" for firegroups,toggles and timers.  

### How to Use

1. Say the command for the preset (for example: "Set mining configuration for 3 x haz or 3 x haz" or Set mining configuration for 3 x none haz multiminer or3 x none haz multiminer`).  
2. VoiceAttack will automatically toggle your ship’s modules to the appropriate configuration.  
3. Switch back and forth at any time depending on the mining site.
4. On fly changes e.g., say "Set timer for laser mining to 1-50 seconds" this command will change the time duration of laser's firing at the rock. another example is  Say "Set Toggle for cargo scoop to 0- 1", this command will enabel (1) or disable (0) "Stop (Mining " command is set) if the cargo scoop should be retracted or not after a duration of time set in the command when the "Timer for cargo scoop set to * seconds. 


## Usage
Once installed and your firegroups are set:

- **Laser Mining Sequence** – Runs the full laser-mining process for you: switches modes if needed, sets power to weapons, turns on mining lasers, fires Collector limpets, opens and closes the cargo scoop, times your laser firing (mining), and finishes by resetting your ship for the next mining run.
- Use voice commands or your chosen keybinds.
- EliteVA will automatically read your in-game keybindings from Elite Dangerous (keyboard-only, not HOTAS).
  
## Known Limitations/issues
- Works only with in game custom keyboard keybindings. HOTAS/joystick buttons are not supported for automated reads and therefore need to be set manually inside the profile.
- Requires [EliteVA (API) by Somfic](https://docs.somfic.dev/projects/eliteva)

- This profile works together with HCS Voicepack with some conflicting commands.
If you use HCS voicepack as you main profile be sure to change the commands for "Start and Stop mining inside the  EliteMining profile.
- There is none known issue in use together with EDcopilot.

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
- Add commands and presets for Core minig.


## Disclaimer
This Profile is Work-in-progress and is subject for changes. (still in beta) 
This profile is a fan-made tool and is not affiliated with Frontier Developments. Use at your own risk and in accordance with the game’s terms of service.


ViperDude


