---
layout: default
---

## Workshop on "Towards Exascale Simulation of integrated engineering systems at extreme scale"

The imminent deployment of exascale computing will usher in a new era
of engineering system prediction, design and optimisation. It would
enable a whole-system approach in a seamless fashion that
significantly cuts the development cycle and cost. Before such a full
potential can be realised, a fundamental rethink is needed about
how we construct physical models and application software codes for
the new computer architectures and software libraries. Sophisticated
engineering systems typically involve multi-physical processes, such
as flow, heat transfer, chemical reactions, electromagnetics,
acoustics, and fluid-structure interaction, often in complex
geometries. Spatial scales can span 9-12 orders of magnitude and the
range of temporal scales can be even wider. In most cases, computer
codes have been developed and optimised for specific applications with
a limited range of time and length scales. The corresponding models
and numerical methods pose different challenges on exascale
computers. How to integrate existing methods and/or develop completely
new methods to make full use of exascale computing is a grand
challenge for mathematicians, physicists, computer scientist as well
as engineers. In this workshop, leading experts in the field will
showcase recent efforts in the development of modelling methodologies,
computer algorithms, software interfaces, and software/hardware
co-design in preparation for the arrival of exascale
computing. Cutting-edge simulations of engineering systems at extreme
time and length scales will be demonstrated. Finally, existing gaps
and remaining issues will be identified to stimulate further
discussions and actions in the field.

### 21 January 2021

- 12:55-13:00 Garth Wells (Cambridge University, UK): Welcome and Introduction

#### Session 1: Chair – David Emerson (DL, UK)

- 13:00-13:30 <a href="https://youtu.be/rNzu7JzbE08">![video](/assets/images/yt_icon_rgb.png)</a> Prof Haohuan Fu (Tsinghua University & National Supercomputing Center in Wuxi, China): Optimizing CESM-HR on Sunway TaihuLight and An Unprecedented Set of Multi-Century Simulation

- 13:30-14:00 <a href="https://youtu.be/59Xn-rrpY0Q">![video](/assets/images/yt_icon_rgb.png)</a> Dr Christopher Maynard (University of Reading and Met Office, UK): Realising Richardson’s Dream: Developing Modelling Capability at Exascale for the Met Office

- 14:00-14:30 <a href="https://youtu.be/4MfeY0Dwd2Y">![video](/assets/images/yt_icon_rgb.png)</a> Stephen Longshaw (STFC/DL/SC, UK): General High-Performance Code Coupling

- 14:30–15:00 <a href="https://youtu.be/9zZxCO3oI0g">![video](/assets/images/yt_icon_rgb.png)</a> Pierre Sagaut (Aix-Marseille Université): Unsteady simulations of complex turbulent flows using Lattice-Boltzmann Methods

- 15:00–15:15 Coffee Break

#### Session 2: Chair – Peter Coveney

- 15:15–15:45  <a href="https://youtu.be/BBg3qC78QmY">![video](/assets/images/yt_icon_rgb.png)</a> Ernesto Monaco (ESS Engineering Software, Austria): Numerical simulation of industrial relevant applications by the ALSIM™ Platform

- 15:45–16:15  Dr Daniel Lycett-Brown (Dassault Systèmes, Spain): Multiscale simulation of multiphase fluid dynamics for engineering applications

- 16:15–16:45  <a href="https://youtu.be/eF64UG4BNQo">![video](/assets/images/yt_icon_rgb.png)</a> Prof Shantenu Jha (Rutgers University, USA): ZettaScale Computing on Exascale Platforms

- 16:45–17:30 Discussions (Chair: Garth Wells, University of Cambridge)

### 22 January 2021

- 12:55–13:00 Kai Luo (UCL, UK): Welcome and Introduction

#### Session 3: Chair – Timo Betcke

- 13:00–13:30  <a href="https://youtu.be/XlqyYkcdAN8">![video](/assets/images/yt_icon_rgb.png)</a> Prof Peter Coveney (UCL, UK): Applications and Challenges for Systems Engineering on the Road to the Exascale

- 13:30–14:00  <a href="https://youtu.be/G4wcRntgF4s">![video](/assets/images/yt_icon_rgb.png)</a> Benjamin Dudson (University of York, UK): Coupling codes at Exascale for the ExCALIBUR UKAEA NEPTUNE Nuclear Fusion Project

- 14:00–14:30  <a href="https://youtu.be/nyL3eocm7Jg">![video](/assets/images/yt_icon_rgb.png)</a> Andrew Davis (UKAEA): Multiphysics in support of Fusion Component Design

