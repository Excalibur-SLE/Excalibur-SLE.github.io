---
layout: page
title: "Workshop V: Data Visualisation and Data Flows"
---

## 16-17 June 2021 13:00-18:00 BST (GMT+1)

The traditional workflow of the computational engineer or scientist:
simulate, store in full, process later – will no longer be fit for
purpose at exascale and a tighter coupling of simulation and
post-processing codes will be required. Stakeholders at this workshop
will discuss the challenges of visualisation and data flow at exascale
and topics such as: (i) limits of current workflows given roadmaps of
future storage and I/O bandwidth; (ii) prescribed and automated
in-situ data extraction; (iii) in-situ dimension reduction techniques;
(iv) intelligent data compression; interactive analysis of large
ensembles of simulations; and, (v) immersive visualisation using VR
and AR. Invited speakers will include experts from exascale programs,
open source initiatives, vendors and commercial visualization software
companies. The workshop panels will include practitioners from
industry, government laboratories and academia, who are pioneering
visualisation approaches at the current limits of both simulated and
experimentally measured data flows.

### Wednesday 16 June 2021 - Data Flow at Exascale

- 13:00 Welcome
- 13:10 <a href="#anna-scaife">Anna Scaife (University of Manchester)</a> - *Big telescope, big data: towards exascale with the SKA*
- 13:40 <a href="#andrew-richards">Andrew Richards (Diamond Light Source)</a> - *The challenge of capturing, managing, and visualising experimental data at Diamond*
- 14:10 **Break**
- 14:40 <a href="#scott-klasky">Scott Klasky (ORNL)</a> - *Exascale Data Management*
- 15:10 <a href="#ozan-tugluk">Ozan Tugluk (Brown University)</a> - *Analysis driven compression of scientific data with MGARD*
- 15:40 **Break**
- 16:10 <a href="#alastair-dewhurst">Alastair Dewhurst (STFC)</a> - *Globally distributed data management at the LHC*
- 16:45 **Breakout social**
- 17:30 Close


### Thursday 17 June 2021 - Data Visualisation at Exascale

- 13:00 Welcome
- 13:10 <a href="#elisabeth-mayer--peter-coveney"> Elisabeth Mayer (Leibniz Supercomputing Centre) / Peter Coveney (UCL)</a> - *Visualization of human-scale blood flow simulation using Intel OSPRay Studio on SuperMUC-NG*
- 13:40 <a href="#dave-demarle">Dave DeMarle (Intel)</a> - *OSPRay in-situ visualization of GR Chombo black hole collisions, things are starting to come together now*
- 14:10 **Break**
- 14:40 <a href="#dave-pugmire">Dave Pugmire (ORNL)</a> - *Scientific Visualization as a Service*
- 15:10 <a href="#will-usher">Will Usher (Intel)</a> - *Interactive Visualization of Terascale Data in the Browser: Fact or Fiction?*
- 15:40 **Break**
- 16:10 <a href="#nick-leaf">Nick Leaf (NVIDIA)</a> - *Cinematic Scientific Visualization with ParaView and Omniverse*
- 16:45 **Breakout social**
- 17:30 Close


### [Anna Scaife](https://www.skatelescope.org/teamska/anna-scaife)
#### Big telescope, big data: towards exascale with the SKA
Unlike optical telescopes, radio interferometers do not image the sky directly but require specialized image formation algorithms. For the Square Kilometre Array (SKA), the computational requirements of this image formation are extremely demanding due to the huge data rates produced by the telescope. This processing will be performed by the SKA Science Data Processor facilities and a network of SKA Regional Centres, which must not only deal with SKA-scale data volumes but also with stringent science-driven image fidelity requirements.

### [Andrew Richards](https://www.diamond.ac.uk/Home/News/LatestNews/2017/19-01-17.html)
#### The challenge of capturing, managing, and visualising experimental data at Diamond
Diamond Light Source is the UK’s national synchrotron. It works like a giant microscope, harnessing the power of electrons to produce bright light that scientists can use to study anything from fossils to jet engines to viruses and vaccines. Diamond provides national science infrastructure that is free at the point of use. Primary facilities are the national Synchrotron along with Cryo electron microscopy (EM) at the Harwell Campus, all available to researchers through a competitive application process, provided that published results are in the public domain. Over 14,000 researchers from across life and physical sciences both from academia and industry use Diamond to conduct experiments, assisted by approximately 700 staff.

