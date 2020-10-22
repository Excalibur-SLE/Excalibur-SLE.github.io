---
layout: default
---

## Workshop on "Data Assimilation and Uncertainty Quantification at the exascale", 24-25 September 2020

Uncertainty Quantification (UQ) includes the propagation of
uncertainty from inputs to outputs through simulators, as well as
inverse problems resulting from the calibration of models against
observations. One key tool is building emulators (surrogate
statistical models) to replace computationally expensive
simulators. Data assimilation (DA) synergizes computer simulations and
real-world data, e.g. from weather prediction to hazard modelling,
urban analytics and biological science, with observations used to
update simulations in real time. With the interaction between forward
simulations and information-driven methods, techniques for UQ and DA
are specifically challenged by the scale of problems that exascale
computing will enable. Developing efficient UQ and DA algorithms will
also be a major challenge, with close collaborations between RSEs and
researchers necessary.

### 13:00 BST - 17:00 BST each day

## Thursday 24 September 2020
#### All times are in BST (GMT+1)

- 13:00	<a href="https://youtu.be/QHp0oDGYZnY">![video](/assets/images/yt_icon_rgb.png)</a> Introduction, Garth Wells, University of Cambridge
- 13:05	<a href="https://youtu.be/_zpOwrF-7Ew">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#takemasa-miyoshi-riken">Takemasa Miyoshi (RIKEN)</a>
- 13:35	<a href="https://youtu.be/ofMU5DOjAnY">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#andrew-lorenc-met-office">Andrew Lorenc (Met Office)</a>
- 14:05	<a href="https://youtu.be/lDMjh15G96g">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#alberto-carrassi-reading">Alberto Carrassi (Reading)</a>
- 14:35	break
- 15:00	<a href="https://youtu.be/W3hd2jY9dDU">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#sam-hatfield-ecmwf">Sam Hatfield (ECMWF)</a>
- 15:15	<a href="https://youtu.be/b-oquVsU70M">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#mariya-mamajiwala-ucl">Mariya Mamajiwala (UCL)</a>
- 15:30	<a href="https://youtu.be/1i7rjrPrhww">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#tuomas-koskela-ucl">Tuomas Koskela (UCL)</a>
- 15:45	<a href="https://youtu.be/wR8oJpSqiEA">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#wayne-arter-ukaea">Wayne Arter (UKAEA)</a>
- 16:00	Break
- 16:20	Panel
- 16:45	breakout - social

## Friday 25 September 2020
#### All times are in BST (GMT+1)

- 13:00	<a href="https://youtu.be/Hdz4azed3Ok">![video](/assets/images/yt_icon_rgb.png)</a> Introduction, Serge Guillas (UCL)
- 13:05	<a href="https://youtu.be/BKnrgQ7Tpg0">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#aretha-teckentrup-edinburgh">Aretha Teckentrup (Edinburgh)</a>
- 13:35	<a href="https://youtu.be/2ditRpjDpBI">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#mike-giles-oxford">Mike Giles (Oxford)</a>
- 14:05	<a href="https://youtu.be/PqBJQlHGUwE">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#habib-najm-sandia">Habib Najm (Sandia)</a>
- 14:35	break
- 15:00	<a href="https://youtu.be/lmFQo4PFbX0">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#eric-daub-turing">Eric Daub (Turing)</a>
- 15:15	<a href="https://youtu.be/Wu22W77KQFk">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#dimitra-salmanidou-ucl">Dimitra Salmanidou (UCL)</a>
- 15:30	<a href="https://youtu.be/R9N9AOPvZbs">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#maxime-vassaux-ucl">Maxime Vassaux (UCL)</a>
- 15:45	<a href="https://youtu.be/8eMXgHFl5io">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#wouter-edeling-cwi">Wouter Edeling (CWI)</a>
- 16:00	Break
- 16:20	Panel
- 16:45	breakout - social


## Thursday 24 September 2020

### Takemasa Miyoshi (RIKEN)
### Big Data, Big Computation, and Machine Learning in Numerical Weather Prediction

