# AO-Fluence-Model-WS2

VLEO Atomic Oxygen Fluence Model 
Created by Pratyush Majumdar for WolfSat-2

Date: May 14 - June 20th.

Note on date: This project marks my early transition into aerospace coding, so some comments can be considered over-explanatory for what they are. That being said, I’ve kept the original comments intact as a reflection of my learning process and problem solving.

Atomic oxygen is a single, unpaired Oxygen atom that is extremely unstable and reactive. It is well documented to cause fast oxidation of spacecraft surfaces, especially in VLEO and LEO orbit environments, where it is in exponentially greater quantities than those of higher altitudes.

This is a python representation of an atomic oxygen fluence model, following the process described in this paper: https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2020JA027944
Immense credit to the authors G. Schumm, J. W. Bonnell, J. R. Wygant, and F. S. Mozer, because this model would not have been possible without this document.

This model approximates oxygen particle collisions through a process of summing vectors and coordinate transformations that creates what would happen if gas particles impacted an ideal surface at different orientations.
This model uses:

 -- NRLMSIS Data
 -- Rodrigues's Rotation Formula
 -- Astropy and Poliastro for orbit propagation
 -- A stand in date for the actual WS-2 launch date, as the true date does not have any atmospheric data for it. 

Mission:
The Wolfsat-2 is is a 1U CubeSat mission designed to test the viability of using a wood chassis rather than the usual metal.
It operates in a very low Earth orbit (~230 km). The orbit is effectively circular for atmospheric purposes.
This model estimates the RPM as constant.

- All physics equations, logic, and modeling were developed (or researched) by the author.
- Artificial Intelligence was used in order to debug and fix errors in the code.
- The simulation is intended for early-phase atomic oxygen analysis of Wolfsat-2.
