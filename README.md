# LAMMPS Simulation of Water Freezing from 70K

## Project Description

This repository contains the input files for a LAMMPS simulation of the freezing behavior of a box of water molecules. The system is cooled to a target temperature of 70 Kelvin to observe crystallization.
This work serves as an example of setting up a basic molecular dynamics simulation for phase transitions.

## Prerequisites for LAMMPS

To run this simulation, you need to have a working installation of [LAMMPS (Large-scale Atomic/Molecular Massively Parallel Simulator)](https://www.lammps.org/).

## How to Run the Simulation

1.  Clone this repository:
    ```bash
    git clone https://github.com/IngawaleAryan/Water-freezing-LAMMPS.git
    ```
2.  Navigate to the project directory:
    ```bash
    cd Water-freezing-LAMMPS
    ```
3.  Run the LAMMPS simulation using the provided input script. The command may vary slightly depending on your LAMMPS installation and whether you are running in parallel:
    ```bash
    lmp -in input/in.water_70k
    ```
    Or for parallel execution (e.g., on 4 cores):
    ```bash
    mpirun -np 4 lmp -in input/in.water_70k
    ```

## File Descriptions

-   `input/in.water_70k`: The main LAMMPS input script. It defines the simulation parameters, fixes, and run commands.
-   `data/water.data`: The initial data file containing atomic coordinates and box dimensions for the water system.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
*(Note: It's good practice to add a LICENSE file. You can do this by clicking "Add file" -> "Create new file" and typing `LICENSE` as the name. GitHub will then give you templates to choose from. MIT is a great default.)*