At RIKEN, we have been exploring a fusion of big data and big computation, and now with AI techniques and machine learning (ML). This fusion will bring a breakthrough to the emulation or surrogate modeling of big process-driven simulators and will bring a fundamental advance to both UQ and DA. The new Japan’s flagship supercomputer “Fugaku”, ranked #1 in the most recent TOP500 list (https://www.top500.org/) in June 2020, is designed to be efficient for both double-precision big simulations and reduced-precision machine learning applications, aiming to play a pivotal role in creating super-smart “Society 5.0.” Our group in RIKEN has been pushing the limits of numerical weather prediction (NWP) through two orders of magnitude bigger computations by taking advantage of the previous Japan’s flagship supercomputer named “K computer”. The efforts include ensemble Kalman filter experiments with 10240 ensemble members and 100-m-mesh, 30-second-update “Big Data Assimilation” (BDA) fully exploiting the big data from the novel phased array weather radar. Now with the new “Fugaku” in mind, we explore to integrate big data, big computation, and ML. The data produced by NWP models become bigger and moving around the data to other computers for ML may not be feasible. Having a next-generation computer like “Fugaku”, good for both big NWP computation and ML, may bring a breakthrough toward creating a new methodology of fusing data-driven (inductive) and process-driven (deductive) approaches in meteorology. This presentation will introduce most recent work on BDA’s real-time weather forecasting demonstration in August 2020, with some specific research examples of DA-AI fusion at RIKEN.


### Andrew Lorenc (Met Office)
### Ensemble DA systems for convective-scale NWP

The historical improvements in NWP have been due to higher resolution and Bayesian DA methods.  Implementation of the latter at high resolution has only been possible thanks to the assumption that errors are small, which permits Gaussian approximations to the PDF.
Convective-scale global NWP, with expected observing systems, will not always have small errors, so current approaches cannot be extended.  One solution is a subtle change of objective.  Most economically valuable forecasts do not require high-resolution accuracy – for instance a probability forecast for extreme weather in a space and time region can be reliable without being able to predict exactly where and when in the region the severe weather will occur.  Convective-scale NWP systems need to focus on improving such forecasts.
I discuss how current DA methods might be extended to initialise convective-scale ensembles, and mention alternative approaches.

### Alberto Carrassi (Reading)
### Combining data assimilation and machine learning to emulate hidden dynamics and to infer unresolved scale pametrisation.

A novel method based on the combination of data assimilation and machine learning is introduced.
The combined approach is designed for emulating hidden, possibly chaotic, dynamics and/or to
devise data-driven parametrisations of unresolved processes in dynamical numerical models.
The method consists in applying iteratively a data assimilation step, here ensemble Kalman filter or
smoother, and a neural network. Data assimilation is used to effectively handle sparse and noisy
data. The output analysis is spatially complete and is used as a training set by the neural network.
The two steps can then be repeated iteratively.
We will show the use of this combined DA-ML approach in two set of experiments. In the first one
the goal is to infer a full surrogate model. Here we carry experiments using the chaotic 40-variables
Lorenz 96 model and show that the surrogate model achieves high forecast skill up to two
Lyapunov times, it has the same spectrum of positive Lyapunov exponents as the original dynamics
and the same power spectrum of the more energetic frequencies. In this context we will also
illustrate the sensitivity of the method to critical setup parameters: the forecast skill decreases
smoothly with increased observational noise but drops abruptly if less than half of the model
domain is observed.
In the second set of experiments, the goal is to infer unresolved-scale parametrization. Data
assimilation is applied to estimate the full state of the system from a truncated model. The unresolved
part of the truncated model is viewed as model errors in the DA system. In a second step, ML is used
to emulate the unresolved part, a predictor of model error given the state of the system. Finally, the
ML-based parametrisation model is added to the physical core truncated model to produce a hybrid
model.
The DA component of the proposed approach relies on an ensemble Kalman filter while the ML
parametrisation is represented by a neural network. Experiments are carried out using the two-scale
Lorenz model and the reduced-order coupled atmosphere-ocean model MAOOAM. We will show
that in both cases the hybrid model yields better forecast skills than the truncated model, and its
attractor resembles much more the original system’s attractor than what achieved by the truncated
model.
References:
- https://doi.org/10.1016/j.jocs.2020.101171
- https://arxiv.org/pdf/2009.04318.pdf

### Sam Hatfield (ECMWF)
### Constructing tangent-linear and adjoint models through automatic differentiation of neural networks

