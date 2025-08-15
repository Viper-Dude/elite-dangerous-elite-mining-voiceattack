# EliteMining - VoiceAttack Profile for Almost Hands-free Mining in Elite Dangerous

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

### Firegroups

| Component | Firegroup | Notes |
|-----------|-----------|-------|
| Discovery Scanner | Secondary fire button |  |
| Mining Lasers | Primary fire button |  |
| Collector Limpet Controller | Same as Mining Laser (and Sub-surface Displacement Missile if installed) | Must be set manually |
| Pulse Wave Analyser | Primary fire button |  |
| Sub-surface Displacement Missile | Primary fire button |  |
| Prospector Limpet Controller | Secondary fire button | Must be set manually |

**Note:** Firegroups for Collector and Prospector Limpet Controllers are **not** set automatically by the profile. You must set them manually as shown above.

---

### Recommended Key/HOTAS Buttons

| Action | Description |
|--------|------------|
| Stop All VA Processes | Immediately stops all VoiceAttack commands currently running |
| Start Mining | Starts the Laser Mining Sequence |
| Reset Mining | Stops and resets the mining sequence if needed |
| Clear and Jump | Clears your ship from mass lock and activates Supercruise or an FSD jump (if a system is selected). This same button can also be used to enter a destination after jumping |


## Usage
Once installed and your firegroups are set:

- **Laser Mining Sequence** – Runs the full laser-mining process for you: switches modes if needed, sets power to weapons, turns on mining lasers, fires Collector limpets, opens and closes the cargo scoop, times your laser firing (mining), and finishes by resetting your ship for the next mining run.
- Use voice commands or your chosen keybinds.
- EliteVA will automatically read your in-game keybindings from Elite Dangerous (keyboard-only, not HOTAS).

## Known Limitations
- Works only with keyboard keybindings (HOTAS/joystick buttons are not supported for automated reads).
- Requires EliteAPI to be running in the background.

## Disclaimer
This profile is a fan-made tool and is not affiliated with Frontier Developments. Use at your own risk and in accordance with the game’s terms of service.

ViperDude