- 14:30–15:00  <a href="https://youtu.be/EA_GVrFp0Rw">![video](/assets/images/yt_icon_rgb.png)</a> Yvan Fournier (EDF, France): Continuous evolution of an industrial CFD code for future environments

- 15:00–15:15 Coffee Break

#### Session 4: Chair – Jianping Meng

- 15:15–15:45  <a href="https://youtu.be/E_88IKy9Kh4">![video](/assets/images/yt_icon_rgb.png)</a> Prof Serge Guillas (UCL, UK): Reduced Order Modelling

- 15:45–16:15  <a href="https://youtu.be/8gaxwrBiyjA">![video](/assets/images/yt_icon_rgb.png)</a> Sauro Succi (Istituto Italiano di Tecnologia & CNR & University of Rome, Italy: Harvard University, USA): Simulating Dropland: Computational Design of Exotic Soft Materials with an Eye to Exascale Computing

- 16:15–16:45  <a href="https://youtu.be/lsBSctsSMFY">![video](/assets/images/yt_icon_rgb.png)</a> Tzanio Kolev (Lawrence Livermore National Laboratory, USA): Efficient Finite Element Discretizations for Exascale Applications

- 16:45–17:30 Discussions (Chair: Kai Luo)


## Invited Talks: Abstracts and Speaker Bios:

### Peter Coveney (UCL, UK): Applications and challenges for systems engineering on the road to the exascale

#### Abstract

In this talk I will highlight some of the work that we are doing within the Centre for Computational Science at UCL that is enabling practical evaluation of several of the current globally leading multi-petascale HPC facilities in preparation for the advent of exascale machines. This work includes simulations at the bleeding edge for applications in cardiovascular blood flow, materials design and drug discovery.
Uncertainty quantification is an essential element in the development of actionable engineering solutions using computers. I will illustrate this by discussing an application of the software tools we have developed to assess the uncertainty in an epidemiological model of the COVID-19 pandemic used to advise UK government ahead of the March 2020 lockdown.

#### Bio

Peter Coveney holds a Chair in Physical Chemistry and is Director of the Centre for Computational Science. He has been at the forefront of HPC-based scientific research for the past twenty years and has led the development of several codes, including the HemeLB and LB3D lattice-Boltzmann packages, which scale to hundreds of thousands of cores on several of the largest supercomputers available. He leads many large projects (MAPPER, ComPat, VECMA FETHPC and CompBioMed1 and 2 phases of the CoE) in which HPC is a central component, including the EPSRC RealityGrid project and subsequent Platform Grant, and the EU HPC Centre of Excellence in Computational Biomedicine.

### Yvan Fournier (EDF): Continuous evolution of an industrial CFD code for future environments

#### Abstract
As one of the largest electricity production utilities, EDF has made
heavy use computational fluid dynamics (CFD) simulations for many
years, both to study improvements to various production means (from
nuclear to wind), and as a part of safety studies around pressurized
water reactors. For most of these applications, EDF has been
continuously developed and maintained the code_saturne CFD solver
since 1997, consolidating experience with older codes. To encourage
and facilitate collaboration, it has been released under a free
software license since 2007.

As with most industrial codes of this type, design must balance ease
of use, robustness, performance, an a wide application and validity
domain, where a tool's life cycle is often longer than thar of many
underlying computing technologies it can use.

Over the years, this has been handled by many incremental code base
evolutions, maintaining features and compatibiliy across several
versions, while rewriting and improving various sub-systems, in a
progressive upgrade cycle.

To keep the user workflow simple and strive for maximum portability
and perfoemance, we have striven over time to ensure as many pre and
post-processing operations as possible are integrated as steps in the
main distributed parallel run, including several in-situ
post-processing options, and parallel coupling features. This has been
done using a combination of internal library functions based on the
code’s main data structures, and optionally leveraging external
libraries, especially for mesh partitioning and in-situ
post-processing.

We will present several of the latest evolutions related to high
performance computing aspects of code_saturne, both related to in-situ
pre and post-processing, and to the computational models and kernels
that have allowed us to adapt for current compute architectures and
prepare for the future, while keeping a consistent long-term
approach.

#### Bio

