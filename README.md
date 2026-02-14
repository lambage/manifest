# Strike Force - Martial Arts Training System

## Overview
Strike Force is an intelligent martial arts training device that combines physical target sensors with mobile app connectivity to provide real-time feedback and training analytics. The system consists of:

- **ESP32 Microcontroller Firmware**: Handles sensor input and wireless communication
- **Flutter Mobile Application**: Provides training modes, statistics, and user interface
- **Physical Hardware Structure**: Robust frame with 6 electronic strike targets

## Repository Structure

This repository uses Google's `repo` tool to manage multiple related projects:

- **strike_force_app**: Flutter mobile application
- **strike_force_esp32**: ESP32 firmware for sensor and communication
- **HARDWARE_DESIGN.md**: Comprehensive physical hardware design specifications

## Getting Started

### For Software Development

1. **Install repo tool**:
   ```bash
   mkdir ~/bin
   curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
   chmod a+x ~/bin/repo
   export PATH=~/bin:$PATH
   ```

2. **Initialize and sync repositories**:
   ```bash
   repo init -u https://github.com/lambage/manifest.git
   repo sync
   ```

3. **Development**:
   - Navigate to `strike_force_app/` for mobile app development
   - Navigate to `strike_force_esp32/` for firmware development

### For Hardware Construction

See **[HARDWARE_DESIGN.md](HARDWARE_DESIGN.md)** for comprehensive specifications including:
- Detailed structural design options (steel, aluminum, wood/metal hybrid, commercial-grade)
- Target placement specifications for all 6 positions
- Materials list and cost estimates ($500 - $6,000 depending on build quality)
- Assembly instructions and safety considerations
- Maintenance requirements
- CAD recommendations and fabrication options

## System Architecture

### Hardware Components
- **6 Strike Targets**: Force-sensitive pads at head, chest, arms, and torso positions
- **ESP32 Microcontroller**: Wireless connectivity and sensor processing
- **Structural Frame**: Adjustable mounting system for targets
- **Power System**: Rechargeable battery with charging circuit

### Software Components
- **Mobile App** (Flutter): 
  - Training modes and exercises
  - Real-time strike feedback
  - Performance analytics and history
  - User profiles and progression tracking
  
- **Firmware** (ESP32):
  - Force sensor monitoring
  - Bluetooth/WiFi communication
  - Strike detection algorithms
  - Battery management

## Target Positions

The system features 6 targets positioned for comprehensive martial arts training:

1. **Head Target**: Upper striking zone
2. **Chest Target**: Center mass striking
3. **Right Arm Target**: Side striking (right)
4. **Left Arm Target**: Side striking (left)
5. **Right Torso/Kick Target**: Lower right zone
6. **Left Torso/Kick Target**: Lower left zone

## Hardware Design Philosophy

The Strike Force training device is designed to:
- **Withstand Impact**: Handle full-force punches and kicks from adult users
- **Maintain Stability**: Won't tip or move during vigorous training
- **Adjustable Height**: Accommodate users of different sizes (4ft - 6.5ft range)
- **Professional Appearance**: Modern aesthetic suitable for home or commercial gym
- **Easy Maintenance**: Modular design with replaceable components
- **Safe Operation**: Smooth surfaces, proper weight distribution, no pinch points

## Build Options

Four construction options are provided to suit different budgets and requirements:

1. **Budget Build** (~$500-900): Wood/metal hybrid, DIY-friendly
2. **Mid-Range** (~$900-1,450): Aluminum frame, good balance of quality and cost
3. **Professional** (~$1,900-3,150): Steel frame, maximum durability  
4. **Commercial Grade** (~$3,500-6,100): Premium materials, gym-quality finish

**Recommended for most users**: Option 2 (Aluminum Frame) - Best balance of durability, weight, aesthetics, and cost.

## Contributing

Contributions are welcome! Please submit pull requests to the appropriate repository:
- App features/fixes → strike_force_app
- Firmware improvements → strike_force_esp32
- Hardware design suggestions → manifest (this repo)

## Safety Notice

⚠️ **Important Safety Information**:
- This device is designed for martial arts training and can withstand significant impact
- Always ensure proper assembly and regular maintenance
- Check all connections before each use
- Maintain adequate clearance (6ft/2m radius) around the device
- Follow all safety guidelines in the hardware documentation
- Consult a professional if unsure about structural integrity

## License

[License information to be added]

## Support

For questions or issues:
- Open an issue in the appropriate repository
- Refer to HARDWARE_DESIGN.md for construction questions
- Check individual project READMEs for software-specific questions

## Project Status

🚧 **Active Development** - This project is under active development. Hardware designs are currently in documentation phase. Software components are functional but being actively improved.

## Version History

- v1.0 (2026-02-14): Initial hardware design documentation and manifest structure
