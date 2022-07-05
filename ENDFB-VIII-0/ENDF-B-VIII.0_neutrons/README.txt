ENDF/B-VIII.0 Neutron Sublibrary README
=======================================

Author: D.A. Brown, NNDC, BNL
Affiliation: NNDC, Brookhaven National Laboratory
Date: 2 Feb 2018

CSEWG announces the release of ENDF/B-VIII.0!  ENDF/B-VIII.0 fully incorporates
he new IAEA standards and uses new evaluated data from the CIELO project for
neutron reactions on 16O, 56Fe, 235U, 238U and 239Pu.  The evaluations benefit
from recent experimental data obtained in the U.S. and Europe, and improvements
in theory and simulation.  Notable advances include updated evaluated data for
light nuclei, structural materials, actinides, fission energy release, and
prompt fission neutron and gamma-ray spectra.  We performed integral validation
testing on a wide range of criticality, reaction rate, and neutron transmission
benchmarks.  In general, our integral validation demonstrates that performance
of the library is a noticeable improvement over the previous ENDF/B-VII.1
library.  The neutron sublibrary is detailed in several Nuclear Data Sheets
papers:

* D. Brown, et al. "ENDF/B-VIII.0: The 8th Major Release of the Nuclear
  Reaction Data Library with CIELO-project Cross Sections, New Standards
  and Thermal Scattering Data," Nuclear Data Sheets 148, 1 (2018).

* M.B. Chadwick, et al., "CIELO Collaboration Summary Results: International
  Evaluations of Neutron Reactions on Uranium, Plutonium, Iron, Oxygen and
  Hydrogen,"  Nuclear Data Sheets 148, 189 (2018).

* M. Herman, et al., "Evaluation of Neutron Reactions on Iron Isotopes for
  CIELO and ENDF/B-VIII.0," Nuclear Data Sheets 148, 214 (2018).

* R. Capote, et al. "IAEA CIELO Evaluation of Neutron-Induced Reactions on 235U
  and 238U Targets for Incident Energies up to 30 MeV," Nuclear Data Sheets 148,
  254 (2018).

* D. Neudecker, et al. "Evaluations of Energy Spectra of Neutrons Emitted
  Promptly in Neutron-induced Fission of 235U and 239Pu," Nuclear Data Sheets
  148, 293 (2018).

The library as a whole is available at http://www.nndc.bnl.gov/endf/b8.0/


Comments about the covariance in current ENDF evaluations
---------------------------------------------------------

1.  The covariance data in the ENDF evaluations represents uncertainties and
    correlations in differential data.
2.  The use of this covariance to calculate uncertainties for integral
    quantities such as Keff will usually result in an overestimate of the
    uncertainty.  That said, comparisons to integral data are essential during
    the evaluation process and users should not be surprised if the
    *mean value* nuclear data allow for the accurate prediction of Keff, even
    if the covariances to not reflect this consideration.
3.  The recommended methodology to overcome this problem is to adjust the
    covariance to add information from set of integral data that represents the
    physics of the system for which the adjusted covariance will be used.
4.  More information on this topic: https://www.oecd-nea.org/science/wpec/sg33/
5.  CSEWG is currently studying the best covariance representation for future
    releases.
