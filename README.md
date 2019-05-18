# MCCG
Repository for the Monash computational chemistry group

<!-- # Cloning -->
<!-- If cloning this repository, use `git clone --recurse-submodules https://github.com/tommason14/mccg`, as qcp is added as a submodule from another repository -->

# Automating workflows

## qcp - Quantum Chemical Processor
Automate processes such as 
- creating input and job files
- recursive parsing of log files
- recursive submission of jobs, deletion of queued jobs
- Finding bond distances of xyz files

Currently installed on Raijin, Magnus, Monarch, Massive and Stampede. Implemented for GAMESS, PSI4 and Gaussian calculations

## PHMD- generation of LAMMPS input files
Scripts to generate a LAMMPS input file, along with a data file containing the appropriate force field parameters, given an xyz file with numbered atoms. Uses a python script to fill a blank data file generated by vmd, with a dictionary populated with the required force field parameters. See the readme in the folder for more details.



## view_hessian_calculation.ipynb
Takes a GAMESS log file as an input and produces an infrared spectra along with a molecule viewer to view all the vibrational modes of files generated using the FMO approach.

## gamess_to_molden.py
Parse GAMESS log files for use with [molden](http://cheminf.cmbi.ru.nl/molden/), allowing for easy viewing of geometries, convergence, frequencies and vibrational modes generated using the FMO approach (also works with non-FMO).

Useful when generating IR spectra as molden automatically fits Lorentzian curves to the intensities found from the Hessian.

# Input files and job scripts
Example files are stored in the templates folder.

# Python tutorial
Have a look through this [tutorial](python_tutorial.md) for some useful tips on using Python. 

# Compiling software
See [this page](compilation.md) for information on how to compile various programs.

# Useful commands
See [here](useful_commands.md) for useful commands.

# System admin
Use [folder_sizes.py](folder_sizes.py) to obtain the sizes of each folder in
the current directory. Useful for logging scratch space usage. (May throw errors if directory names contain spaces)


