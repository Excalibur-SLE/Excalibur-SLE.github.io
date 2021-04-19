---
layout: default
---

## Workshop on "Inverse Problems and Optimisation" 6-7 May 2021

Inverse problems are concerned with the recovery of the parameters of a
forward model given observations of data that it describes. Such
problems arise in almost all fields of science when details of a
postulated model, such as maps of physical properties and/or their
classification into identifiable objects, have to be determined from a
set of observed data.The inverse problem topic is highly
cross-disciplinary, both within mathematics, encompassing aspects of
pure, applied and statistics, and across subjects, including physical
sciences, engineering and biology to name only a few. Inverse problems
increasingly consider mappings between solutions and data1in high
numbers of dimensions (e.g. three in space plus time plus
wavelength). Direct representations easily exceed existing
computational and memory resources, and necessitate appropriate design
of data structures and algorithms. In parallel, machine learning
methods designed for "big data" problems are proving useful in
developing data reduction approaches and representation of appropriate
priors. Some of the topics of this planned workshop includescheduling
and optimising parallelism for multiple forward solves as part of a
nonlinear inverse problem on exascale architectures; the combination
of inference-based machine learning techniques and classical model
based inverse problems at scale, and their often differing hardware
requirements (e.g. GPU vs CPU); using exascale computing to include
uncertainty in the formulation of inverse problems.

### Programme 

#### Thursday 6 May

13:00 Introduction  
13:05 James Nagy (Emory University) - TBA  
13:55 Bill Lionheart (University of Manchester) - TBA  
14:45 **Break**  
15:15 Chris Budd (University of Bath) - TBA  
16:05 George Biros (U. T. Austin) - TBA  
17:00 **Open Discussion**  

#### Friday 7 May

13:00 Laurent Demanet (MIT) - TBA  
13:50 Vladimir Druskin (Worcester Polytechnic Institute) - *Data-Driven Reduced Order Models, Ladder Networks, and Inverse Scattering*  
14:40 **Break**  
15:10 Jiri Jaros (Brno University) / Felix Lucka (CWI) - TBA  
16:00 Oscar Bruno (Caltech) - *Fast spectral integral solvers for general electromagnetic structures*  
17:00 **Virtual drinks and discussions**  


### Registration

The workshop will take place on Zoom: please [register](https://www.eventbrite.co.uk/e/excalibur-workshop-on-inverse-problems-and-optimisation-tickets-149191430585) to take part.

### Abstracts

#### Oscar Bruno - Data-Driven Reduced Order Models, Ladder Networks, and Inverse Imaging

We present fast spectral electromagnetic solvers that address some of the main difficulties associated with the simulation of realistic engineering electromagnetic problems in the frequency- and time-domain. Based on the use of Green functions and fast high-order methods for evaluation of integral operators, these algorithms can solve, with high-order accuracy, problems of electromagnetic propagation and scattering for large and complex three-dimensional structures and devices -- including e.g. silicon devices, structured lenses, and metamaterials. In particular, we will consider the important but challenging problem of inverse design and optimization of optical and photonic devices of large electrical sizes. A variety of applications will be presented demonstrating the significant design capabilities inherent in the new methods, as well as the improvements these algorithms can provide, over other approaches, in generality, accuracy, and speed. Time permitting, a novel class of accelerated Green function methods will be mentioned.

#### Vladimir Druskin - Data-Driven Reduced Order Models, Ladder Networks, and Inverse Scattering

We discuss a novel unified framework for imaging with active electromagnetic and acoustic arrays in complex environments over a broad range of regimes ranging from lossless wave propagation to diffusion-dominated regime. Many conventional approaches to imaging based on linearizations fail in the presence of strong non-linear effects such as multiple scattering, high contrasts, losses, dispersion, etc. Even if applied iteratively in optimization framework, they may lack robustness and converge slowly due to a highly non-convex data misfit.

One of classical tasks of the network synthesis is to construct ROMs realized via ladder networks matching rational approximations of a targeted filter transfer function. The inverse scattering can be also viewed in the network synthesis framework. The proposed framework is based on data-driven reduced order models (ROMs) and it avoids the issues faced by the conventional techniques. A ROM of the underlying partial differential equation (PDE) is constructed from the measured data, hence the designation “data-driven”. The key is continuum interpretation of the equivalent network in terms of the underlying medium properties, aka embedding.  It encodes the PDE coefficients which carry information about the target. Construction of the ROM is a highly non-linear process that “absorbs” much of the nonlinearity of the problem, thus making the subsequent imaging a lot more straightforward.  For example, it allows us to avoid local minima in optimization frameworks and for some problems even to develop direct nonlinear imaging algorithms. 

We will show a number  of 2D numerical experiments ranging from seismic full wave inversion   to radar imaging.   This is joint work with Liliana Borcea, Alex Mamonov, Shari Moskow, Mikhail Zaslavsky and Jorn Zimmerling.
