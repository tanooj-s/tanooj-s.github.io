

I am a graduate student in the Materials Science and Engineering department at Rensselaer Polytechnic Institute, where I am a member of the [Virtual Materials Group](https://mse.rpi.edu/people/faculty/yunfeng-shi) and the [Ab-initio multi physics group](http://abinitiomp.org/), respectively coadvised by Yunfeng Shi and Ravishankar Sundararaman. 

My work focuses on using [molecular simulation](https://en.wikipedia.org/wiki/Molecular_dynamics) and machine learning to a) investigate physical mechanisms relevant for energy technologies at a microscopic scale and b) develop predictive methods to extrapolate quantum-level assumptions to bulk macroscopic properties. These molecular dynamics simulations can be used to model any kind of material (or chemically or biologically relevant microscopic system) at an atomic scale, so long as an accurate description of the interactions between constituent particles, a force field, is available. They can often serve as a useful computational microscope to investigate processes not accessible through experiment. 

[Computers have been used](https://pubs.aip.org/aip/jcp/article-abstract/31/2/459/1031509/Studies-in-Molecular-Dynamics-I-General-Method?redirectedFrom=fulltext) [to run such simulations](https://ui.adsabs.harvard.edu/abs/1960PhRv..120.1229G/abstract) [dating back to the 1950s](https://ui.adsabs.harvard.edu/abs/1964PhRv..136..405R/abstract), however appropriate force fields were only available for a relatively small class of materials. In the last 15 years or so, with the advent of machine learned force fields, this paradigm has changed. With appropriate training data it should in principle be possible to model any kind of system at an atomic level now, subject to computational tractability. 

I majored in Physics at UC Berkeley, after which I worked as a contractor at the [self-driving car project at Google X](https://waymo.com/) while it was being spun out into its own thing. After that I spent a couple of years doing tech work remotely and in India, after which I decided it was an appropriate time to go back to school.

All papers listed below are works in progress, although some are much further along than others. The molten salts work was presented at the [American Nuclear Society Winter Meeting 2022](https://www.ans.org/meetings/wm2022/session/view-1409/) and at [Argonne National Lab](https://www.anl.gov/our-history), and has been accepted for presentation at the [American Chemical Society Fall Meeting 2023](https://callforabstracts.acs.org/acsfall2023/I&EC). 


**First-principles molten salt phase diagrams through thermodynamic integration**<br>
*Tanooj Shah, Kamron Fazel, Jie Lian, Liping Huang, Yunfeng Shi, Ravishankar Sundararaman*<br>
Molten salts are a class of high-temperature ionic fluids that have recently attracted renewed interest due to their potential applications in modular nuclear reactors and thermal energy storage systems. A molten alkali halide salt (such as NaCl) can be used as a coolant instead of highly pressurized water in small modular reactors; these salts can also act as the medium in which fuel and fission products are dissolved. Accurate knowledge of the salt's phase diagram is critical to determine the operating conditions of such reactors, and computational predictions of the phase diagram can serve as an initial screen for such salts before more costly experimental validation. Precise prediction of phase diagrams in molecular dynamics simulations is challenging due to the simultaneous need for long time and large length scales and accurate interatomic potentials. We show that thermodynamic integration (TI) from low cost force fields to machine learned force fields trained using density functional theory (DFT) enables rapid first principles prediction of the solid-liquid phase boundary in NaCl. We use this technique to compare the accuracy of several DFT exchange-correlation functionals for predicting the NaCl phase boundary, and find that the inclusion of dispersion interactions is critical to obtain good agreement with experiment. Importantly, our methodology introduces an approach to predict solid-liquid phase boundaries for any material at an ab-initio accuracy, with the majority of the computational cost at the level of classical additive pairwise potentials. 


**Ab-initio liquidus line predictions and solubility limits in binary molten salt systems**<br>
*Tanooj Shah, Kamron Fazel, Jie Lian, Liping Huang, Yunfeng Shi, Ravishankar Sundararaman*<br>
The salts proposed to be used in small modular reactors are typically multicomponent mixtures such as FLiNaK. Here, using the model NaCl-MgCl2 system, we develop a free-energy method to obtain the state points (X, T) where a specified solid phase and the liquid mixture are in equilibrium (i.e. points along the liquidus line). We also adapt a method typically used by the biological community to calculate solvation energies of salt solutes - such a method can be used to estimate solubility limits of fission product solutes such as uranium chloride, and can guide selection of the salts used in such reactors. 



**[Improving the reliability of machine learned potentials for modeling inhomogenous liquids](https://arxiv.org/abs/2306.00970)**<br>
*Kamron Fazel, Nima Karimitari, Tanooj Shah, Chris Sutton, Ravishankar Sundararaman*<br>
Accurate models of the response of fluids to inhomogeneities in the environment (such as interfaces or solute particles) are critical to developing an enhanced understanding of electrochemical and biologically relevant processes at a microscopic scale. All-atom simulations allow direct access to these responses through the reconfiguration of solvent particles over the course of a molecular dynamics trajectory, however, these can be too computationally expensive to model certain processes (for example protein folding) over time scales of interest. On the other hand, implicit solvent models use a mean field approximation to model the response of these fluids as a functional of the density. Here we demonstrate the viability of using neural network potentials (NNPs) trained to external potentials in various geometries (as a generalization of different kinds of inhomogeneities) in order to develop such solvation models. 


**Improved machine learned potentials through delta learning**<br>
*Kamron Fazel, Tanooj Shah, Jie Lian, Liping Huang, Yunfeng Shi, Ravishankar Sundararaman*<br>
Machine learned force fields are gaining increasing adoption from the molecular simulation community. However, various schemes are used to make these force fields learn certain physically necessary aspects of the potential energy surface, such as repulsion at small interatomic distances, with no clear consensus about how to do this in the community. On the other hand, such physically necessary features are built into the functional forms of classical force fields. We introduce a scheme called delta learning, which trains a machine learned force field to learn the difference between a classical model and an ab-initio model. Such a resulting delta force field can be used as a first-principles correction overlaid on the classical potential. In order to test the viability of this approach, we compare certain bulk quantities between a classical pair potential, a conventional machine learned force field, and our delta learned force fields for the model NaCl system.


**In-silico evidence of current induced in graphene from the flow of an ionic solution**<br>
*Tanooj Shah, Yunfeng Shi*<br>
Experiments appear to indicate that the flow of an ionic solution such as seawater over a graphene sheet is able to generate a voltage, leading to the nascent field of hydrovoltaics. Current explanations of this phenomenon generally involve two components - how adsorbed ions at the interface move relative to the overall flow of the solution, and how delocalized electrons in graphene subsequently couple to and move along with the adsorbed ions. A full quantum-level investigation of this phenomenon is computationally intractable for the requisite time scales needed to establish a flow velocity comparable to experiment. We are developing methods to investigate this phenomenon from a purely classical perspective (stay tuned for more)