Many numerical weather prediction centres rely on the 4D-Var approach to data assimilation. With this algorithm, a linearisation of the forecast model, the tangent-linear model, is used to propagate model state perturbations forwards in time, and the adjoint of this linearised model is used to propagate gradients backwards in time. In this way, a cost function measuring the fit of a four-dimensional model trajectory to observations can be minimised efficiently. The construction and maintenance of these separate tangent-linear and adjoint models is usually done manually, a time-consuming, tedious and error-prone process. This is especially the case for physical parametrisation schemes, whose code can be esoteric and which can contain sharp discontinuities which complicate the linearisation process. In this talk I will propose an alternative. By replacing physical parametrisation schemes with an emulator based on a neural network, we can construct tangent-linear and adjoint models trivially by taking advantage of the by-design differentiability of the neural network. I will present results showing how an operational numerical prediction model using this scheme can produce forecasts competitive in skill with the original scheme.


### Mariya Mamajiwala (UCL)
### Efficient parameter estimation with non-linear stochastic filtering : a modified parameter dynamics

In data assimilation, the standard way of estimating parameters is to treat them as additional states which evolve as Wiener processes. Thus, unlike the original system states, there is no physically motivated drift field governing the parameter dynamics. This often manifests in slower or no convergence of the parameters. When convergence does occur, the final estimates may have a higher sampling variance or equivalently there may be a need for a higher ensemble size for the stochastic filtering method to work. Motivated by this limitation, we propose a modified parameter dynamics wherein an additional drift field is introduced based on a psuedo-energy term created out of the available observations. Through numerical simulations, we demonstrate the advantages of the modified parameter dynamics over the conventional method in the context of state and parameter estimations of the Lorenz-1963 model. Specifically, we show that the new parameter dynamics enables a reduction in the ensemble size by at least an order of magnitude.

### Tuomas Koskela (UCL)
### Lessons learned from developing high performance particle filtering software

We are developing fast implementations of state-of-art data assimilation code targeted at HPC in the RADDISH project at UCL. The aim is to create tools that can be applied to forecasting tsunamis and modeling the evacuation of people and vessels in coastal areas. In this talk I will discuss the development of a parallel particle filter code for data assimilation of the tsunami forecast model, that we intend to make more widely available. I will introduce technologies and practices that we have found useful, discuss the parallel algorithm for particle filtering, show preliminary scaling results and discuss the lessons we have learned along the way.


### Wayne Arter (UKAEA)
### Data assimilation approach to analysing systems of ordinary differential equations

The problem of parameter fitting for nonlinear oscillator models to noisy time series is addressed using a combination of Ensemble Kalman Filter and optimisation techniques. Encouraging preliminary results for acceptable sampling rates and noise levels are presented. Application to the understanding and control of tokamak nuclear reactor operation is discussed.

## Friday 25 September 2020

### Aretha Teckentrup (Edinburgh)
### Learning functions from data

We are interested in the problem of recovering an unknown function from a finite number of point evaluations. Applying Gaussian process regression to this problem allows for recovery with uncertainty quantification, as we obtain a probability distribution on the unknown function.
A great challenge in Gaussian process regression is that hyper-parameters appearing in the mean and covariance structure of the emulator, such as parameters governing smoothness and typical length scales, are a-priori unknown. We work in the framework of empirical Bayes, where values of hyper-parameters are learnt from the data, along with the posterior mean and covariance. Using results from scattered data approximation, we provide a convergence analysis of the method used to learn an unknown, deterministic function.


### Mike Giles (Oxford)
### Multilevel Monte Carlo Methods

In the presentation I will give a quick review of the Multilevel Monte Carlo (MLMC) method, and then outline current research on
a) estimating the Expected Value of Partial Perfect Information (EVPPI) and Expected Value of Sample Information (EVSI);
b) using approximate random variables and reduced precision arithmetic within a nested MLMC formulation to reduce the total computational cost.

### Habib Najm (Sandia)
### Uncertainty Quantification in Large Scale Computational Models

