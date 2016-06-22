---
layout: default
title: Research
permalink: /work projects
---


# Coupling method between Local and Non-local Models: The morphing method

In this work, I designed a new type of coupling method between the classic continuum theory and integral non-local models such as peridynamics. The motivation of such method is to reduce computational cost when using peridynamics by restricting the domain of application, and to provide simple boundary conditions. In [1], I developed the morphing method based on an energy density constraint at the local level. A smooth transition between local model and non-local model is achieved by introducing a coupling parameter, alpha(x), in the hybrid constitutive equation. The coupling is achieved in a thick coupling zone, where alpha(x) varies, surrounding the pure non-local patch.
The paper [1] demonstrates the effectiveness of the method for 2D cases, and gives an interpretation to the coupling error in an analytical 1D case. The paper [2] extends the method to three dimensions and partial anisotropic cases, and paper [8] extend it to state-based peridynamic. In these cases, the standard Finite Element Method is used.


<img src="/images/vortex.gif" width="200" style="float:right; margin: 1em 0 4em 2em;"
title="Potential vorticity during the vortex splitting event in December 1984."/>



**Resources**

* Journal Papers:

[1] G. Lubineau, Y. Azdoud, F. Han, C. Rey and A. Askari, A morphing strategy to couple local to non-local continuum mechanics, Journal of the Mechanics and Physics of Solids, Vol 60, 6, 1088-1102, (2012)

[2] Y.Azdoud, F. Han, G. Lubineau, A morphing framework to couple non-local and local anisotropic continua, International Journal of Solids and Structures, Vol 50, 9, 1332-1341, (2013)

[8]F Han, G. Lubineau, Y. Azdoud, A. Askari, A morphing approach to couple state-based peridynamics with classical continuum mechanics, Computer Methods in Applied Mechanics and Engineering, (2016)  


* Book chapters:

[6] Y. Azdoud, F. Han, D. Littlewood, G. Lubineau and P. Seleson, Coupling Local and Nonlocal Models, Chapter 17, Handbook of Peridynamic Modeling, Chapman and Hall/CRC, expected 2016

[9] A. Askari, Y. Azdoud, F. Han, G. Lubineau, S. Silling, Peridynamics for analysis of failure in advanced composite materials, Chapter 19 (12), Numerical Modelling of Failure in Advanced Composite Materials, Woodhead Publishing (2015)

* PhD thesis:
[7] Y.Azdoud, A hybrid local/non-local framework for the simulation of damage and fracture, 2014
Technical Summary of Work:
(Please provide one to two paragraphs describing the work using the technical terminology and explanation of work that an expert would be able to understand and evaluate.)



Work2: Adaptive coupling for fracture and damage.
Date of Project Initiation:
August 2010
Date of Project Completion:
February 2014
Resulting Publication or Report (if applicable, please provide corresponding information):
-Journal Papers:

[5] Y. Azdoud, F. Han, G. Lubineau, The morphing method as a flexible tool for adaptive local/non-local simulation of fracture, Computational mechanics, Vol 54, 711-722, (2014)

-Internal Boeing reports: 1

PhD thesis:
[7] Y.Azdoud, A hybrid local/non-local framework for the simulation of damage and fracture, 2014

Technical Summary of Work:
(Please provide one to two paragraphs describing the work using the technical terminology and explanation of work that an expert would be able to understand and evaluate.)

In this work, I designed a new method for simulating fracture and damage using a hybrid local/non-local model. The morphing method is used to seamlessly link the local and non-local region that are adaptively defined following non-local (in the case of fracture [5]) or local (in the case of damage [7]) evolution criteria. Discontinuous Galerkin Finite Element Method (DGFEM) is used in the non-local region to allow failure induced discontinuities. In [5], a seed region is defined where fracture initiation is likely to occur, and propagation of the region is handled by maintaining a characteristic distance to the crack nucleation area. I demonstrate that the adaptive scheme does not interact with the crack propagation phenomenology by using a 3D CT test. I also demonstrate mesh independence.
In [7], I extend the concept to damage continuum. I couple local damage to non-local fracture in order to handle softening by the non-local model, while initiation and hardening is predicted by the local model. The adaptive local/non-local partition is controlled by a local criterion dependent upon the value of the local damage indicator. In that case, no seed region is required. A simple one variable local damage model with hardening is taken. Demonstration is given using a simple 3D traction test.

