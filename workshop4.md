---
layout: page
title: "Workshop IV: Inverse Problems and Optimisation"
---

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

### Thursday 6 May 2021

- 13:00 Introduction
- 13:05 <a href="#james-nagy">James Nagy (Emory University)</a> - *Krylov Subspace Regularization for Inverse Problems*
- 13:55 <a href="#bill-lionheart">Bill Lionheart (University of Manchester)</a> - *Computational Challenges in Rich and Nonlinear Tomography*
- 14:45 **Break**
- 15:15 <a href="#chris-budd">Chris Budd (University of Bath)</a> - *Adaptive methods for meteorological data assimilation*
- 16:05 <a href="#george-biros">George Biros (U. T. Austin)</a> - *Scalable algorithms for diffeomorphic image registration*
- 17:00 **Open Discussion**

### Friday 7 May 2021

- 13:00 <a href="#marta-betcke">Marta Betcke (UCL)</a> - *Stochastic solution of sparsely sampled inverse problem in large-scaler PAT using ray based full wave approximation*
- 13:50 <a href="#vladimir-druskin">Vladimir Druskin (Worcester Polytechnic Institute)</a> - *Data-Driven Reduced Order Models, Ladder Networks, and Inverse Scattering*
- 14:40 **Break**
- 15:10 <a href="#jiri-jaros--felix-lucka">Jiri Jaros (Brno University) / Felix Lucka (CWI)</a> - *Computational Challenges in Photoacoustic and Ultrasonic Breast Imaging*
- 16:00 <a href="#oscar-bruno">Oscar Bruno (Caltech)</a> - *Fast spectral integral solvers for general electromagnetic structures*
- 17:00 **Virtual drinks and discussions**


### James Nagy
#### Krylov Subspace Regularization for Inverse Problems

<div class="iframeVideo">
<iframe width="420" height="315" src="https://www.youtube.com/embed/iwb1GvXRqpw" frameborder="0" allowfullscreen></iframe>
</div>

Krylov subspace-based regularization approaches that combine direct matrix factorization methods on small subproblems with iterative solvers have been shown to be very effective for inverse problems. The methods are very efficient for large scale inverse problems, they have the advantage that various regularization approaches can be used, and they can also incorporate methods to automatically estimate regularization parameters. We introduce new Krylov based solvers for the computation of low-rank approximate solutions, adopting an iteratively reweighted norm approach to reformulate nuclear norm regularization as a sequence of quadratic problems. Numerical experiments show that our new solvers are competitive with other state-of-the-art solvers for low-rank problems, and deliver reconstructions of increased quality with respect to other classical Krylov methods.

### Bill Lionheart
#### Computational Challenges in Rich and Nonlinear Tomography

<div class="iframeVideo">
<iframe width="420" height="315" src="https://www.youtube.com/embed/Davb-4KVT_k" frameborder="0" allowfullscreen></iframe>
</div>

Advances in measurement technology means that increasingly tomographic data can be acquired in which for each ray we have much more than a scalar measurement: a diffraction pattern, a spectrum or a polarization change are examples. The measurement speed and the number of pixel detectors for each projection increases as does the rate of data acquisition. In addition many examples of tomographic problems are non-linear, even if their linearization is still sparse. While increases in processor speed, number of processors and memory allow us to tackle bigger problems faster a deeper mathematical understanding also reduces computational demands. In this talk we will look specifically at the reconstruction problems for diffraction tomography (using X-rays, electrons and neutrons), time of flight neutron tomography, and polarimetric neutron tomography as examples.

### Chris Budd
#### Adaptive methods for meteorological data assimilation

<div class="iframeVideo">
<iframe width="420" height="315" src="https://www.youtube.com/embed/wJX5Hn2bFHY" frameborder="0" allowfullscreen></iframe>
</div>

Data assimilation is widely used as part of a meteorological weather
forecast in order to combine a model forecast with incoming data to
more accurately represent the atmospheric state. This is often done
as part of an optimisation procedure. An important aspect
of doing this accurately is to estimate the covariance of the various errors
made in the data and in the calculation. Spurious correlations between errors
in this inverse problem can lead to significant forecasting errors. In this talk
I will show how an adaptive method, based on ideas from optimal transport,
can significantly reduce these spurious correlations, leading to much more
accurate weather foerecasts.

### George Biros
#### Scalable algorithms for diffeomorphic image registration

<div class="iframeVideo">
<iframe width="420" height="315" src="https://www.youtube.com/embed/5N3yB2iULJo" frameborder="0" allowfullscreen></iframe>
</div>

3D image registration is one of the most fundamental and computationally expensive operations in medical image analysis.  Despite the importance of image registration, only a few implementations of large deformation diffeomorphic registration packages support heterogeneous and distributed memory architectures.  Our algorithm uses a partial differential equation constrained optimal control formulation. Finding the optimal deformation map requires the solution of a highly nonlinear problem that involves pseudo-differential operators, biharmonic operators, and pure advection operators both forward and backward in time. A key issue is the time to solution, which poses the demand for efficient optimization methods as well as an effective utilization of high performance computing resources. To address this problem we use a preconditioned, inexact, Gauss-Newton-Krylov solver. Our algorithm integrates several components: a spectral discretization in space, a semi-Lagrangian formulation in time, analytic adjoints, different regularization functionals (including volume-preserving ones), a spectral preconditioner, a highly optimized distributed Fast Fourier Transform, and a cubic interpolation scheme for the semi-Lagrangian time-stepping.  We solve a 256^3-resolution image registration problem in five seconds on a single NVIDIA Tesla V100, with a performance speedup of 70% compared to the state-of-the-art. In our largest run, we register 2048^3 resolution images (25B unknowns; approximately 152× larger than the largest problem solved in state-of-the-art GPU implementations) on 64 nodes with 256 GPUs on TACC’s Longhorn system.

