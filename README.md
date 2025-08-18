# EliteMining - VoiceAttack Profile for Almost Hands-free Mining operations in Elite Dangerous

This repository contains EliteMining, a VoiceAttack profile designed to make mining operations in Elite Dangerous smoother, faster, and more immersive — with minimal manual input.

## Features
- Custom voice commands to automate mining operations (e.g., deploying limpets, activating and firing mining lasers)
- Customizable ship presets
- Streamlined controls for an efficient mining workflow
- Works alongside EliteAPI by Somfic for automatic in-game data reading

## Requirements
- [EliteVA (API) by Somfic](https://docs.somfic.dev/projects/eliteva)
- [VoiceAttack](https://voiceattack.com/) – Paid version
- A working microphone for voice commands
- Elite Dangerous (PC version)

## Installation
1. Download the latest release from this repository
2. Extract all contents of the downloaded `.rar` file into your VoiceAttack app folder
3. In VoiceAttack, go to **Profile > Import Profile** (in your VoiceAttack app folder)
4. Select **EliteMining-Profile.vap**

## Update
1. Download the EliteMining.vap file from the latest release
2. Replace the existing file in your `\VoiceAttack\App\EliteMining` folder
3. Update your Elite Dangerous keybindings and joystick/HOTAS buttons as needed

**Note:** Sometimes new updates require you to update both the Elitemining.vap and the Variables folder inside the EliteMining folder.

## Getting Started

### Set Your Firegroup (FG) as Follows

| Component | FG | Primary or Secondary fire button | Notes |
|-----------|----|----------------------------------|-------|
| Discovery Scanner | Set by command or presets | Secondary fire button | |
| Surface Scanner | A | Primary fire button | |
| Mining Lasers | Set by command or presets | Primary fire button | |
| Collector Limpet Controller | Set by command or presets | Same as Mining Lasers (and Sub-surface Displacement Missile if installed) | Must be set manually |
| Pulse Wave Analyser | Set by command or presets | Primary fire button | |
| Sub-surface Displacement Missile | Set by command or presets | Primary fire button | |
| Prospector Limpet Controller | Same as Pulse Wave Analyser (recommended) | Secondary fire button | Must be set manually |

**Important:** FG for Collector and Prospector Limpet Controllers are **not** set automatically by the profile. You must set them manually as shown above.

### Recommended Key/HOTAS Buttons

| Action | Description |
|--------|-------------|
| Stop All VA Processes | Immediately stops all VoiceAttack commands currently running |
| Start Mining | Starts the Laser Mining Sequence |
| Reset Mining | Stops and resets the mining sequence if needed |
| Deploy seismic charge launcher | Change FG for Seismic Charge Launcher |
| Deploy weapons | Change FG to weapons |
| Start Scanning for Cores | Start Sequence for scanning cores (Setting FG, Continuous boost and pulsewave) |
| Stop Scanning for Cores | Stop sequence for scanning cores |
| Clear and Jump | Clear your ship from mass lock and activates Supercruise or an FSD jump |
| TrackIR integration | Set your pause toggle in the TrackIR software to F9 |

## Commands

### Check – Status
These commands let you check what FG or toggles are currently active.

| Spoken Command | Description |
|----------------|-------------|
| "Say firegroup for weapons" | Reports the FG assigned to weapons |
| "Say firegroup for mining lasers" | Reports the FG assigned to mining lasers |
| "Say firegroup for Sub-surface Displacement Missile" | Reports the FG assigned to Sub-surface Missiles |
| "Say firegroup for Pulse Wave Analyser" | Reports the FG assigned to the Pulse Wave Analyser |
| "Say Toggle for cargo scoop / power / mining / etc." | Confirms current toggle status |
| "Say timer for laser mining / target / pause" | Reads back current timer values |

### Voice Commands for Setting Parameters

| Spoken Command | Description |
|----------------|-------------|
| "Set firegroup for Discovery Scanner to [A–H]" | Assigns Discovery Scanner to chosen FG |
| "Set firegroup for mining lasers to [A–H]" | Assigns mining lasers to chosen FG |
| "Set firegroup for Pulse Wave Analyser to [A–H]" | Assigns Pulse Wave Analyser to chosen FG |
| "Set firegroup for Seismic Charge Launcher to [A–H]" | Seismic Charge Launcher to chosen FG |
| "Set firegroup for Sub-surface Displacement Missile to [A–H]" | Assigns missiles to chosen FG |
| "Set firegroup for weapons to [A–H]" | Assigns weapons to chosen FG |

Additional commands available in these categories:
- Commands - Set Firegroups (FG)
- Commands - Set Timers
- Commands - Set Toggles
- Commands - Check - Status

### Misc Commands

| Spoken Command | Description |
|----------------|-------------|
| "Landing Request" | Requests docking and extends landing gear after 5 seconds |
| "Enable/Disable Autohonk" (enabled by default) | Automatic discovery scan after jump |

## Mining Presets Example

### Hazardous Mining Preset
**Command:** "Set mining configuration for 3 x haz"

Configuration includes:
- Firegroups set for all mining tools
- Timers configured for optimal mining
- Toggles set for proper power management

### Customization
You can:
- Add new presets for your ship builds
- Change FGs, timers, and toggles on-the-fly
- Adjust with built-in commands

## Usage Tips
For commands with start/stop functions:
- **Short press**: Start command
- **Long press**: Stop/reset same command
- Enable "Shortcut is invoked when long-pressed"

Best practice:
1. Set your fire buttons and FGs as described
2. Choose a ship preset
3. Go mining to familiarize yourself with commands

## Known Limitations
- Only works with in-game keyboard keybindings (HOTAS requires manual setup)
- Potential conflicts with HCS VoicePack (requires command adjustments)
- Works with EDCopilot without issues

## Training Speech Recognition
1. Open VoiceAttack
2. Go to **Help → Utilities → Recognition Training**
3. Follow on-screen prompts
4. For best results: train in quiet environment with your gaming microphone

Backup your speech profile with: [SpProfileMgr.zip](https://voiceattack.com/filesend.aspx?id=SpProfileMgr.zip)

## Missing Features
- Core/laser mining switch
- Primary/secondary firebutton switch

## Disclaimer
This profile is work-in-progress (still in beta) and not affiliated with Frontier Developments. Use at your own risk.

## Credits
- [Somfic](https://docs.somfic.dev/projects/eliteva) – Creator of EliteVA
- CMDR ViperDude
