---
layout: default
title: Research
permalink: /work projects
---


# I Adaptive Wavelet Enhancement method

In this work, I develop an innovative optimization method to adaptively enrich the accuracy of crystal plasticity simulation while limiting the computational cost. Modeling complex polycrystalline microstructure requires a fine discretization to ensure satisfactory accuracy, which ultimately impacts the computational cost. This is especially critical for problems introducing phenomenology with localization, such as shear banding, twinning or fracture. I develop a new method based on second generation wavelets to enrich finite element simulations.
<img src="https://azdoud.github.io/images/enrich-p2.png" width="280" style="float:right; margin: 1em 0 4em 2em;"
title="the enrichment nodes are located where needed for this polycrystalline structure"/>
In this new method, a wavelet decomposition scheme is used to analyze error indicators in order to provide a basis of enrichment functions. The wavelet family is chosen such that the enriching function constitutes a hierarchical finite element basis. These functions are introduced adaptively in the FEM scheme to locally enrich the solution. The particularity of this method is that the adaptive scheme is consistent with the error analysis.

This is currently a work in progress but it has been favorably received in the community through conference [1] and reports [2, 3]. I am currently preparing 2 publications on this subject that are expected for submission in 2016.

**Resources**

* Conference and report meetings:

[1] Y.Azdoud, J.Cheng, S. Ghosh, The Adaptive Wavelet Enhancement for Crystal Plastic Finite Element Method, 13th US National Congress on Computational Mechanics, San Diego, CA (2015)

[2] S.Ghosh, Y. Azdoud, Advancing Computational Methods for Image-based Modeling of Polycrystalline Metallic Material, AFOSR 2015 Multiscale Structural Mechanics Annual Grantees Meeting, Fort Walton, FL (2015)

[3] S.Ghosh, Y. Azdoud, Advancing Computational Methods for Image-based Modeling of Polycrystalline Metallic Material, AFOSR 2014 Multiscale Structural Mechanics Annual Grantees Meeting, Albuquerque, NM (2014)








# II Adaptive coupling for fracture and damage.





In this work, I designed a new method for simulating fracture and damage using a hybrid local/non-local model. The morphing method is used to seamlessly link the local and non-local region that are adaptively defined following non-local (in the case of fracture [1]) or local (in the case of damage [2,3]) evolution criteria. Discontinuous Galerkin Finite Element Method (DGFEM) is used in the non-local region to allow failure induced discontinuities. In [1], a seed region is defined where fracture initiation is likely to occur, and propagation of the region is handled by maintaining a characteristic distance to the crack nucleation area. I demonstrate that the adaptive scheme does not interact with the crack propagation phenomenology by using a 3D CT test. I also demonstrate mesh independence.
<img src="https://azdoud.github.io/images/frac-dam.png" width="280" style="float:right; margin: 1em 0 4em 2em;"
title="crack intereaction in the adaptive hybrid local damage non-local fracture model"/>
In [2,3], I extend the concept to damage continuum. I couple local damage to non-local fracture in order to handle softening by the non-local model, while initiation and hardening is predicted by the local model. The adaptive local/non-local partition is controlled by a local criterion dependent upon the value of the local damage indicator. In that case, no seed region is required. A simple one variable local damage model with hardening is taken. Demonstration is given using a simple 3D traction test.


**Resources**

* Journal Papers:

[1] Y. Azdoud, F. Han, G. Lubineau, The morphing method as a flexible tool for adaptive local/non-local simulation of fracture, Computational mechanics, Vol 54, 711-722, (2014)

[2] F. Han, G. Lubineau, Y. Azdoud, Adaptive coupling between damage mechanics and peridynamics: a route for objective simulation of material degradation up to complete failure, Journal of the Mechanics and Physics of Solids, (2016)

* PhD thesis:

[3] Y.Azdoud, A hybrid local/non-local framework for the simulation of damage and fracture, 2014


# III Coupling Local and Non-local Models: The morphing method