Plain Language Summary of Work:
(Please provide one to two paragraphs describing the work in layman’s terms or plain language that an average person would be able to understand and evaluate.)

In this work, I used the morphing coupling method to design a new method. Peridynamics, as presented before, can be used for the simulation of fracture, and my coupling method allows to use it only where necessary. However, this region can be difficult to situate in some structures. To address this, I designed a method that decides where to introduce the peridynamic region. I selected appropriate solving tools to introduce cracks in the otherwise continuous models (using DGFEM) in order to represent fracture. 
I extended the compatibility of my method to solve a canonical problem in damage simulation. Indeed, damage simulations generally fail to be accurate when fracture is imminent and the material is softening, but have good prediction potential when the damage is spread in a structure. For that purpose, I used my hybrid model to replace the damage model by the peridynamic model when it is necessary. This strategy is completely novel and allows addressing the inaccuracy during softening by using the peridynamic theory, which better describes that type of situation.

Summary of the Significance of the Work:
(Please provide a brief summary of the significance of the research to the field, economy, health care system, a particular industry, or the general national interest.)

This work is of significance when using peridynamics as a prediction of failure such as fracture and damage. I defined an adaptive method that selects where the peridynamic region has to be introduced in an automatic manner, and introduced DGFEM to supports fracture. As such, it does not require advanced understanding of failure mechanism and can be readily applied in commercial software for simulation of structures. These technical developments make my method compelling for the rapid and accurate prediction of failure for advanced materials. This lowers the time for such material to be safely used in structures such as aircraft, and reduces the need for costly physical experiments.


Summary of the Implementation/Influence of the Work:
(This section is especially important for contributions that do not have any other objective evidence supporting their influence and/or implementation.  In other words, if there is no citation record affiliated with the contribution, no media coverage surrounding the award, or if there is no other objective evidence readily available, then we need to include similar information in objective reference letters to support the contribution’s influence on the field/industry of endeavor.  Therefore, please provide a brief paragraph or a list of instances where this work has been cited, adopted, implemented, commercialized, patented, or utilized in the field/industry.)

This work has resulted into 1 papers, and is part of my PhD thesis [5, 7]. It has been cited 5 times [5] by independent authors in the scientific community. The method is currently being implemented by the Boeing Company, since it was the funding institution for this work. Another paper is currently in preparation on the subject, focused on damage. This work is recognized as an adaptive way of introducing peridynamics with fracture and damage.


Work3: Microstructural simulation of CNT nanocomposites
Date of Project Initiation:
January 2013
Date of Project Completion:
February 2014
Resulting Publication or Report (if applicable, please provide corresponding information):
-Journal Papers:

[3] F. Han, Y. Azdoud, G. Lubineau, Computational modeling of elastic properties of carbon nanotube/polymer composites with interphase regions. Part I: Microstructural characterization and geometric modeling, Computational Materials Science, Vol 81, 641-651, (2014)

[4] F. Han, Y. Azdoud, G. Lubineau, Computational modeling of elastic properties of carbon nanotube/polymer composites with interphase regions. Part II: Mechanical modeling, Computational Materials Science, Vol 81, 652-661, (2014)

Technical Summary of Work:
(Please provide one to two paragraphs describing the work using the technical terminology and explanation of work that an expert would be able to understand and evaluate.)
In this work, I study a particular problem associated with the prediction of effective properties of Carbon Nanotube (CNT) nanocomposites. Homogenized mechanical properties of CNT nanocomposites are generally difficult to predict because of the complex network of nanotubes, possible clustering, confinement and alteration of the matrix due to the nanotubes high aspect ratio and small size. Indeed, biphasic simulations conducted with straight nanotubes having a random distribution and orientation were unable to predict the experimentally observed moduli at either low or high volume fraction of CNT. In [3] and [4], we propose a new strategy based on the introduction of an interphase, which emulates the effect of the nanotube on the matrix. Indeed, density and crystallinity of the matrix has been demonstrated to be higher closer to the nanotube and present good bonding properties. In [3], we present the geometrical analysis associated with the nanocomposite problem. Parameters related to distribution, orientation and clustering of CNT are introduced, as well as interphase parameters. In [4], we develop two models, one based a hybrid local/non-local model, which simply introduces a change in the matrix behavior, as well as a local model which has an equivalent effective stiffness model based on the hybrid. An important result of this study is that the interphase volume fraction is the driving parameter when it comes to analyzing effective moduli, while other parameters such as ‘clusterization’ parameter, CNT volume fraction and interphase thickness are weakly influencing the results. Moreover, the hybrid model gives finer-grain information relative to stress and strain concentration in the model, and will be used for damage and failure simulation.

