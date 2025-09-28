# Objective
This project provides a Python script that generates a Tcl script for VMD to visualize dynamic community assignments of residues over time. Using a JSON file that contains residues assignment in communities over time, it allows users to color-code residues according to their community membership across different time frames. Each community is annotated with a number directly in the VMD model, enabling functional modules to be visually distinguished and traced throughout the trajectory. This visualization facilitates direct observation of structural rearrangements over time, supporting detailed analysis of both local residue interactions and global conformational changes.

# Required Inputs
- JSON file: Contains community assignments for residues over time frames. Example format: {"0": {"C1": [0,1,2]}}
- Structure file: .pdb or .gro file
- Trajectory file: .xtc file

# HOW TO USE python to generate tcl
- make sure ot have JSON file to be saved in the same folder as python file
- Open python file in VS Code, IntelliJ or notepad++
- Change variables/and file directory in User parameters section in python file
- 

# HOW TO LOAD TCL in VMD
1. Load .pdb/.gro file in VMD (file -> New Molecule -> filename)
2. Load .xtc file on the structure file (file -> New Molecule -> filename)
3. source /full/path/to/your/tcl/file

