# Data cards for Monte Carlo production - TTTT_5f_SMEFT and Background samples.

This repository contains the data cards used for Monte Carlo (MC) production with MadGraph 3.5 and Pythia8, along with detector simulation handled by Delphes. The project focuses on the four-top-quark differential cross-section with SMEFT (Standard Model Effective Field Theory) contributions.

There are three categories of samples: Signal, Background and Validation. For signal samples, six data cards are required for the full simulation: **run_card.dat**, **param_card.dat**, **madspin_card.dat**, **reweight_card.dat**, **configLHE_template.cmnd** and **delphes_card.tcl**. For background and validation samples, five data cards are needed: **run_card.dat**, **param_card.dat**, **madspin_card.dat**, **configLHE_template.cmnd** and **delphes_card.tcl**.

**Data cards description**

*  **run_card.dat**: Contains the process information, such as the center-of-mass energy for the event and the choice of Parton Distribution Function (PDF).

*  **param_card.dat**: Specifies parameter values in the model, including constants like the Yukawa coupling and the values for Wilson coefficients used in SMEFT studies.

* **madspin_card.dat**: Defines particle decay modes, such as top quark and W boson decays, to control which particles decay and how they decay in the simulation.

* **reweight_card.dat**: Specifies reweighting parameters, allowing changes in parameter values for different physics scenarios. For instance, starting from the Standard Model (SM) with       $c_{tt1}=10^{-10}$, the reweighting card can request alternative values, like $c_{tt1} = -1.0$ or $c_{tt1} = 1.0$, for comparative analysis.

* **configLHE_template.cmnd**: Provides configuration details for Pythia8, including parton shower uncertainties and additional decays for particles like the Higgs boson.

* **delphes_card_CMS_PileUp_4T.tcl**: Configures Delphes for detector simulation, specifying options like whether pileup effects are included and details on detector resolution.

**Signal samples description** 

* `tttt_w_minus` : An exclusive sample where the $W^{-}$ boson from the top decay is forced to decay to leptons, while the $W^{+}$ boson is allowed to decay into all possible particles.

* `tttt_w_plus` : An exclusive sample where the $W^{+}$ boson from the top decay is forced to decay to leptons, while the $W^{-}$ boson is allowed to decay into all possible particles.

**Background samples description** 

* `ttw_minus` :  An exclusive sample where the $W^{-}$ boson is forced to decay to leptons, while the $W^{+}$ boson is allowed to decay into all possible particles.

* `ttw_plus` :  An exclusive sample where the $W^{+}$ boson is forced to decay to leptons, while the $W^{-}$ boson is allowed to decay into all possible particles.

* `ttH_to_ZZ` :  An inclusive sample where the $W^{±}$ bosons are allowed to decay into all possible particles, the Higgs boson ($H$) decays exclusively to $ZZ$, and each $Z$ boson can decay into all possible particles.

* `ttH_to_WW_minus` :  An exclusive sample where the $W^{-}$ boson is requierd to decay leptons, while the $W^{+}$ boson is allowed to decay into all possible particles. The Higgs boson ($H$) decays exclusively to $W^{+}W^{-}$.

 * `ttH_to_WW_plus` :  An exclusive sample where the $W^{+}$ boson is requierd to decay leptons, while the $W^{-}$ boson is allowed to decay into all possible particles. The Higgs boson ($H$) decays exclusively to $W^{+}W^{-}$.

**Validation samples description**

 * `tt_W_minus` :  A NLO exclusive sample where the $W^{-}$ boson is requierd to decay leptons, while the $W^{+}$ boson is allowed to decay into all possible particles. This ensures that there is at least one charged lepton in the final state. These samples include three top mass hypotheses: $m_{t}=171.5$ GeV, $m_{t}=172.5$ GeV and $m_{t}=173.5$ GeV.

 * `tt_W_plus` :  A NLO exclusive sample where the $W^{+}$ boson is requierd to decay leptons, while the $W^{-}$ boson is allowed to decay into all possible particles. This ensures that there is at least one charged lepton in the final state. These samples include three top mass hypotheses: $m_{t}=171.5$ GeV, $m_{t}=172.5$ GeV and $m_{t}=173.5$ GeV.

