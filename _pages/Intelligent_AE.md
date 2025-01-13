---
layout: archive
title: "Intelligent Acoustic Emission Monitoring"
collection: research
permalink: /research/Intelligent_AE/
---

## AE-PNet: A Deep-Learning P-Wave Arrival Picker for Laboratory Acoustic Emissions
<p align="justify">
The effective stress concept and the poromechanical framework pioneered by Terzaghi and Biot have been widely adopted to illustrate coupled fluid flow and solid deformation in porous rocks, but there were still some links missing for anisotropic and ductile rocks like shale. There hardly exists complete discussions in existing research work on poromechanical formulations that consider material anisotropy, elastoplastic, and grain compressibility, and they are all critical components in quantifying the hydromechanical processes in transversely isotropic rocks. Based on the mixture theory and continuum thermodynamics, I derived a novel mathematical framework for coupled solid deformation and fluid flow with all of the aforementioned factors addressed[1].  
</p> 
<p align="justify">
The proposed framework involves a new set of governing equations for mass conservation of fluid and solid, and a new effective stress formulation that identifies distinct forms of effective stress for elastic response and plastic response respectively. Coefficients that emerge in the governing equations are evaluated naturally through the derivation, thus the proposed framework won’t require any additional constitutive law or assumption for parameter evaluation. For this work, I also developed a mixed finite element framework for its numerical implementation and conducted simulations of a consolidation problem with strip loading to reveal the unique hydromechanical response in anisotropic elastoplastic porous rocks, as demonstrated in the ensuing figures.   
</p>

<img src="/images/AEPNET.jpg"/>  
<h6 align="center">Setup of the consolidation problem in a transversely isotropic medium under a strip load.  
</h6>

<img src="/images/Input & output_AEPNET.jpg"/>  
<h6 align="center">Evolution of ground settlement and pore pressure.  
</h6>

## Stanford Acoustic Emission Data set [(SAED)](https://purl.stanford.edu/mz374gr4108)
<p align="justify">
The figures below demonstrate the influence of elastoplasticity on the consolidation process in the domain. In elastic domain, the pore pressure build-up and the ground settlement is the least, while for normally consolidated medium with p<sub>c0</sub>=-1MPa, the material is the weakest and the domain undergoes largest pore pressure accumulation and ground settlement. For overconsolidated medium with p<sub>c0</sub>=-2MPa, the evolution of pore pressure and ground settlement lie in between the other two scenarios.  
</p>

<img src="/images/Input & output_AEPNET.jpg"/>  
<h6 align="center">Evolution of ground settlement and pore pressure.  
</h6>

<p align="justify">
The following two sets of figures demonstrate contours of pore pressure and Darcy velocities for various cases, where a unique response in domains made up of  overconsolidated materials has been observed. For such cases, plastic dilation in regions beneath the strip load leads to an arc-shaped pore pressure distribution accompanied with and an eddy-shaped Darcy velocity distribution.   
</p>


## AE P-wave arrival picking platform
<p align="justify">
I have developed a novel continuum poromechanical framework for shale considering the bimodal pore size distribution from the existing form of voids in shale as either microcracks or nanopores. Specifically speaking, I extended the framework discussed in the previous section with the double porosity theory, which allows for the consideration of different permeability and constitutive law for fluid flow at different pore scales[2]. This work is the first of its kind to integrate factors including anisotropy, elastoplasticity, and double porosity in the analysis of hydromechanical responses of shale. 
</p>
<img src="/images/Picking Platform_V1.jpg"/>  
<img src="/images/Picking Platform_V2.jpg"/> 
<h6 align="center">Illustration of the double porosity concept.   
</h6>
<p align="justify">
The figure above demonstrates the concept of double porosity, where the voids can be separated into two continuous porous network consists of pores with different length scales. In macropores made up of microcracks, we consider the fluid flow inside is anisotropic, with a preferred flow direction along the crack planes. In micropores, we assume the fluid flow is isotropic. With this proposed framework, I reproduced the 1-D consolidation process of Opalinus shale, and the setup of the problem as well as the loading protocol is demonstrated in the figure below:  

## Reference:
\[1\] <b>Guo T.Y.\*</b>, Vanorio T., $ Jihui D. (2024). A Deep-learning P-wave Arrival Picker for Laboratory Acoustic Emissions: Model Training and its Performance. <i>Rock Mechanics and Rock Engineering</i>. 1-19. [https://doi.org/10.1007/s00603-024-04296-5](https://doi.org/10.1007/s00603-024-04296-5)  
\[2\] <b>Guo T.Y.\*</b>, Vanorio T., $ Jihui D. (2024). Stanford Acoustic Emission Data set. <i>Stanford Digital Repository</i> [https://purl.stanford.edu/mz374gr4108](https://purl.stanford.edu/mz374gr4108)  
