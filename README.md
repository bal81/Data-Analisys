# Data Analysis

This code was created to analyse different phase-space files created with Monte Carlo simulations for particle transport of mono-energetic protons beams in water.

The software Tool for Particle Transport (TOPAS) was used to transport mono-energetic protons beams in water. A surface scorer placed at the Brag Peak for each energy was used to record a phase space file, which involves the energy, time, and momentum of each particle traversing the surface scorer.

This code load three different phase-space files in order to analyse the final energy of the primary particles and their time of arrival at the Brag Peak (property inherent to charges particles).

Proton beams of 0.08, 1 and 5 MeV were analysed using a python program building in OOP able to load many phase-space files for their analysis. The class "Reader" open a single phase-space file and check for the existence of the file and if there is any null data on it. After that, it returns the energy and time parameters for each particle that traversed the scorer.

We observed that the energy spectra energy and time spectra become broader proportionally to the input energy leading to the conclusion that low energy protons can deposit their entire energy in a single interaction, creating an almost perfect pencil beam, while high energy proton (with initial energy above 1 MeV) reach the Brag Peak position with an energy of one order of magnitude lower than their input energy.