The data challenge at Diamond starts with the collection of experimental data from each of the individual end-stations (beamlines and EM) whose data volume per experiment can range from gigabytes to multiple terrabytes of data. Pre COVID-19, Diamond was trending towards collecting 1PB of data per calendar month with this set to continue to increase as Diamond further upgrades beamlines and detectors. Diamond is also in the advanced stages of planning the Diamond-II, a major upgrade in capability of the synchrotron itself. The current data archive contains nearly 30PB of data at present and is predicted that by 2030 the archive could be between 500PB and 1EB of experimental data.

The data pipeline can be separated into the initial data acquisition phase associated with the actual experimental visit to Diamond and a period of 30 days for initial processing, followed by a longer period of data analysis that occurs post-visit and can extend for many months or years. After the initial 30-day period all data from the experimental visit is archived and can be retrieved as required for the later data analysis, either locally to Diamond or an external location controlled by the user. Within this pipeline the biggest challenges are associated with the initial data capture and near real-time feedback, visualisation, to the users on ‘how the experiment is going’, through to providing sufficient ongoing computational resources to allow for subsequent data analysis. In this latter stage work is ongoing to better segregate on-premise systems for the initial data analysis phase and to facilitate the use of external cloud like platforms whether at the STFC or with commercial providers such as AWS and Google for later stages of data analysis. 

The final challenge yet to be fully addressed is the future requirement to make data open. Diamond is working alongside many other synchrotrons as part of projects such as ExPANDS EU Horizon 2020 funded) to ensure data can be FAIR (Findable, Accessible, Interopable, resusable) and accessible to end users form multiple data locations.


### [Scott Klasky](https://csmd.ornl.gov/profile/scott-klasky)
#### Exascale Data Management
The pace of scientific data generation is outstripping the rate of improvement in the computing resources needed to save, transmit, and analyze those data. With the first generation of exascale machines and the next generation of experimental and observational facilities on the horizon, there will be a huge strain on computing hardware due to unprecedented data volumes and velocities. This landscape highlights the growing need to move, manage, reduce and store the data as efficient as possible. As part of the Exascale Computing Project (ECP), the ADIOS team has worked together to create an extensible framework to achieve these goals. Our team has worked with many large scale applications including:  the Fusion Whole Device Modeling project  (WDMApp), E3SM - Energy Exascale Earth System Model, ECP-WarpX project, along with work with the LAMMPS framework, the GTC fusion code, the SPECFEM3D_GLOBE project, the KSTAR fusion reactor, the CANDLE project,  and the SKA project.  In all of these projects we will show examples of how ADIOS has enabled new science, by giving the scientists a new capability to perform I/O at large scale, to couple codes, and to enable next-generation science.

### [Ozan Tugluk](https://appliedmath.brown.edu/people/ozan-tugluk)
#### Analysis driven compression of scientific data with MGARD
Rapidly evolving high performance computing resources result in an exponential increase in data storage demands. Scientific data compression is a much cheaper alternative to constantly expanding data storage units. However, due to the nature of current floating point representations and scientific simulations, lossless compression is rarely relevant. Lossy compression offers a viable alternative, however there are two main challenges, namely hesitancy of application scientists and seemingly low compression ratios. We present our approach to tackling these two problems. Our approach involves compressing the data so that a prescribed loss is guaranteed, not on the original data, but on the quantities of interest which are computed from the data. Advantages of this approach are twofold, preserving quantities of interest results in better compression, and assures the user that compression artifacts will not adversely affect their analysis. We present our mathematical framework, and our compression tool/library MGARD (MultiGrid Adaptive Reduction of Data) which was developed for CODAR (Co-design Center for Online Data Analysis and Reduction at the Exascale).  We provide illustrative examples from experimental and computational data.

### Alastair Dewhurst
#### Globally distributed data management at the LHC
The LHC experiments are already managing over an Exabyte of data between them.  This is expected to increase by at least an order of magnitude for the High Luminosity LHC in 2027. As the UK Tier-1, RAL plays a key role in archiving, processing and distributing data across the 100+ sites that make up the Worldwide LHC Computing Grid (WLCG).  I will describe the current setup of the RAL Tier-1 and our plans to continue to scale these services.  I will also talk about Rucio and FTS, which are the data management tools used by the LHC and how RAL is enabling scientific communities outside High Energy Physics to take advantage of the tools and experiences from the LHC.

### Elisabeth Mayer / Peter Coveney
#### Visualization of human-scale blood flow simulation using Intel OSPRay Studio on SuperMUC-NG
HemeLB is a highly scalable, 3D blood flow solver capable of generating high-resolution simulations of blood flow through human-scale vasculatures. Post-processing such simulations is a significant challenge, particularly due to the volume of data generated. We have utilized Intel OSPRay Studio to visualize generated data timeseries directly on the production machine — SuperMUC-NG at LRZ. We use a custom input plugin to efficiently map the simulation data whilst eliminating complex pre-processing. This allows the full domain simulated by HemeLB to be quickly observed by users for assessment

