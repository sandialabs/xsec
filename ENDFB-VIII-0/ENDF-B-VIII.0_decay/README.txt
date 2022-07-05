ENDF/B-VIII.0 Decay Sublibrary README
=======================================

Author: D.A. Brown, NNDC, BNL
Affiliation: NNDC, Brookhaven National Laboratory
Date: 2 Feb 2018

In the ENDF/B-VIII.0 release, the decay data sublibrary underwent a number of
checks and updates, mainly on the beta intensities following beta-minus decay,
X-ray energies for actinide nuclides, and some error fixes.
As in the previous library release, beta intensities from Total Absorption Gamma
Spectroscopy (TAGS) experiments were incorporated in order to improve the
electron and antineutrino spectra predictions following fission.  Additionally,
for another set of neutron-rich nuclides lacking TAGS data and yet deemed
important in antineutrino spectra applications, beta intensities obtained from
adjusting the electron spectra measured have been used.

Another update had to do with X-ray energies, which are produced following decay
under two circumstances, electron capture or electron conversion.  These
processes create vacancies in the atomic orbitals, and as these vacancies are
filled, X-rays and Auger electrons are emitted.  For ENDF/B-VII.1, LLNL’s EADL
data, also part of the ENDF/B library, were used to calculate the energy and
intensity of the transitions.  The energies are calculated by a simple
difference of the atomic shell binding energies listed in EADL.  However, it
was noticed that the K_alpha1 X-ray energy for Uranium was shifted by +0.4 keV.
An interim solution was implemented for ENDF/B-VIII.0, where K X-ray energies
from the NIST X-ray Transition Energy Database were used, for decay datasets
with Z=89-96.

Finally, the datasets for the following nuclides were corrected: 86As, 98mY,
149mEr, 209Rn, 220Fr, 177Ir, 203Po, 224Ac, 231U, 236mNp, 239Am, and 253Es.

The decay sublibrary is detailed in

* D. Brown, et al. "ENDF/B-VIII.0: The 8th Major Release of the Nuclear
  Reaction Data Library with CIELO-project Cross Sections, New Standards
  and Thermal Scattering Data," Nuclear Data Sheets 148, 1 (2018).