### Marta Betcke
#### Stochastic solution of sparsely sampled inverse problem in large-scaler PAT using ray based full wave approximation

<div class="iframeVideo">
<iframe width="420" height="315" src="https://www.youtube.com/embed/n44EEq4riaw" frameborder="0" allowfullscreen></iframe>
</div>

We propose a novel Hamilton-Green (HG) solver for the forward and adjoint equations in photoacoustic tomography with heterogenous sound-speed.  The HG solver can be viewed as a ray tracing approximation of the unknown heterogeneous Green’s function in the respective Green’s integral formula. The solution for each sensor is computed independently at a fractional cost of the full wave solution enabling efficient partial-operator evaluation used in e.g. ray-based methods for CT or PET or stochastic methods popular in machine learning applications. We present results for HG deployed in stochastic primal hybrid gradient method for sparse data PAT reconstruction. Joint work with Francesc Rullan.

### Vladimir Druskin
#### Data-Driven Reduced Order Models, Ladder Networks, and Inverse Scattering

<div class="iframeVideo">
<iframe width="420" height="315" src="https://www.youtube.com/embed/QKJ79Jv3n-I" frameborder="0" allowfullscreen></iframe>
</div>

We discuss a novel unified framework for imaging with active electromagnetic and acoustic arrays in complex environments over a broad range of regimes ranging from lossless wave propagation to diffusion-dominated regime. Many conventional approaches to imaging based on linearizations fail in the presence of strong non-linear effects such as multiple scattering, high contrasts, losses, dispersion, etc. Even if applied iteratively in optimization framework, they may lack robustness and converge slowly due to a highly non-convex data misfit.

One of classical tasks of the network synthesis is to construct ROMs realized via ladder networks matching rational approximations of a targeted filter transfer function. The inverse scattering can be also viewed in the network synthesis framework. The proposed framework is based on data-driven reduced order models (ROMs) and it avoids the issues faced by the conventional techniques. A ROM of the underlying partial differential equation (PDE) is constructed from the measured data, hence the designation “data-driven”. The key is continuum interpretation of the equivalent network in terms of the underlying medium properties, aka embedding.  It encodes the PDE coefficients which carry information about the target. Construction of the ROM is a highly non-linear process that “absorbs” much of the nonlinearity of the problem, thus making the subsequent imaging a lot more straightforward.  For example, it allows us to avoid local minima in optimization frameworks and for some problems even to develop direct nonlinear imaging algorithms.

We will show a number  of 2D numerical experiments ranging from seismic full wave inversion   to radar imaging.   This is joint work with Liliana Borcea, Alex Mamonov, Shari Moskow, Mikhail Zaslavsky and Jorn Zimmerling.


### Jiri Jaros / Felix Lucka
#### Computational Challenges in Photoacoustic and Ultrasonic Breast Imaging

<div class="iframeVideo">
<iframe width="420" height="315" src="https://www.youtube.com/embed/dPd11oQIVZo" frameborder="0" allowfullscreen></iframe>
</div>

Novel scanner prototypes allow to probe the breast with high-resolution, three-dimensional imaging techniques without delivering harmful radiation. In particular combining photo-acoustic tomography (PAT) and ultrasound computed tomography (USCT) promises access to high-quality images of tissue parameters with important diagnostic value. However, the involved image reconstruction problems are very challenging from an experimental, mathematical and computational perspective. In this talk, we want to illustrate some of the computational challenges using data from an ongoing clinical feasibility study. In particular, we will discuss Full Waveform Inversion (FWI) approaches for speed-of-sound imaging with USCT and iterative model-based reconstruction approaches for PAT. To obtain high-quality 3D images with 0.5mm resolution or less, PDEs modeling ultrasound propagation through domains with different material properties needs to be solved repeatedly and to a high accuracy. After reviewing our current results, we will discuss future developments that will broaden the range of clinical scenarios in which these techniques are viable.

### Oscar Bruno
#### Fast spectral integral solvers for general electromagnetic structures

<div class="iframeVideo">
<iframe width="420" height="315" src="https://www.youtube.com/embed/Xf7vaelM6m4" frameborder="0" allowfullscreen></iframe>
</div>

We present fast spectral electromagnetic solvers that address some of the main difficulties associated with the simulation of realistic engineering electromagnetic problems in the frequency- and time-domain. Based on the use of Green functions and fast high-order methods for evaluation of integral operators, these algorithms can solve, with high-order accuracy, problems of electromagnetic propagation and scattering for large and complex three-dimensional structures and devices -- including e.g. silicon devices, structured lenses, and metamaterials. In particular, we will consider the important but challenging problem of inverse design and optimization of optical and photonic devices of large electrical sizes. A variety of applications will be presented demonstrating the significant design capabilities inherent in the new methods, as well as the improvements these algorithms can provide, over other approaches, in generality, accuracy, and speed. Time permitting, a novel class of accelerated Green function methods will be mentioned.
