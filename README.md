# EliteMining - VoiceAttack Profile for Hands-free Mining in Elite Dangerous

This repository contains the EliteMining VoiceAttack profile designed to streamline mining operations in Elite Dangerous with minimal manual input.

## Features
- Voice-controlled mining operations (limpet deployment, laser activation, etc.)
- Customizable ship presets for different mining scenarios
- Integrated with EliteAPI for real-time game data
- Over 500 organized voice commands
- TrackIR support

## Requirements
- [VoiceAttack](https://voiceattack.com/) (Paid version)
- [EliteVA (API) by Somfic](https://docs.somfic.dev/projects/eliteva)
- Elite Dangerous (PC version)
- Working microphone

## Installation
1. Download the latest release
2. Extract the `.rar` file to your VoiceAttack app folder
3. In VoiceAttack: **Profile > Import Profile**
4. Select `EliteMining-Profile.vap`

## Configuration

### Firegroup Setup

| Component                  | FG Preset          | Fire Button       | Notes                      |
|----------------------------|--------------------|-------------------|----------------------------|
| Discovery Scanner          | Set by command     | Secondary         |                            |
| Surface Scanner            | A                  | Primary           |                            |
| Mining Lasers              | Set by command     | Primary           |                            |
| Collector Limpet Controller| Same as Mining Lasers | Primary       | Must be set manually       |
| Pulse Wave Analyser        | Set by command     | Primary           |                            |
| Sub-surface Displacement   | Set by command     | Primary           |                            |
| Prospector Limpet Controller | Same as PWA     | Secondary         | Must be set manually       |

### Recommended Keybinds

| Action                    | Description                                  |
|---------------------------|----------------------------------------------|
| Stop All VA Processes     | Emergency stop for all commands              |
| Start Mining              | Initiates laser mining sequence              |
| Reset Mining              | Cancels current mining operation             |
| Deploy Seismic Charges    | Switches FG to seismic charge launcher       |
| Clear and Jump            | Handles FSD jumps and supercruise            |
| TrackIR Toggle            | Pauses TrackIR when docked (default: F9)     |

## Command Categories

### Firegroup Management
- Set Discovery Scanner to [A-H]
- Set Mining Lasers to [A-H]
- Set Weapons to [A-H]

### Status Checks
- "Say firegroup for weapons"
- "Say timer for laser mining"
- "Say toggle for cargo scoop"

### Mining Presets
Example: **"Set mining configuration for 3 x haz"**
- Auto-configures FGs, timers, and toggles
- Customizable for different ship builds

## Usage Tips
- **Long-press functionality**: Set the same button for start/stop commands
- **Training**: Use VoiceAttack's recognition training for better accuracy
- **Presets**: Start with a preset configuration for easier learning curve

## Limitations
- Only supports keyboard bindings (not HOTAS/joystick)
- Potential conflicts with HCS VoicePack (requires command adjustment)
- Currently in beta (features may change)

## Support
For issues or suggestions, please open an issue in this repository.

## Credits
- [Somfic](https://docs.somfic.dev/projects/eliteva) for EliteVA API
- CMDR ViperDude for profile development