### Dave DeMarle
#### OSPRay in-situ visualization of GR Chombo black hole collisions, things are starting to come together now
An ongoing collaboration between Intel's Advanced Rendering and Visualization Architecture (ARVA) group and the COSMOS Intel Parallel Computing Centre at The Stephen Hawking Centre for Theoretical Cosmology has been pushing the boundaries of our understanding of the universe. Theoretically proposed events, such as Boson star collisions and cosmic string decays as well as only recently experimentally detected events such as black hole collisions are being numerically simulated on supercomputing platforms to test ideas about their underlying physical nature. These events all emit gravitational waves of the kind that were recently detected by the LIGO telescope.
 
Simulating these types of processes is challenging because of the massive range of scales involved and inherent numerical costs of calculating them. Visualization of the calculated gravitational waves is an important means to debug simulation correctness, understand the physical processes involved, and communicate results with the public. ARVA's OSPRay ray tracing engine has been integral to these visualizations.
 
In this talk we will introduce the collaborators and present some of the more impactful visualizations that the team has created. We will also describe the software architecture behind the studies and preview upcoming work that will enhance the highly scalable ParaView Catalyst based in situ infrastructure utilized by the team.

### [Dave Pugmire](https://csmd.ornl.gov/profile/dave-pugmire)
#### Scientific Visualization as a Service
One of the primary challenges facing scientists is extracting understanding from the large amounts of data produced by simulations, experiments, and observational facilities. The use of data across the entire lifetime ranging from real-time to post-hoc analysis is complex and varied, typically requiring a collaborative effort across multiple teams of scientists. Over time, three sets of tools have emerged: one set for analysis, another for visualization, and a final set for orchestrating the tasks. This trifurcated tool set often results in the manual assembly of analysis and visualization workflows, which are one-off solutions that are often fragile and difficult to generalize.  To address these challenges, we propose a serviced-based paradigm and a set of abstractions to guide its design. These abstractions allow for the creation of services that can access and interpret data, and enable interoperability for intelligent scheduling of workflow systems. This work results from a codesign process over analysis, visualization, and workflow tools to provide the flexibility required for production use.  This talk will describe a forward-looking research and development plan that centers on the concept of visualization and analysis technology as reusable services, and also describes several real-world use cases that implement these concepts.


### [Will Usher](https://www.willusher.io)
#### Interactive Visualization of Terascale Data in the Browser: Fact or Fiction?
Information visualization applications have become ubiquitous, in no small part thanks to the ease of wide distribution and deployment to users enabled by the web browser. Scientific visualization applications, relying on native code libraries and parallel processing, have been less suited to such widespread distribution, as browsers do not provide the required libraries or compute capabilities. In this paper, we revisit this gap in visualization technologies and explore how new web technologies, WebAssembly and WebGPU, can be used to deploy powerful visualization solutions for large-scale scientific data in the browser. In particular, we evaluate the programming effort required to bring scientific visualization applications to the browser through these technologies and assess their competitiveness against classic native solutions. As a main example, we present a new GPU-driven isosurface extraction method for block-compressed data sets, that is suitable for interactive isosurface computation on large volumes in resource-constrained environments, such as the browser. We conclude that web browsers are on the verge of becoming a competitive platform for even the most demanding scientific visualization tasks, such as interactive visualization of isosurfaces from a 1TB DNS simulation. We call on researchers and developers to consider investing in a community software stack to ease use of these upcoming browser features to bring accessible scientific visualization to the browser.

### Nick Leaf
#### Cinematic Scientific Visualization with ParaView and Omniverse
Cinematic visualization aims to incorporate the high visual fidelity of film-oriented rendering into more traditional scientific workflows. Advanced rendering is useful for engaging broader audiences, but it also enhances the perception of data in everyday analyses--provided the rendering is fast enough for everyday use. I'll cover two rendering technologies that NVIDIA has developed for ParaView in partnership with Kitware, the OptiX pathtracing backend and the IndeX volume rendering plugin. I'll also give an overview of NVIDIA Omniverse, a platform for data fusion and collaborative work on large 3D scenes, built on the open-source USD format. Applications built inside Omniverse, like Omniverse Create, natively support high-quality interactive rendering and real time physical simulation. I'll illustrate with a few examples of how these capabilities can be combined to improve both the fidelity and impact of visualization.



