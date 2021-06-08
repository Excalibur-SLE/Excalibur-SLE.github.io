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
- 16:10 <a href="#alastair-dewhurst">Alastair Dewhurst (STFC)</a>
- 16:45 **Breakout social**
- 17:30 Close


### Thursday 17 June 2021 - Data Visualisation at Exascale

- 13:00 Welcome
- 13:10 <a href="#elisabeth-mayer--peter-coveney"> Elisabeth Mayer (Leibniz Supercomputing Centre) / Peter Coveney (UCL)</a> - *Visualization of human-scale blood flow simulation using Intel OSPRay Studio on SuperMUC-NG*
- 13:40 <a href="#dave-demarle">Dave DeMarle (Intel)</a> - *OSPRay in-situ visualization of GR Chombo black hole collisions, things are starting to come together now*
- 14:10 **Break**
- 14:40 <a href="#dave-pugmire">Dave Pugmire (ORNL)</a> 
- 15:10 <a href="#will-usher">Will Usher (Intel)</a> - *Interactive Visualization of Terascale Data in the Browser: Fact or Fiction?*
- 15:40 **Break**
- 16:10 <a href="#nick-leaf">Nick Leaf (NVIDIA)</a> - *Cinematic Scientific Visualization with ParaView and Omniverse*
- 16:45 **Breakout social**
- 17:30 Close

### Registration
The workshop will take place on Zoom: please [register](https://www.eventbrite.co.uk/e/excalibur-workshop-on-data-visualisation-and-data-flows-tickets-155943325685) to take part and receive further instructions.

### [Anna Scaife](https://www.skatelescope.org/teamska/anna-scaife)
#### Big telescope, big data: towards exascale with the SKA
Unlike optical telescopes, radio interferometers do not image the sky directly but require specialized image formation algorithms. For the Square Kilometre Array (SKA), the computational requirements of this image formation are extremely demanding due to the huge data rates produced by the telescope. This processing will be performed by the SKA Science Data Processor facilities and a network of SKA Regional Centres, which must not only deal with SKA-scale data volumes but also with stringent science-driven image fidelity requirements.

### [Andrew Richards](https://www.diamond.ac.uk/Home/News/LatestNews/2017/19-01-17.html)
#### The challenge of capturing, managing, and visualising experimental data at Diamond

### [Scott Klasky](https://csmd.ornl.gov/profile/scott-klasky)
#### Exascale Data Management
The pace of scientific data generation is outstripping the rate of improvement in the computing resources needed to save, transmit, and analyze those data. With the first generation of exascale machines and the next generation of experimental and observational facilities on the horizon, there will be a huge strain on computing hardware due to unprecedented data volumes and velocities. This landscape highlights the growing need to move, manage, reduce and store the data as efficient as possible. As part of the Exascale Computing Project (ECP), the ADIOS team has worked together to create an extensible framework to achieve these goals. Our team has worked with many large scale applications including:  the Fusion Whole Device Modeling project  (WDMApp), E3SM - Energy Exascale Earth System Model, ECP-WarpX project, along with work with the LAMMPS framework, the GTC fusion code, the SPECFEM3D_GLOBE project, the KSTAR fusion reactor, the CANDLE project,  and the SKA project.  In all of these projects we will show examples of how ADIOS has enabled new science, by giving the scientists a new capability to perform I/O at large scale, to couple codes, and to enable next-generation science.

### [Ozan Tugluk](https://appliedmath.brown.edu/people/ozan-tugluk)
#### Analysis driven compression of scientific data with MGARD
Rapidly evolving high performance computing resources result in an exponential increase in data storage demands. Scientific data compression is a much cheaper alternative to constantly expanding data storage units. However, due to the nature of current floating point representations and scientific simulations, lossless compression is rarely relevant. Lossy compression offers a viable alternative, however there are two main challenges, namely hesitancy of application scientists and seemingly low compression ratios. We present our approach to tackling these two problems. Our approach involves compressing the data so that a prescribed loss is guaranteed, not on the original data, but on the quantities of interest which are computed from the data. Advantages of this approach are twofold, preserving quantities of interest results in better compression, and assures the user that compression artifacts will not adversely affect their analysis. We present our mathematical framework, and our compression tool/library MGARD (MultiGrid Adaptive Reduction of Data) which was developed for CODAR (Co-design Center for Online Data Analysis and Reduction at the Exascale).  We provide illustrative examples from experimental and computational data.

### Alastair Dewhurst
#### Title TBA

### Elisabeth Mayer / Peter Coveney
#### Visualization of human-scale blood flow simulation using Intel OSPRay Studio on SuperMUC-NG
HemeLB is a highly scalable, 3D blood flow solver capable of generating high-resolution simulations of blood flow through human-scale vasculatures. Post-processing such simulations is a significant challenge, particularly due to the volume of data generated. We have utilized Intel OSPRay Studio to visualize generated data timeseries directly on the production machine — SuperMUC-NG at LRZ. We use a custom input plugin to efficiently map the simulation data whilst eliminating complex pre-processing. This allows the full domain simulated by HemeLB to be quickly observed by users for assessment

### Dave DeMarle
#### OSPRay in-situ visualization of GR Chombo black hole collisions, things are starting to come together now

### [Dave Pugmire](https://csmd.ornl.gov/profile/dave-pugmire)
#### Title TBA

### [Will Usher](https://www.willusher.io)
#### Interactive Visualization of Terascale Data in the Browser: Fact or Fiction?
Information visualization applications have become ubiquitous, in no small part thanks to the ease of wide distribution and deployment to users enabled by the web browser. Scientific visualization applications, relying on native code libraries and parallel processing, have been less suited to such widespread distribution, as browsers do not provide the required libraries or compute capabilities. In this paper, we revisit this gap in visualization technologies and explore how new web technologies, WebAssembly and WebGPU, can be used to deploy powerful visualization solutions for large-scale scientific data in the browser. In particular, we evaluate the programming effort required to bring scientific visualization applications to the browser through these technologies and assess their competitiveness against classic native solutions. As a main example, we present a new GPU-driven isosurface extraction method for block-compressed data sets, that is suitable for interactive isosurface computation on large volumes in resource-constrained environments, such as the browser. We conclude that web browsers are on the verge of becoming a competitive platform for even the most demanding scientific visualization tasks, such as interactive visualization of isosurfaces from a 1TB DNS simulation. We call on researchers and developers to consider investing in a community software stack to ease use of these upcoming browser features to bring accessible scientific visualization to the browser.

### Nick Leaf
#### Cinematic Scientific Visualization with ParaView and Omniverse
Cinematic visualization aims to incorporate the high visual fidelity of film-oriented rendering into more traditional scientific workflows. Advanced rendering is useful for engaging broader audiences, but it also enhances the perception of data in everyday analyses--provided the rendering is fast enough for everyday use. I'll cover two rendering technologies that NVIDIA has developed for ParaView in partnership with Kitware, the OptiX pathtracing backend and the IndeX volume rendering plugin. I'll also give an overview of NVIDIA Omniverse, a platform for data fusion and collaborative work on large 3D scenes, built on the open-source USD format. Applications built inside Omniverse, like Omniverse Create, natively support high-quality interactive rendering and real time physical simulation. I'll illustrate with a few examples of how these capabilities can be combined to improve both the fidelity and impact of visualization.