Plain Language Summary of Work:
(Please provide one to two paragraphs describing the work in layman’s terms or plain language that an average person would be able to understand and evaluate.)
In this work, we try to predict the mechanical properties of a carbon nanotube nanocomposite. This is a material composed of a plastic (epoxy in our case) bulk in which carbon nanotubes are introduced. Because the nanotube's size is similar to that of the plastic polymer chains that make up the plastic bulk, the interaction between them matters. Our hypothesis is that the plastic changes properties around the nanotube, resulting in the whole material becoming stiffer. This is justified by physical experiments that were not taken into account in previous simulations. We used the hybrid classic continuum/peridynamic model to simulate this change in the plastic and we were able to find prediction that where compatible with the experiment. This work is a direct application of the coupled model that we defined with the morphing method, which demonstrates the versatility of our approach to a material-oriented problem.


Summary of the Significance of the Work:
(Please provide a brief summary of the significance of the research to the field, economy, health care system, a particular industry, or the general national interest.)

This work is of significance when designing and predicting behavior of CNT nanocomposites. Such composites are part of the new generation of functional material and are therefore used in high end application such as aircraft, automotive and satellites. This work introduces a novel way of understanding the effect of CNT on the bulk polymer, and can help tailor new materials. It is then of interest in the manufacture of specialty lightweight structural materials.


Summary of the Implementation/Influence of the Work:
(This section is especially important for contributions that do not have any other objective evidence supporting their influence and/or implementation.  In other words, if there is no citation record affiliated with the contribution, no media coverage surrounding the award, or if there is no other objective evidence readily available, then we need to include similar information in objective reference letters to support the contribution’s influence on the field/industry of endeavor.  Therefore, please provide a brief paragraph or a list of instances where this work has been cited, adopted, implemented, commercialized, patented, or utilized in the field/industry.)

This work has resulted into 2 papers [3, 4]. It has been cited 20 times (12 times for [3] and 8 for [4]) by independent authors in the scientific community. For instance, S. Gong et al considered our clustering approach of nanotube to study the effect of on piezoresistivity; T. Takeda et al reached similar conclusion on interphase importance in the case of fatigue and Z. Yuan and Z. Lu used a similar geometric generation protocol on elastic-plastic polymer composite.

Zeshuai Yuan, Zixing Lu, Numerical analysis of elastic–plastic properties of polymer composite reinforced by wavy and random CNTs, Computational Materials Science, Volume 95, December 2014, Pages 610-619

S. Gong, Z.H. Zhu, S.A. Meguid, Carbon nanotube agglomeration effect on piezoresistivity of polymer nanocomposites, Polymer, Volume 55, Issue 21, 9 October 2014, Pages 5488-5499
Tomo Takeda Yasuhide Shindo Zhijuan Wei Yu Kuronuma Fumio Narita, Fatigue failure and electrical resistance behaviors of carbon nanotube-based polymer composites under uniaxial tension–tension loading in a cryogenic environment, Journal of Composite Materials February 2015 vol. 49 no. 4 457-463
Work4: Adaptive Wavelet Enhancement method
Date of Project Initiation:
February 2014
Date of Project Completion:
Current
Resulting Publication or Report (if applicable, please provide corresponding information):
-2014 AFOSR annual report
-Conference and report meetings:
[10] Y.Azdoud, J.Cheng, S. Ghosh, The Adaptive Wavelet Enhancement for Crystal Plastic Finite Element Method, 13th US National Congress on Computational Mechanics, San Diego, CA (2015)

