# MD-S-protein-PLA

This repository contains molecular dynamics simulation data and analysis results for the manuscript:

**"In-silico Study of SARS-CoV-2 Spike Glycoprotein - Polylactic Acid Surface Interaction at Varying Temperatures"**

## Repository Overview

This repository shares simulation data and relevant analysis results from molecular dynamics (MD) simulations investigating the interaction between SARS-CoV-2 spike glycoprotein and polylactic acid (PLA) surfaces at different temperatures.

## Repository Structure

```
MD-S-protein-PLA/
├── Simulation/
│   ├── 3deg/
│   ├── 24deg/
│   └── 50deg/
└── Analysis/
    ├── H-bonds/
    │   ├── 3deg/
    │   ├── 24deg/
    │   └── 50deg/
    ├── mindist/
    │   ├── 3deg/
    │   ├── 24deg/
    │   └── 50deg/
    ├── MMPBSA/
    │   ├── 3deg/
    │   ├── 24deg/
    │   └── 50deg/
    ├── RMSD/
    │   ├── 3deg/
    │   ├── 24deg/
    │   └── 50deg/
    └── RMSF/
        ├── 3deg/
        ├── 24deg/
        └── 50deg/
```

## Data Description

### Simulation Data

The `Simulation/` folder contains MD simulation files organized by temperature:

- **3deg/**: Simulation data at 3°C
- **24deg/**: Simulation data at 24°C  
- **50deg/**: Simulation data at 50°C

Each temperature subfolder contains:

| File Type | Description |
|-----------|-------------|
| `.pdb` | Initial protein structure at 0 ns |
| `.tpr` | Portable binary run input file (GROMACS topology and parameters) |
| `.xtc` | Compressed trajectory file (protein coordinates only) |

### Analysis Data

The `Analysis/` folder contains post-processing analysis results organized by analysis type and temperature:

- **H-bonds/**: Hydrogen bonding analysis between spike protein and PLA surface
- **mindist/**: Minimum distance calculations between protein and substrate
- **MMPBSA/**: Molecular Mechanics Poisson-Boltzmann Surface Area binding energy analysis
- **RMSD/**: Root Mean Square Deviation analysis of protein backbone 
- **RMSF/**: Root Mean Square Fluctuation analysis of protein residues during the last 500 ns of simulation

Each analysis subfolder is further organized by temperature (3deg/, 24deg/, 50deg/) containing the corresponding analysis output files.

## File Access and Additional Data

**Note**: The trajectory files provided contain protein coordinates only. For access to:
- Complete system trajectory files including PLA substrate
- Additional simulation files
- Raw data files

Please contact: **karin.hasegawa@stonybroook.edu**

## Usage Guidelines

### File Formats
- **PDB files**: Can be opened with molecular visualization software (PyMOL, VMD, ChimeraX)
- **TPR files**: GROMACS binary files containing simulation parameters
- **XTC files**: GROMACS compressed trajectory files (require GROMACS or compatible software)

## License

This project is licensed under the MIT License. See LICENSE for details.
