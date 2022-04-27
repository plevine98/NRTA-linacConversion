# NRTA-linacConversion
bremsstrahlung x-ray and photodisintegration neutron energy spectra for linac electron-to-neutron conversion
from SM/SB thesis:
Feasibilty study of compact Neutron Resonance Transmission Analysis using a linac, a fusion-based neutron generator, and an isotopic source
2022

These data are particle energy spectra for the bremsstrahlung and photodisintegration steps of the electron-to-neutron conversion process for NRTA using an electron linear accelerator. 60 million electrons were simulated in Grasshopper, a Geant4-backed Monte Carlo simulation engine. Monoenergetic linac beam energies of 3.0 to 5.0 MeV were simulated. There are two folders of data files:

brem_data
contains the bremsstrahlung x-ray energy spectra by linac beam energy. The beam energy is provided in the file name, without a decimal. For example, the 3.0 MeV beam contains "30" in the file name, and 3.5 MeV contains "35." The first column provides histogram bin edges in energy MeV. The second column provides the number of bremsstrahlung x-rays in the energy bin from the simulation. The counts come from 60 million simulated electrons.

photodisintegration_data
contains the total, unmoderated neutron energy spectra by linac beam energy. The beam energy is provided in the file name, without a decimal. For example, the 3.0 MeV beam contains "30" in the file name, and 3.5 MeV contains "35." The first column provides histogram bin edges in energy MeV. The second column provides the number of neutrons in the energy bin from the bremsstrahlung simulations weighted by ENDF cross section in that energy bin. Neutron energies E_n have been calculated from x-ray energy E_x according to the equation: E_n = ( E_x - Q ) / 2 where Q = 2.2246 MeV, the Q-value of the photodisintegration reaction in heavy water. The factor of 2 comes from energy splitting evenly between the daughter neutron and proton. The counts come from the simulation with 60 million electrons.