[11] S.Ghosh, Y. Azdoud, Advancing Computational Methods for Image-based Modeling of Polycrystalline Metallic Material, AFOSR 2015 Multiscale Structural Mechanics Annual Grantees Meeting, Fort Walton, FL (2015)

[12] S.Ghosh, Y. Azdoud, Advancing Computational Methods for Image-based Modeling of Polycrystalline Metallic Material, AFOSR 2014 Multiscale Structural Mechanics Annual Grantees Meeting, Albuquerque, NM (2014)

Technical Summary of Work:
(Please provide one to two paragraphs describing the work using the technical terminology and explanation of work that an expert would be able to understand and evaluate.)
In this work, I develop an innovative optimization method to adaptively enrich the accuracy of crystal plasticity simulation while limiting the computational cost. Modeling complex polycrystalline microstructure requires a fine discretization to ensure satisfactory accuracy, which ultimately impacts the computational cost. This is especially critical for problems introducing phenomenology with localization, such as shear banding, twinning or fracture. I develop a new method based on second generation wavelets to enrich finite element simulations. In this new method, a wavelet decomposition scheme is used to analyze error indicators in order to provide a basis of enrichment functions. The wavelet family is chosen such that the enriching function constitutes a hierarchical finite element basis. These functions are introduced adaptively in the FEM scheme to locally enrich the solution. The particularity of this method is that the adaptive scheme is consistent with the error analysis.

Plain Language Summary of Work:
(Please provide one to two paragraphs describing the work in layman’s terms or plain language that an average person would be able to understand and evaluate.)

Crystal plasticity is the study of the behavior of metals at the scale of few microns. At this scale, metals are composed of aggregates of small metallic crystals, called grains. Under stress, defects on these grains move and coalesce which leads to permanent deformation. The crystal plasticity theory aim at predicting these deformations, which are paramount to predict failure of metallic objects under complex loading; for example, parts in plane engine. The crystal plasticity theory is simulated on computers using the crystal plasticity finite element method. One important feature of the deformations at the scale of the grains in the metals is that they are very sensitive to local arrangement of the grains. It is then important, when doing a computer simulation to account in details of the exact arrangement of the grain. This generally calls for a very small resolution, hence a long computation time. In order to speed up the computation, only important features should be finely resolved, while the rest of the domain should have a lower resolution. To explain this principle, imagine the picture of an object on a black background. If you reduce the resolution (the number of pixel) on the black background, this will not affect your understanding of the picture, since the object is correctly resolved. This is actually what compressed format of images like JPEG do to compress an image. In order to do so, JPEG images are compressing with a mathematical tool called wavelets. Wavelets can be seen as a set of filter functions that identify where sharp feature are, and at which scale, which tell you where to keep high resolution. In my work, I adapted the concept of wavelets to crystal plasticity. I use a wavelet method to analyses my grain structure during the simulation and put the right amount of computational resource where needed. Since this is done in real time, the resolution actually evolve when the crystal structure deforms, always keeping important features “visible”. My method significantly reduces the computation time, which in turn reduces the cost of simulating complex structure, helping making better predictions.

Summary of the Significance of the Work:
(Please provide a brief summary of the significance of the research to the field, economy, health care system, a particular industry, or the general national interest.)
This work is of significance when designing and predicting behavior of metals under high stress, or during formation. Most studied alloy are specialty alloys used for plane engines, tank armors and other structures exposed to extreme conditions. This work introduces a novel way of quickly computing simulations involving crystal plasticity, greatly reducing time and cost of predicting behavior. This in turn allows for fast development in state of the art industries.
Summary of the Implementation/Influence of the Work:
(This section is especially important for contributions that do not have any other objective evidence supporting their influence and/or implementation.  In other words, if there is no citation record affiliated with the contribution, no media coverage surrounding the award, or if there is no other objective evidence readily available, then we need to include similar information in objective reference letters to support the contribution’s influence on the field/industry of endeavor.  Therefore, please provide a brief paragraph or a list of instances where this work has been cited, adopted, implemented, commercialized, patented, or utilized in the field/industry.)

This is currently a work in progress but it has been favorably received in the community through conference [10] and reports [11, 12]. I am currently preparing 2 publications on this subject that are expected for submission in 2016.