Yvan Fournier obtained a "diplôme d’ingénieur" (equivalent to a
Master) in aeronautics in 1994 from École Centrale Paris. He has
worked as a researcher at EDF R&D since 1998, and is currently a
principal research engineer, working on various HPC, pre and
post-processing, and software engineering aspects of EDF’s CFD
in-house codes, mainly code_saturne (code-saturne.org). His current
interests include in-situ mesh improvement and post-processing,
distributed algorithms, software engineering, and high performance
computing. Past interests also include CFD modeling of cooling towers
and PWR fuel assemblies.

### Prof Haohuan Fu (Tsinghua University & National Supercomputing Center in Wuxi): Optimizing CESM-HR on Sunway TaihuLight and An Unprecedented Set of Multi-Century Simulation

#### Abstract

CESM is one of the very first and most complex scientific codes that
gets migrated onto Sunway TaihuLight. Being a community code involving
hundreds of different dynamic, physics, and chemistry processes, CESM
brings severe challenges for the many-core architecture and the
parrallel scale of Sunway TaihuLight. This talk summarizes our
continuous effort on enabling efficient run of CESM on Sunway,
starting from refactoring of CAM in 2015, redesigning of CAM in 2016
and 2017, and a collaborative effort starting in 2018 to enable highly
efficient simulations of the high-resolution (25 km atmosphere and 10
km ocean) Community Earth System Model (CESM-HR) on Sunway
Taihu-Light. The refactoring and optimizing efforts have improved the
simulation speed of CESM-HR from 1 SYPD (simulation years per day) to
5 SYPD (with output disabled). Using CESM-HR, We manage to provide an
unprecedented set of high-resolution climate simulations, consisting
of a 500-year pre-industrial control simulation and a 250-year
historical and future climate simulation from 1850 to 2100. Overall,
high-resolution simulations show significant improvements in
representing global mean temperature changes, seasonal cycle of
sea-surface temperature and mixed layer depth, extreme events and in
relationships between extreme events and climate modes.

#### Bio

Haohuan Fu is a professor in the Ministry of Education Key Laboratory
for Earth System Modeling, and Department of Earth System Science in
Tsinghua University, where he leads the research group of High
Performance Geo-Computing (HPGC). He is also the deputy director of
the National Supercomputing Center in Wuxi, leading the research and
development division. Fu has a PhD in computing from Imperial College
London. His research work focuses on providing both the most efficient
simulation platforms and the most intelligent data management and
analysis platforms for geoscience applications, leading to two
consecutive winning of the ACM Gordon Bell Prizes (nonhydrostatic
atmospheric dynamic solver in 2016, and nonlinear earthquake
simulation in 2017).

### Serge Guillas (UCL, UK): Reduced Order Modelling

#### Abstract

Uncertainty quantification of complex coupled models is done
via building surrogates (known as statistical emulators) that mimic
the input-output relationship, in order to alleviate the computational
burden of running ensembles. However, the complexities of models are
often large so building emulators can be challenging. In this talk, we
discuss strategies to reduce input and output dimensions with little
loss in information, exploiting input sensitivities and output
variability over time or space. We also propose a bespoke
approach for systems of sub-models where emulators can be linked to
achieve large gains in computational efficiency and approximation
accuracy.

#### Bio

S. Guillas is Professor of Statistics at UCL and the Met Office Joint Chair in Data Sciences for Weather and Climate. He obtained his PhD (Paris 6 Pierre-et-Marie-Curie, France) in 2001. He was postdoc at the University of Chicago, USA over 2002-2004, Assistant Professor (Georgia Institute of Technology, USA) over 2004-2007, and joined UCL in 2007. He was vice-Chair of the SIAM activity group on Uncertainty Quantification (UQ) over 2015-2016. He is currently Chair of the Working group on Uncertainties in the COST action "Accelerating Global science In Tsunami HAzard and Risk analysis" (AGITHAR, 25 countries). He leads several projects on UQ, mostly for multi-scale and multi-physics simulations on HPC. He founded in 2019 the UQ interest group at the Alan Turing Institute.

### Prof Shantenu Jha (Rutgers University, USA): ZettaScale Computing on Exascale Platforms

#### Abstract

We outline the vision of  “Learning Everywhere,” which captures the
impact of learning methods coupled to traditional HPC methods. We
present several examples of "effective performance" improvements for
traditional HPC simulations that learning (MLforHPC) provides. We
discuss how we are applying the "Learning Everywhere” paradigm to
advance therapeutics for COVID19. We will showcase the challenges and
performance of scalable integrated HPC & AI software infrastructure
developed to support long-running computational campaigns as part of
the DOE’s Medical Therapeutics project under the umbrella of the
National Virtual Biotechnology Laboratory.

