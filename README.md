This repository contains the data cards used for Monte Carlo (MC) production with MadGraph 3.5 and Pythia8, along with detector simulation handled by Delphes. The project focuses on the four-top-quark differential cross-section with SMEFT (Standard Model Effective Field Theory) contributions.

There are two categories of samples: Signal and Background. For signal samples, six data cards are required for the full simulation: run_card.dat, param_card.dat, madspin_card.dat, reweight_card.dat, configLHE_template.cmnd and delphes_card.tcl. For background samples, five data cards are needed: run_card.dat, param_card.dat, madspin_card.dat, configLHE_template.cmnd and delphes_card.tcl.

Here’s a clearer description of each card and its purpose:

1) run_card.dat: Contains the process information, such as the center-of-mass energy for the event and the choice of Parton Distribution Function (PDF).

2) param_card.dat: Specifies parameter values in the model, including constants like the Yukawa coupling and the values for Wilson coefficients used in SMEFT studies.

3) madspin_card.dat: Defines particle decay modes, such as top quark and W boson decays, to control which particles decay and how they decay in the simulation.

4) reweight_card.dat: Specifies reweighting parameters, allowing changes in parameter values for different physics scenarios. For instance, starting from the Standard Model (SM) with       ctt1=10^-10, the reweighting card can request alternative values, like ctt1=-1.0 or ctt1=1.0, for comparative analysis.

5) configLHE_template.cmnd: Provides configuration details for Pythia8, including parton shower uncertainties and additional decays for particles like the Higgs boson.

6) delphes_card_CMS_PileUp_4T.tcl: Configures Delphes for detector simulation, specifying options like whether pileup effects are included and details on detector resolution.
