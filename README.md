# Dual ADC Board PCB Design
![Alt text](Images/3D.png)
## Overview
The ADC module in this project is intended to collect two signals and pass the data to a pin header, which could then connect to an external board like a microcontroller module. 
The module will include the following set of major components:
 - **ISL75051ASEHVFE** - Rad-hard 5V to 3V3 power regulator module.
 - **ADC128S102CIMTX** - 8-Channel, 0.5 to 1 MSps 12-bit ADC.
 - **AMC1203BPSA** - Single-channel 40 kSps 8-bit sigma-delta isolated current-sensing ADC.
 
The two main portions of the schematics for this module are the isolated and non-isolated ADCs.
The PCB was designed using Altium Designer 23, based on the schematic provided in Zachariah Peterson tutorial ([altium.com]([https://www.youtube.com/watch?v=wCYNTt5krDM&ab_channel=Phil%E2%80%99sLab](https://resources.altium.com/p/dual-adc-module-pcb-design-project#starting-the-adc-module))).

## Project Highlights

- **4-Layer PCB Design**: Designed a 4-layer board with a dedicated ground reference plane for improved signal integrity and noise reduction in order to prevent inductive coupling between analog and digital sections.
- **Layer Stack**: SIG+PWR / GND / GND/ SIG (we do not have controlled impedance requirements).
- **Material Specifications**: Utilized FR4 material with a thickness of 1.6mm.
- **Library Management**: Extracted and refined all component libraries in accordance with datasheet specifications and IPC standards.
- **Design Rule Compliance**: Ensured all design rules were meticulously followed as per IPC guidelines.
- **Manufacturing Outputs**: Generated comprehensive Gerber files and automated assembly files to facilitate seamless manufacturing and assembly processes.

## Repository Folder Contents

- `Assembly/`: Pick and Place information for SMT machine process.
- `BOM/`: Bill of materials listing all components used in the design.
- `Gerber/`: Manufacturing Files, PCB stack-up and layer information.
- `Images/`: Board Images 2D and 3D.
- `Mechanical/`: Contains files for mechanical design such as 3D STEP and DWG of Board.
- `Reports/`: Contains DRC and ERC status.
- `Schematic/`: Detailed schematic of the Class-D amplifier circuit.
- `Source Files/`: Directory containing Altium Designer project files.
- `CHANGELOG.md`: Documentation of changes and updates made throughout the project.
- `LICENSE`: License information for the project.

## Tools Used

- **PCB Design Software**: Altium Designer 22 and Viewmate (for gerber verification)

## Acknowledgments

The schematic design for this project was adapted from Resources > Altium Designer Projects > Dual ADC Module PCB Design Project; by Zachariah Peterson.
## About Me

I am a PCB design engineer with a focus on creating efficient and reliable layout designs. For more about my professional background, please visit my LinkedIn profile: [Vijayalakshmi M](https://www.linkedin.com/in/vijayalakshmi-m-542050314).

## License

This project is licensed under the [MIT License](LICENSE).

---

*Note: This project is intended for educational and demonstration purposes. The schematic design credits go to Altium.*