#### Bio
 Shantenu Jha is the Chair of Computation & Data Driven Discovery
 Department at Brookhaven National Laboratory, and Professor of
Computer Engineering at Rutgers University. His research interests are
 at the intersection of high-performance distributed computing and
 computational & data science. Shantenu leads the the
 RADICAL-Cybertools project which are a suite of middleware building
 blocks used to support large-scale science and
 engineeringapplications.  He was appointed a Rutgers Chancellor's
 Scholar (2015) and was the recipient of the inaugural Chancellor's
 Excellence in Research (2016) for his cyberinfrastructure
 contributions to computational science. He is a recipient of the NSF
 CAREER Award (2013), the Gordon Bell Award (2020)
and several other prizes at SC'xy and ISC’xy,well as the winner of
 IEEE SCALE 2018.  More details can be found at:
 http://radical.rutgers.edu/shantenu

### Tzanio Kolev (Lawrence Livermore National Laboratory): Efficient Finite Element Discretizations for Exascale Applications

#### Abstract

Exascale architectures require rethinking of the numerical algorithms
used in many large-scale applications. These architectures favor
algorithms that expose fine-grain parallelism and maximize the ratio
of floating point operations to energy intensive data movement. One
of the few viable approaches to achieve high efficiency in the area
of PDE discretizations on unstructured grids is to use
matrix-free/partially-assembled high-order finite element methods to
increase the accuracy and/or lower the computational time due to
reduced data motion.

In this talk we report on recent work in the Center for Efficient
Exascale Discretizations (CEED) [1], a co-design center in the US
Exascale Computing Project that is focused on the development of
next-generation discretization software and algorithms to enable a
wide range of finite element applications to run efficiently on future
hardware. CEED is a research partnership involving 30+ computational
scientists from two US national labs and five universities, including
members of the Nek5000, MFEM [2], MAGMA, OCCA and PETSc projects.

Topics of discussion will include recent progress in CEED packages and
applications, new miniapps, benchmarks and libraries developed in the
project, efficient GPU algorithms, and our efforts in unstructured
adaptive mesh refinement, matrix-free linear solvers and high-order
data analysis and visualization.

[1] Center for Efficient Exascale Discretizations, https://ceed.exascaleproject.org

[2] MFEM finite element library, https://mfem.org

#### Bio

Tzanio Kolev is a computational mathematician at the Center for
Applied Scientific Computing in Lawrence Livermore National Laboratory
(LLNL), where he works on finite element discretizations and solvers
for problems in compressible shock hydrodynamics, multi-material
arbitrary Lagrangian Eulerian methods, radiation hydrodynamics, and
computational electromagnetics. Tzanio is the director of the Center
for Efficient Exascale Discretizations (CEED) in US Exascale Computing
Project and leads the high-order finite element discretization
research and development efforts in the MFEM and BLAST projects at
LLNL. Tzanio's research interests include the development and analysis
of advanced finite element discretization methods, massively parallel
preconditioners, discretization-enhanced algebraic multigrid
algorithms, and the design and implementation of large-scale
scientific software.

### Stephen Longshaw (STFC, DL, SC; UK): General High-Performance Code Coupling

#### Abstract

 In this talk I will describe the open-source Multiscale Universal
 Interface (MUI) code coupling library. A joint development between
 UKRI STFC, Lawrence-Berkeley National Laboratory, IBM Research UK and
 Brown University, MUI is a C++ header-only library that provides a
 simple point-based data transfer paradigm, alongside an extensible
 collection of spatial and temporal sampling algorithms. It is
 designed entirely around the MPI MPMD (Multiple Program Multiple
 Data) concept and offers great potential for use in an HPC
 environment. As example I will also discuss a recent effort using MUI
 to couple a Molecular Dynamics and Direct Simulation Monte Carlo
 solver to enable solution of microscopic problems involving gas and
 large simulation domain sizes.

#### Bio

 Stephen is a Principal Computational Scientist in the Computational
 Engineering Group based at UKRI STFC’s Daresbury Laboratory. He is a
 computer scientist that specialises in computational modelling
 (especially computational fluid dynamics (CFD) using particle methods
 such as smoothed particle hydrodynamics) and scientific code coupling
 for both multi-scale and multi-physics problems. He also has a keen
 interest in understanding and utilising novel and emerging computing
 hardware and HPC and, in particular, how these two interests combine
 to form the new exascale landscape.

### Dr Daniel Lycett-Brown (Dassault Systèmes): Multiscale simulation of multiphase fluid dynamics for engineering applications

