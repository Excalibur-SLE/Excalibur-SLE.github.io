---
layout: default
---

## Tuesday 14 July 2020

### Ulrich Rüde, FAU Erlangen-Nürnberg
##### waLBerla - Towards extreme scale multiphysics simulations

Programming supercomputers remains challenging. Multiple levels of
parallelism must be exploited in the core, on the compute node, and
between nodes. Heterogeneous hardware with accelerators further
complicate development and achieving performance portability. The
waLBerla framework[^1] addresses these challenges by providing
building blocks for simulations on block-structured grids. Adaptive
mesh refinement and load balancing are shown to
scale. Meta-programming techniques are used to generate highly
efficient code for CPUs and GPUs[^2]. The development workflow can
thus start from the symbolic formulation of the problem. The steps of
deriving the specific simulation method,  simplifying the computation
by symbolic manipulation, and eventually generating efficient code for
various architectures is performed automatically. We will demonstrate
the features of waLBerla with some multiphysics applications.

[^1]: Martin Bauer, Sebastian Eibl, Christian Godenschwager, Nils Kohl, Michael Kuron, Christoph Rettinger, Florian Schornbaum, Christoph Schwarzmeier, Dominik Thönnes, Harald Köstler, Ulrich Rüde (2020), waLBerla: A block-structured high-performance framework for multiphysics simulations, Computers & Mathematics with Applications,. https://doi.org/10.1016/j.camwa.2020.01.007.

[^2]: Bauer, M., Köstler, H., & Rüde, U. (2020). lbmpy: A flexible code generation toolkit for highly efficient lattice Boltzmann simulations. arXiv preprint arXiv:2001.11806.

### Lorena Barba, George Washington University
##### Title

### Tim Costa, NVIDIA
##### Title

### Jed Brown, University of Colorado, Boulder
##### Title

### Jeff Hammond, Intel
##### Title

## Wednesday 15 July 2020

### Sato Mitsuhisa, Riken, Japan
##### Fugaku with available software and programming tools

### Tom Deakin, University of Bristol, UK
##### Performance Portability

### Hal Finkel, Argonne National Laboratory
##### Programming Models and Compiler Technology for Exascale

Exascale systems will present application authors with a diverse set of programming models targeting a diverse set of hardware architectures. While many of these hardware architectures will be similar, the heterogeneity of each requires us to carefully consider our application designs and the technologies that will allow those applications to be portable between systems. In this talk, we'll discuss the ecosystem of programming models that will be available in the coming years, including OpenMP, SYCL, Kokkos, RAJA, HIP, and CUDA, and the compiler technology required for each. In the space of programming models, there is a trade off between user control and the potential for compiler optimizations, and work exploring compiler optimizations for parallel programs will be highlighted. Finally, we'll discuss auto-tuning and the potential advantages of using just-in-time compilation to maximize performance.


### Mike Heroux, Sandia National Laboratories
##### Title


### Kumudha Narasimhan, Codeplay
##### SYCL Performance and Portability

Over recent years heterogeneous systems have become more popular
across HPC systems, with over 100 supercomputers in the TOP500
incorporating GPUs or other accelerators. Such platforms have
different performance characteristics and optimization requirements.
In order to make the most of various accelerators, a programming model
is required to support portability without losing performance. The
SYCL programming model allows users to write heterogeneous programs
using completely standard C++, and so developers have access to the
power of C++ templates meta programming to develop a highly
parameterized kernels. SYCL offers performance, programmability, and
portability with extensive hardware support.

Developers can currently use SYCL to target a wide range of processors
including those from Intel, Arm, NVidia  and Renesas.  Alongside this
support, however, is a growing ecosystem of projects developed using
SYCL that provide developers with optimized libraries for common
operations and algorithms used in AI.

During this presentation, we will examine some of these projects. Show
how these libraries can be used to offer portability and performance,
and how these libraries can be used to accelerate complex HPC
applications.  Codeplay Software will discuss some of the available
papers detailing the implementation, performance, and programmability
of these libraries and frameworks.