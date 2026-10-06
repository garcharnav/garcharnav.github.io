---
layout: page
title: Engineering Projects
location: head
published: true
---
Selected design and computational modeling projects from my undergraduate studies and co-op terms at the University of Waterloo. My current research is described on the [Research](/research/) page.

### Heat transfer fin solver (MATLAB, finite differences)

I developed a numerical solver to predict the temperature field and heat transfer within a fin array. To do so, I discretized the governing differential equation using the finite difference method (FDM) and used boundary conditions to form a sparse matrix of the fin geometry. I implemented the solver in MATLAB and varied the mesh size to assess grid independence.

<img src="https://raw.githubusercontent.com/garcharnav/garcharnav.github.io/master/images/fin.png" alt="MATLAB Fin Model">


### Combustor inlet optimization (ANSYS CFX)

To study the optimal gas inlet angle for a combustor, I developed a CFD model of a non-reacting combustor with ANSYS CFX. The model determined that a 20° clockwise angle yielded optimal mixing. Simulations were also completed with two turbulence CFD models to elucidate their effects on the results.

<img src="https://raw.githubusercontent.com/garcharnav/garcharnav.github.io/master/images/combustor.PNG" alt="ANSYS Combustor Model">

### Ultrasonic transducer mount (Hatch co-op)

During a co-op at Hatch, I designed a transducer mounting system to improve ultrasonic data collection on blast furnaces, featuring: 
* Two silicone diaphragms that allowed two sensors (one signal emitting, one receiving) to conform to the shape of a curved wall.
* An aluminum sheet metal frame and a 304 stainless steel cage for corrosion resistance and strength.

:-------------------------:|:-------------------------:
<img src="https://raw.githubusercontent.com/garcharnav/garcharnav.github.io/master/images/sensor.png" width="99%"> | <img src="https://raw.githubusercontent.com/garcharnav/garcharnav.github.io/master/images/sensor1.png" width="99%">

### Blood shearing assay drive (undergraduate research)

For the Materials in Biological Systems Lab at the University of Waterloo, I designed a gear train mechanism for a blood shearing assay. The objective of this design was to increase experimental output of a 24 well plate. This design used:
* 6 brushed DC gearmotors coupled to 6 separate gear trains.
* 3D printed mounting box that houses the gear trains and rests above a 24 well plate.

:-------------------------:|:-------------------------:
<img src="https://raw.githubusercontent.com/garcharnav/garcharnav.github.io/master/images/gear.png" width="99%"> | <img src="https://raw.githubusercontent.com/garcharnav/garcharnav.github.io/master/images/gear2.png" width="99%">

### Low-speed drive (Waterloop design team)

On the Waterloop design team, I collaborated on the design of a low speed drive. The goal was to develop a fail safe linear motion machine that provides initial acceleration to team’s vehicle. I worked on design ideation, refinement and CAD. The system featured:
* Coaxial electric drive motor with cast urethane wheel tread.
* Pneumatic cylinder and boomerang linkage to provide contact force between the wheel and track.
* Sheet metal mounts to connect the low speed drive to the vehicle’s space frame.

:-------------------------:|:-------------------------:
<img src="https://raw.githubusercontent.com/garcharnav/garcharnav.github.io/master/images/lsd.png" width="99%">  |  <img src="https://raw.githubusercontent.com/garcharnav/garcharnav.github.io/master/images/lsd1.png" width="99%">
