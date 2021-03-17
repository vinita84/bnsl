# Binary Nanoparticle Superlattices (BNSL) 

What does this code do
* The code simulates the assembly of two types of charged nanoparticles (NPs) into aggregates mediated by smaller, oppositely-charged linkers under different ionic physiological conditions. 

* The NPs are modeled after P22 virus-like particles (VLPs) of diameter 56 nanometers, and linkers represent smaller nanoparticles (dendrimers) of 6 nanometer diameter. 

* Simulations are performed using LAMMPS; pre- and postprocessing are done using C++ codes. 

* Simulation results are tested and validated using SAXS and dynamic light scattering measurements of the VLP aggregates; experiments also guide the model design.

Local install and testing (after loading the needed modules):
* module load gsl && module load openmpi/3.0.1 && module load boost/1_67_0
* from root (bnsl) directory: make local-install 
* cd bin/
* to test 1:1 systems: make run-preprocessor r=1 
* to test 1:4 systems: make run-preprocessor r=4

### nanoHUB app page:
* https://nanohub.org/tools/bnsl

<!--- * Users can input control parameters such as NP charge (from -500e to -1500e), linker density (from 25X to 100X the NP density), and ionic strength (from 0.01 M to 0.3 M) to predict formation of NP aggregates. ---!>

<!--- * This information may be useful in designing NP features to produce desired effects when NPs interface with biological entities. Outputs are structural information such as pair correlation functions (often denoted as g(r)) and simulation snapshots (with only NPs shown for clarity). The NPs are modeled after P22 virus-like particles (VLPs) of diameter 56 nanometers, and linkers represent smaller nanoparticles (dendrimers) of 6 nanometer diameter. Linker charge is fixed to about 35e. ---!>

<!--- * At the end of simulation run, which will take close to 60 minutes, g(r) will be produced in the "Pair Correlation" tab. ---!>

<!--For further details please refer to the [documentation](https://softmaterialslab.github.io/bnsl/)--!>


