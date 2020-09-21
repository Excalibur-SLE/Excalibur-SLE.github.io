---
layout: default
---

## Workshop on "Data Assimilation and Uncertainty Quantification" 24-25 September 2020

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

- 13:00	Introduction, Garth Wells, University of Cambridge
- 13:05	Takemasa Miyoshi (RIKEN)
- 13:35	Andrew Lorenc (Met Office)
- 14:05	Alberto Carrassi (Reading)
- 14:35	break
- 15:00	Sam Hatfield (ECMWF)
- 15:15	Mariya Mamajiwala (UCL)
- 15:30	Tuomas Koskela (UCL)
- 15:45	Wayne Arter (UKAEA)
- 16:00	Break
- 16:20	Panel
- 16:45	breakout - social

## Friday 25 September 2020
#### All times are in BST (GMT+1)

- 13:00	Introduction, Serge Guillas (UCL)
- 13:05	Aretha Teckentrup (Edinburgh) 
- 13:35	Mike Giles (Oxford)
- 14:05	Habib Najm (Sandia)
- 14:35	break
- 15:00	Eric Daub (Turing)
- 15:15	Dimitra Salmanidou (UCL)
- 15:30	Maxime Vassaux (UCL)
- 15:45	Wouter Edeling (CWI)
- 16:00	Break
- 16:20	Panel
- 16:45	breakout - social


The workshop will be hosted online with Zoom. In order to participate, please [register](https://www.eventbrite.co.uk/e/workshop-on-exascale-uncertainty-quantification-and-data-assimilation-tickets-117832627561).

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


### Wayne Arter (UKAEA)
### Data assimilation approach to analysing systems of ordinary differential equations

The problem of parameter fitting for nonlinear oscillator models to noisy time series is addressed using a combination of Ensemble Kalman Filter and optimisation techniques. Encouraging preliminary results for acceptable sampling rates and noise levels are presented. Application to the understanding and control of tokamak nuclear reactor operation is discussed.

