# Monte Carlo-NVT
This repository serves as an illustrative example of an __NVT__ (constant Number of particles, constant Volume, and constant Temperature) __Monte Carlo (MC)__ calculation.

## Steps:

1. **Generate Atomic Coordinates:**
   - Generate coordinates for atoms within a cubic simulation box with a periodic boundary condition.
   - Simulation box edge length: 15 (all quantities in reduced Lennard-Jones units).
   - Achieve number density of 0.8.

2. **Lennard-Jones Interaction Potential:**
   - Implement the 6-12 Lennard-Jones interaction potential between atoms.
   - Utilize a potential truncated and shifted at a distance of 2.5.

3. **NVT Monte Carlo (MC) Simulation:**
   - Conduct NVT MC simulation, maintaining constant number of particles, volume, and temperature (Tr = 1.0).
   - The simulation will have the particle translationas the Monte Carlo moves (select a random particle and move randomely) to reach the equilibrium.

4. **Analysis and Comparison:**
   - Examine the radial distribution function (RDF) at the beginning and end of the simulation.
   - Compare RDF profiles to assess structural changes and equilibration.
   - Monitor the change of Energy with each move (How many MC moves does it take for the system to equilibrate at these conditions)