#### Abstract

 The computational simulation of fluid dynamics is required across a
 wide range of engineering applications. Here we focus on multiphase
 fluid dynamics using the lattice Boltzmann method, with applications
 ranging from the micron scale (porous media, ink-jet printing,
 lab-on-a-chip etc.) to the meters scale (car wading, offshore wind
 turbines, ship dynamics etc.). Different physics dominates at
 different scales which has led to the development of different
 modelling approaches for different applications. However many
 practical applications bridge a wide range of scales and this
 modelling approach breaks down. We propose solutions to this problem,
 for which exascale computing plays a significant role. Highly
 efficient and scalable codes that can take full advantage of modern
 CPU supercomputers and GPU clusters are allowing simulations with
 higher resolutions than previously possible. Combined with
 technologies for adaptive mesh refinement and effective load
 balancing across MPI processes this will allow a larger range of
 scales to be simulated with acceptable turnaround times. However in
 some circumstances subgrid scale phenomena will still require
 modelling.  Development of models for these subgrid phenomena and
 coupling between models at different scales is required. Exascale
 computing can again play a role; large numbers of high-resolution
 simulations at the microscale can be used to inform these subgrid
 models (for example droplet collision maps can be built up to inform
 spray dynamic models). The combination of new models, coupled across
 time and length scales, and the power of exascale computing will be
 revolutionary in the simulation tools needed to design the
 engineering applications of tomorrow.

### Dr Christopher Maynard (University of Reading and Met Office, UK): Realising Richardson’s dream: Developing modelling capability at Exascale for the Met Office

#### Abstract

The Met Office is developing a new weather and climate
modelling system to exploit Exoscale computing. The atmospheric model
is named LFRic after Lewis Fry Richardson, who first attempted
numerical weather prediction a century ago. The LFRic model is being
co-designed with a Domain Specific Language (DSL) and new scientific
methods, such as communication avoiding algorithms. The DSL allows for
single source science code with parallel code for different
programming models. Some Initial performance results are shown.

#### Bio

Chris Maynard has been an Associate Professor of Computer Science
at the University of Reading since January 2018 and he retains his
position as an Expert Scientific Software Engineer at the Met Office
which he has held since 2012. Prior to joining the Met Office he
worked at the Edinburgh Parallel Computing Centre (EPCC) where he
developed and optimised scientific software for supercomputers in
diverse fields such as Particle Physics, Computational Fluid Dynamics
(CFD), Magnetic materials, acoustic properties of materials, Group
Theory, Numerical Analysis and Quantum Computing. He obtained his PhD
in 1998 from the University of Edinburgh in theoretical particle
physics. Since joining the Met Office he has optimised the solver for
the UM dynamical core called ENDGame. He is leading the development of
a domain specific language for the new Met Office Model, Gung Ho/LFRic
to enable performance on diverse exascale computing architectures. His
research interests include methods for High Performance Computing,
parallel programming models, languages and algorithms and domain
specific languages.


### Dr Ernesto Monaco (ESS Engineering Software, Austria): Numerical simulation of industrial relevant applications by the ALSIM™ Platform

#### Abstract

The talk will give an overview about the most recent developments of
the ALSIM™ platform, which represents the unique ESS solution to
tackle several relevant industrial applications, with special emphasis
on topics related to car manufacturing: examples will include
Paint-shop (E-Coating, Oven), as well as washing, pre-treatment and
deformation of metal sheets. ALSIM employs a portfolio of several
solvers (LBM, FDM, SPH, DEM) in combination to specifically tailored
GUIs to deliver accuracy, performance and easiness to use even for
engineers with limited CFD expertise.

#### Bio

Dr. Ernesto Monaco got his Master Degree in Aerospace Engineering at University of Naples in 2004. In 2009 he obtained a Ph.D. at Southampton University about Lattice Boltzmann simulations of complex multiphase flows, which has been his most relevant research interest since then. From 2008 to 2013 and 2016 to Spring 2018 he was Post-Doctoral researcher, respectively at TU-Clausthal and Erlangen University (Germany). After working as software developer at Fluidyna (now part Altair Group) he is leader of the LBM group at ESS (Engineering Software Steyr) since July 2018.


### Pierre Sagaut (Aix-Marseille Université): Unsteady simulations of complex turbulent flows using Lattice-Boltzmann Methods

