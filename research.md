---
layout: page
title: Research
description: Research projects of Arnav Garcha on computational modeling of arterial thrombosis and coronary hemodynamics.
---

My research combines computational fluid dynamics, discrete particle methods, and high-performance computing to study how blood flow governs platelet transport and thrombosis in arteries, and how vascular anatomy shapes the hemodynamic metrics used in clinical assessment of coronary artery disease. This work is carried out in the [BioSiMM Lab](https://meche.engineering.cmu.edu/faculty/gutierrez-biosimm-lab.html) at Carnegie Mellon University.

## Particle-level modeling of arterial thrombosis

Arterial thrombosis begins with the transport of platelets to the vessel wall, followed by their adhesion, activation, and aggregation. These events occur at the scale of individual platelets, whereas the flows that govern them are set by the geometry of the artery, several orders of magnitude larger. Cell-resolved methods capture platelet behavior in detail but become computationally prohibitive at arterial length scales.

My dissertation develops a hybrid continuum–discrete framework to bridge these scales. The arterial flow is resolved as a continuum, and platelets are tracked as discrete particles with models for wall adhesion, activation state, and post-activation aggregation. The framework is parallelized with MPI for high-performance computing systems.

<p class="related-outputs"><strong>Related:</strong> manuscript in preparation; oral presentations at WCCM 2026, CMBE 2026, and CMBBE 2025; 1st place poster, Engineering in Cardiovascular Medicine Workshop, University of Michigan, 2026.</p>

## Near-wall platelet enrichment in arterial flows

Platelets accumulate near vessel walls in flowing blood, a phenomenon known as margination that has been characterized mainly in small vessels. This project examines the mechanisms that govern near-wall platelet enrichment as vessel scale increases to that of arteries, including the influence of secondary flows. The results inform how platelets are initialized in arterial-scale thrombosis simulations.

<p class="related-outputs"><strong>Related:</strong> Garcha &amp; Grande Gutiérrez, <a href="https://doi.org/10.1063/5.0324694"><em>Physics of Fluids</em> (2026)</a>, Editor's Pick; APS Division of Fluid Dynamics 2024.</p>

## Vascular structure and coronary hemodynamics

Coronary artery anatomy varies between individuals in branching angles, branch positions, and vessel diameter ratios. Using computational fluid dynamics, this work quantifies how such variations, in healthy and diseased arteries, affect local hemodynamic quantities such as wall shear stress and global indices used in clinical assessment, such as the instantaneous wave-free ratio.

<p class="related-outputs"><strong>Related:</strong> Garcha &amp; Grande Gutiérrez, <a href="https://doi.org/10.1038/s41598-025-85781-x"><em>Scientific Reports</em> (2025)</a>; BMES 2023; APS Division of Fluid Dynamics 2023; ASME Summer Bioengineering Conference 2024.</p>

## Microvascular resistance and coronary diagnostic indices

Coronary diagnostic indices are measured in the epicardial arteries but also depend on the resistance of the downstream microvasculature. This project, led by Tej Jolly during his master's research under my mentorship, used multiscale simulations to quantify the influence of microvascular resistance on these indices.

<p class="related-outputs"><strong>Related:</strong> Jolly, Garcha &amp; Grande Gutiérrez, <a href="https://doi.org/10.1007/s10439-026-04378-1"><em>Annals of Biomedical Engineering</em> (2026)</a>; 1st place, Master's Student Competition, ASME Summer Bioengineering Conference 2025.</p>

## Collaborative projects

- Best practices for selecting physiological, patient-specific boundary conditions in vascular CFD simulations (manuscript in preparation).
- Transport patterns for nutrient delivery in a multiscale computational model of the placentone (manuscript in preparation).
- Graph neural network super-resolution to accelerate cardiovascular CFD simulations (manuscript in preparation).

## Earlier work

Before graduate school, I worked on mechanical design and computational modeling projects during my undergraduate studies and co-op terms. Selected examples are on the [Engineering Projects]({{ '/Portfolio/' | relative_url }}) page.
