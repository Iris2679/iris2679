# Objective
This project provides a Python script that generates a Tcl script for VMD to visualize dynamic community assignments of residues over time. Using a JSON file that contains residues assignment in communities over time, it allows users to color-code residues according to their community membership across different time frames. Each community is annotated with a number directly in the VMD model, enabling functional modules to be visually distinguished and traced throughout the trajectory. This visualization facilitates direct observation of structural rearrangements over time, supporting detailed analysis of both local residue interactions and global conformational changes.

# Required Inputs
- JSON file: Contains community assignments for residues over time frames. Example format: {"0": {"C1": [0,1,2]}}
- Structure file: .pdb or .gro file
- Trajectory file: .xtc file

# How to Use Python to Generate TCL
- Make sure the JSON file is saved in the same folder as the Python script.
- Open the Python file (py_to_tcl.py) in VS Code, IntelliJ, or Notepad++.
- Update the User Parameters section in the Python file with the correct file paths and variables.
- Run the Python script. This will generate a TCL file. Example result: a2b3_example.tcl

# HOW TO LOAD TCL in VMD
1. Load the structure file (.pdb or .gro file) in VMD: File -> New Molecule -> [filename]
2. Load the trajectory file (.xtc) on top of the structure file: File -> New Molecule -> [filename]
3. Source the TCL file in VMD main: Plugin -> TK console -> source /full/path/to/your/tcl/file.tcl

