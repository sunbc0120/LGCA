LGCA
====

Adsorption Isotherm and Kinetics Emulation with Lattice Gas Cellular Automata:

Adsorption phenomena are increasingly utilized to perform separation processes, adsorption chilling, hydrogen driven vehicle and more recently gas storage. The physical adsorption process occurs mainly within the pores of the external adsorbent surface due to van der Waals force field. The amount of adsorbate uptake depends on the nature of adsorbates and the porous adsorbent structure. For higher adsorptive capacity, the adsorbents should have a high surface area and/or high micropore volume, with an optimum pore width distribution that spans from super micropore to mesopores. However, the porous medium is naturally associated with very small pores and adsorbate molecules have to find their way to the interior surface area or micropore volume. This path-finding gives rise to the so-called diffusional resistance towards molecular flow within scope of adsorption kinetics.

Lattice Gas Cellular Automata (LGCA), as a fluid dynamic simulation method that is conceptually simple, can be applied to deal with thermal interface effects to a wide array of boundary conditions. Based on LGM, lattice Boltzmann Method (LBM) has been successfully used to model a number of typical fluid dynamic problems within macroscope. In this project, however, we extend LGM into microscopic scale to deal with surface adsorption problems including its isotherm and kinetics.

To express the evolution, 6 bit digit is used: 

0 for empty

1 for gas particle movement

2 for surface wall

3 for gas particle move onto the wall

4 for gas adsorbed by the surface wall

5 for gas particle move onto the adsorbed gas
	
Construct 2D porous network structure of adsorbent material surface: 

        Parameters corresponding to pore width and/or volume distribution

        Reflect nano-porous structure of activated carbon, zeolite, etc.
	
Implement lattice gas fluid CA model which incorporates: 
        
        Local rules of lattice gas collision and movement

        Periodic space boundary conditions

        Issues regarding to hexagonal grids topology and geometry (6 bit digit and hexagonal, rule space will be 6^6)
	
Defining local rules of lattice gas interaction with material surface boundaries:

        Probabilistic adsorption of lattice gas (adsorption potential with relation to temperature) onto different surface boundary conditions (1~6 walls)

        Diffusion resistence onto LGM within porous surface structures*
	
Visualize the LGCA emulation result:

        Relationship between the uptake of LG onto the surface and the initilized LG density, this corresponds to adsorption isotherm
	
        Dependence of the uptake of LG on the LGCA running steps, this reflects the adsorption kinetics