#### Abstract
The presentation deals with recent developments in the design of
Lattice-Boltzmann methods (LBM) for the simulation of turbulent flows
in complex geometries, with a broad range of applications ranging from
urban physics, micrometeorology to aerospace engineering. Two key
issues are addressed, more precisely 1) accounting for realistic
thermodynamics (from perfect gas with compressibility effects to humid
air with phase changes) while optimizing the numerical efficiency of
the method and 2) stabilizing the method while preserving the
low-dispersion/low-dissipation feature of the original LBM method. The
latter point will be addressed within the Scale Resolving Approach for
turbulent flow simulation, and the optimization of the stabilizing
procedure for Implicit LES, explicit LES and hybrid RANS-LES methods
will be discussed. Since LBM is based on the use of Cartesian grids,
the development of efficient immersed boundary techniques along with
the coupling with turbulent wall models is a key issue that will be
illustrated.  During the talk, the emphasis will be put on the Hybrid
Recursive Regularized LBM approach developed at the M2P2 laboratory
that is implemented in the ProLB software.

#### Bio

 Professor Pierre Sagaut is Director of M2P2 Laboratory at
 Aix-Marseille Université, associated with CNRS and Ecole Centrale
 Marseille. He also holds the Chaire Airbus-Renault-Safran on
 Lattice-Boltzmann Methods for CFD. He has a PhD in Fluid mechanics
 (1995) from Université Pierre et Marie Curie, and has worked for
 various organisations including the French National Aerospace
 Lab. Since 1997, he has successfully supervised 68 PhD students and
 15 postdoctoral fellows. He has published extensively in journals,
 conferences and books on topics such as computational fluid dynamics,
 aerodynamics, aeroacoustics, uncertainty quantification, aerospace
 engineering, urban physics, turbulence dynamics and modelling,
 numerical methods. Prof Sagaut has received numerous honours and
 awards including 2002: John Green prize (International Council for
 Aeronautical Sciences) in 2002, Prize of Association of European
 Research Establishments in Aerospace (shared with G. Desquesnes,
 E. Manoha, M. Terracol) in 2007 and Grand Prix de l’Académie des
 Sciences/ EADS  in  « Science & Engineering » in 2010. He has served
 as an editor/editor-in-chief for five international journals.


### Sauro Succi (Istituto Italiano di Tecnologia & CNR & University of Rome, Italy: Harvard University, USA): Simulating Dropland: Computational Design of Exotic Soft Materials with an Eye to Exascale Computing

#### Abstract

We present recent variants of the Lattice Boltzmann method
for the mesoscale modelling of exotic soft materials, such as
microﬂuidic crystals, dense and mul-ticore emulsions and recent
Petascale simulations of deep-sea glassy sponges, with an eye on
prospective exascale simulations

#### Bio

Dr Sauro Succi holds a degree in Nuclear Engineering from the
University of Bologna and a PhD in Plasma Physics from the EPFL,
Lausanne, Switzerland. He has held a research staﬀ position at the IBM
European Center for Scien-tiﬁc and Engineering Computing, Rome. Till
2018 he served as a Director of Research at the Istituto Applicazioni
Calcolo of the Italian National Research Council in Rome and he is
also a Research Associate of the Physics Department of Harvard
University and a regular Visiting Professor at the Institute of
Ap-plied Computational Science at the School of Engineering and
Applied Sciences of Harvard University. Since 2018 he is a Senior
Research Executive and Prin-cipal Investigator at the Center for Life
Nanosciences of the Italian Institute of Technology at La Sapienza,
Rome.

He has published extensively on a broad range of topics in
computational physics, soft matter and the interface between physics
and biology.

He is the author of the highly cited monograph ”The lattice Boltzmann
equation for ﬂuid dynamics and beyond”, (Oxford Univ. Press, 2001) and
”The Lattice Boltzmann Equation for Complex States of Flowing Matter”
(OUP, 2018).

Dr Succi is an elected Fellow of the American Physical Society (1998),
a a member of the European Physical Society and an elected member of
the Academia Europaea (2015). He has received the Humboldt Prize in
physics (2002), the Killam Award of the the University of Calgary
(2005) and the Ra-man Chair of the Indian Academy of Sciences
(2011). In 2017, he has been awarded a European Research Council
Advanced Grant on the computational design of mesoscale porous
materials. He is also the recipient of the 2017 APS Aneesur Rahman
Prize for Computational Physics for seminal contributions to the
development and application of the Lattice Boltzmann method and the
2019 Bernie J. Alder CECAM prize for exceptional contributions to the
microscopic simulation of matter.