In this work, I designed a new type of coupling method between the classic continuum theory and integral non-local models such as peridynamics. The motivation of such method is to reduce computational cost when using peridynamics by restricting the domain of application, and to provide simple boundary conditions. In [1], I developed the morphing method based on an energy density constraint at the local level. A smooth transition between local model and non-local model is achieved by introducing a coupling parameter, alpha(x), in the hybrid constitutive equation. The coupling is achieved in a thick coupling zone, where alpha(x) varies, surrounding the pure non-local patch.
The paper [1] demonstrates the effectiveness of the method for 2D cases, and gives an interpretation to the coupling error in an analytical 1D case. The paper [2] extends the method to three dimensions and partial anisotropic cases, and paper [3] extend it to state-based peridynamic. In these cases, the standard Finite Element Method is used.





**Resources**

* Journal Papers:

[1] G. Lubineau, Y. Azdoud, F. Han, C. Rey and A. Askari, A morphing strategy to couple local to non-local continuum mechanics, Journal of the Mechanics and Physics of Solids, Vol 60, 6, 1088-1102, (2012)

[2] Y.Azdoud, F. Han, G. Lubineau, A morphing framework to couple non-local and local anisotropic continua, International Journal of Solids and Structures, Vol 50, 9, 1332-1341, (2013)

[3]F Han, G. Lubineau, Y. Azdoud, A. Askari, A morphing approach to couple state-based peridynamics with classical continuum mechanics, Computer Methods in Applied Mechanics and Engineering, (2016)  


* Book chapters:

[5] Y. Azdoud, F. Han, D. Littlewood, G. Lubineau and P. Seleson, Coupling Local and Nonlocal Models, Chapter 17, Handbook of Peridynamic Modeling, Chapman and Hall/CRC, expected 2016

[6] A. Askari, Y. Azdoud, F. Han, G. Lubineau, S. Silling, Peridynamics for analysis of failure in advanced composite materials, Chapter 19 (12), Numerical Modelling of Failure in Advanced Composite Materials, Woodhead Publishing (2015)

* PhD thesis:

[7] Y.Azdoud, A hybrid local/non-local framework for the simulation of damage and fracture, 2014
Technical Summary of Work:
(Please provide one to two paragraphs describing the work using the technical terminology and explanation of work that an expert would be able to understand and evaluate.)




# IV Microstructural simulation of CNT nanocomposites






In this work, I study a particular problem associated with the prediction of effective properties of Carbon Nanotube (CNT) nanocomposites. Homogenized mechanical properties of CNT nanocomposites are generally difficult to predict because of the complex network of nanotubes, possible clustering, confinement and alteration of the matrix due to the nanotubes high aspect ratio and small size. Indeed, biphasic simulations conducted with straight nanotubes having a random distribution and orientation were unable to predict the experimentally observed moduli at either low or high volume fraction of CNT. In [1] and [2], we propose a new strategy based on the introduction of an interphase, which emulates the effect of the nanotube on the matrix. Indeed, density and crystallinity of the matrix has been demonstrated to be higher closer to the nanotube and present good bonding properties. In [1], we present the geometrical analysis associated with the nanocomposite problem. Parameters related to distribution, orientation and clustering of CNT are introduced, as well as interphase parameters. 
<img src="https://azdoud.github.io/images/nano.png" width="280" style="float:right; margin: 1em 0 4em 2em;"
title="reconstruction of statistically representative CNT nanostructure with interphase"/>
In [2], we develop two models, one based a hybrid local/non-local model, which simply introduces a change in the matrix behavior, as well as a local model which has an equivalent effective stiffness model based on the hybrid. An important result of this study is that the interphase volume fraction is the driving parameter when it comes to analyzing effective moduli, while other parameters such as ‘clusterization’ parameter, CNT volume fraction and interphase thickness are weakly influencing the results. Moreover, the hybrid model gives finer-grain information relative to stress and strain concentration in the model, and will be used for damage and failure simulation.


**Resources**

* Journal Papers:

[1] F. Han, Y. Azdoud, G. Lubineau, Computational modeling of elastic properties of carbon nanotube/polymer composites with interphase regions. Part I: Microstructural characterization and geometric modeling, Computational Materials Science, Vol 81, 641-651, (2014)

[2] F. Han, Y. Azdoud, G. Lubineau, Computational modeling of elastic properties of carbon nanotube/polymer composites with interphase regions. Part II: Mechanical modeling, Computational Materials Science, Vol 81, 652-661, (2014)