Uncertainty quantification (UQ) in large scale computational models of physical systems faces the two key challenges of high dimensionality and high computational cost. Such models often involve a large number of uncertain parameters, associated with various modeling constructions, as well as uncertain initial and boundary conditions. Exploring such high-dimensional spaces typically necessitates the use of a large number of computational samples, which, given the cost of large scale computational models, is prohibitvely expensive and frequently infeasible.  I will discuss a set of UQ methods, and a UQ workflow, to address this challenge. The suite of methods includes global sensitivity analysis with polynomial chaos regression and compressive sensing, coupled with multilevel multifidelity methods. The combination of these tools is often useful to reliably cut-down dimensionality with feasible computational costs, identifying a lower-dimensional subspace on uncertain parameters where subsequent adaptive sparse quadrature methods can be feasibly employed, with accurate estimation of predictive uncertainty. I will illustrate this UQ workflow on problems of practical relevance.

### Eric Daub (Turing)
### mogp_emulator: A Software Library for Uncertainty Quantification Using Gaussian Process Emulators

We present an overview of mogp_emulator, a software library for fitting Gaussian Process Emulators to complex simulation codes in order to perform robust Uncertainty Quantification and model calibration. The library is written in Python and includes a number of tools for Experimental Design and History Matching addition to a GP emulator implementation to provide an end-to-end suite of tools for calibrating models to data. We highlight recent improvements to the GP implementation which include formula-based mean functions and prior distributions for hyperparameter values to enable a full Bayesian fitting procedure that produces more robust fits to high dimensional data. We illustrate an application to a nonlinear projectile simulation that is provided as a documented example in the code base.

### Dimitra Salmanidou (UCL)
### Uncertainty quantification workflows for high-resolution tsunami hazard prediction in North Cascadia.

Statistical emulators are stochastic approximations of the numerical response that can be utilized to assess the results of numerous scenarios when the computational models become expensive to run. They thus comprise valuable methods for uncertainty quantification. In this work we analyse the workflows followed for the uncertainty quantification of tsunami hazard in British Columbia. Earthquake tsunamis generated from the Cascadia subduction zone could pose a major threat for the area. Probabilistic hazard prediction can aid disaster mitigation and preparedness; the objective is to provide with high-resolution probabilistic outputs of the tsunami elevation. To do so, we build Multi-Output Gaussian Process emulators with the aid of a sequential design approach that adaptively selects the training sets of runs.  We discuss the different stages followed in this study and the computational speeds of the modelling approach.


### Maxime Vassaux (UCL)
###  Large-scale UQ of single-scale molecular dynamics and heterogeneous multiscale simulations of biomedical and advanced materials systems.

I will introduce in this talk two simulation applications we perform large-scale uncertainty quantification (UQ) on using advanced methods showing high scalability. On one side, I will discuss the use of the VECMAtk and its EasyVVUQ feature to perform tractable UQ of binding affinity calculations on a protein-ligand system simulated with molecular dynamics. Such application typically features a high-dimensional input parameter space which cannot be explored using Monte-Carlo sampling. On the other side, I will discuss the use of surrogate modelling to perform UQ of materials properties prediction using semi-concurrent multiscaling. Single multiscale simulations can already require exascale supercomputers, I will explain how training on-the-fly a surrogate model of the microscale model can be helpful to rapidly decrease the cost of subsequent multiscale simulations necessary for UQ.

### Wouter Edeling (CWI)
### Forward uncertainty propagation for high-dimensional input spaces using the VECMA toolkit

Parametric uncertainty arises due to imperfect knowledge in the input parameters of a computational model. Although this is not the only source of uncertainty, assessing the impact of the unknown input parameters is important as computational models are increasingly used in decision and policy making at different levels of society. It is not uncommon for a model to have hundreds of inputs, in which case many forward propagation techniques break down due to the well-known curse of dimensionality. In the Verified Exascale Computing for Multiscale Applications (VECMA,https://www.vecma.eu/) project, we are developing, amongst others, a toolkit for forward propagation of uncertainty. To tackle the high dimensionality, we are considering dimension-adaptive sampling approaches, which iteratively refine the sampling plan based on a suitable error metric. Moreover, we particularly focus on computationally expensive models, with applications ranging from epidemiological modelling of COVID-19 through fusion energy reactor design, drug discovery and weather forecasting to climate change, and are developing various mechanisms to effectively execute the (adaptive) ensembles on HPC resources. We will discuss our framework for uncertainty propagation, and discuss future challenges.
