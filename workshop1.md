---
layout: default
---

## Workshop on "Software Engineering"

Getting scientific applications ready for exascale is a huge
undertaking. Very few of today’s codes can take full advantage of
current Tier-1 systems, such as the 750,000 core ARCHER-2, let alone
the millions of cores on heterogeneous systems that are anticipated
with exascale. This workshop will explore the challenges facing the
scientific computing community, and cover exascale readiness
techniques such as performance portability, algorithmic fault
tolerance, asynchronous programming, and improving scalability. The
workshop will include contributions from experts from international
exascale initiatives such as ECP in the USA and EuroHPC. It will also
include input from leading vendors such as Cray/HPE, NVIDIA, AMD,
Intel and Codeplay. Key questions will be: (i) how different
simulation tools can be software-engineered for interoperability at
scale; (ii) how future software engineering and new languages
abstractions most effectively support the separation of concerns in
development; and, (iii) how multi-physics simulations can optimally
exploit heterogeneous hardware platforms.

## Tuesday 14 July 2020
#### All times are in BST (GMT+1)

- 13:00 Introduction, Garth Wells, University of Cambridge
- 13:15 <a href="https://youtu.be/HiutQfwhYSg">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#ulrich-rüde-fau-erlangen-nürnberg">Ulrich Rüde, FAU Erlangen-Nürnberg</a>
- 13:45 <a href="https://youtu.be/4ypw1AXMP6E">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#lorena-barba-george-washington-university">Lorena Barba, George Washington University</a>
- 14:15 break
- 14:45 <a href="#tim-costa-nvidia">Tim Costa, NVIDIA</a>
- 15:15 <a href="https://youtu.be/zamUkpm1gRA">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#jed-brown-university-of-colorado-boulder">Jed Brown, University of Colorado, Boulder</a>
- 15:45 break
- 16:15 <a href="https://youtu.be/16qFqQpXqjk">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#jeff-hammond-intel">Jeff Hammond, Intel</a>
- 16:45 breakout - social


## Wednesday 15 July 2020
#### All times are in BST (GMT+1)

- 13:00 Introduction, Simon McIntosh-Smith, University of Bristol
- 13:15 <a href="https://youtu.be/nSXaouT4ZUo">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#sato-mitsuhisa-riken-japan">Sato Mitsuhisa, Riken, Japan</a>
- 13:45 <a href="https://youtu.be/ewkVPGldsCQ">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#tom-deakin-university-of-bristol-uk">Tom Deakin, University of Bristol, UK</a>
- 14:15 break
- 14:45 <a href="https://youtu.be/ANbR5WATyQQ">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#hal-finkel-argonne-national-laboratory">Hal Finkel, Argonne National Laboratory</a>
- 15:15 <a href="https://youtu.be/MR4qaY7xeD8">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#mike-heroux-sandia-national-laboratories">Mike Heroux, Sandia National Laboratories</a>
- 15:45 break
- 16:15 <a href="https://youtu.be/CQNpbbYzZqE">![video](/assets/images/yt_icon_rgb.png)</a> <a href="#kumudha-narasimhan-codeplay">Kumudha Narasimhan, Codeplay</a>
- 16:45 breakout - social


### Ulrich Rüde, FAU Erlangen-Nürnberg
##### [waLBerla - Towards extreme scale multiphysics simulations](https://doi.org/10.13140/RG.2.2.17176.62727)

Programming supercomputers remains challenging. Multiple levels of
parallelism must be exploited in the core, on the compute node, and
between nodes. Heterogeneous hardware with accelerators further
complicate development and achieving performance portability. The
[waLBerla framework](https://doi.org/10.1016/j.camwa.2020.01.007) addresses these challenges by providing
building blocks for simulations on block-structured grids. Adaptive
mesh refinement and load balancing are shown to
scale. Meta-programming techniques are used to generate [highly
efficient code for CPUs and GPUs](https://arxiv.org/abs/2001.11806). The development workflow can
thus start from the symbolic formulation of the problem. The steps of
deriving the specific simulation method,  simplifying the computation
by symbolic manipulation, and eventually generating efficient code for
various architectures is performed automatically. We will demonstrate
the features of waLBerla with some multiphysics applications.


### Lorena Barba, George Washington University
##### ExaFMM - 10+ years, 7 re-writes. The tortuous progress of computational research.

The story of writing codes in my lab for one algorithm, over and over,
illustrates the sometimes tortuous progress of computational
research. This tale speaks of the inherent tension between the
students’ goals (one-time use, performance brag, thesis results) and
the goals of reusable, sustainable software. ExaFMM is a new re-write
of a high-performance implementation of the fast multipole method in
C++. My students and a post-doc have written at least seven separate
code bases for this algorithm, over more than 10 years, and we hope
this one is the definitive one.


### Tim Costa, NVIDIA
##### Accelerated Computing in 2020 and Beyond


### Jed Brown, University of Colorado, Boulder
##### Libraries, communities, and performance portability

We take a holistic view of efficiently using human and compute
resources via libraries and community building.  Performance
portability is a key ingredient, albeit with different meaning at
different levels of the software stack.  We discuss some traps and
fallacies, as well as techniques and methods of evaluation that help
to align incentives and improve communication.

### Jeff Hammond, Intel
##### Programming heterogeneous systems using SYCL 2020, OpenMP 5 and oneAPI

I will explain Intel's oneAPI initiative, including direct programming
support for accelerators using SYCL 2020 and OpenMP 5.
Special consideration will be give to programmers who do not want to
port their code to ever platform using a different programming model
or who need to maintain simulation codes for one or more decades.

### Sato Mitsuhisa, Riken, Japan
##### The SuperComputer "Fugaku" with available software and programming tools

We have been carrying out the FLAGSHIP 2020 to develop the Japanese
next-generation flagship supercomputer, Post-K, named as “Fugaku”
recently. In the project, we have designed a new Arm-SVE enabled
processor, called A64FX, as well as the system including interconnect
with the industry partner, Fujitsu. The processor is designed for
energy-efficiency and sustained application performance. The “Fugaku”
is being installed and scheduled to be put into operation for public
service around 2021. In this talk, several features and software,
programming tools of the “Fugaku” system will be presented as well as
some preliminary performance results.


### Tom Deakin, University of Bristol, UK
##### Performance Portability across Diverse Architectures

The range of computer architectures used in supercomputers today is
growing in diversity. The Exascale machines due to be online by next
year (2021) and the UK’s Tier-2 systems showcase the variety of
architectures we need to think about: high-performance CPUs and GPUs
from different hardware vendors. As HPC specialists, we need to write
and maintain our codes to make sure they work efficiently on this wide
and changing range of hardware. We want to write performance portable
codes that run well everywhere. To do this we need robust ways to
measure and evaluate performance portability, and we need to use write
codes using programming models which are simultaneously performant and
portable. This talk highlights some of the ongoing research into
performance portability from the High Performance Computing Research
Group at the University of Bristol.

### Hal Finkel, Argonne National Laboratory
##### Programming Models and Compiler Technology for Exascale

Exascale systems will present application authors with a diverse set
of programming models targeting a diverse set of hardware
architectures. While many of these hardware architectures will be
similar, the heterogeneity of each requires us to carefully consider
our application designs and the technologies that will allow those
applications to be portable between systems. In this talk, we'll
discuss the ecosystem of programming models that will be available in
the coming years, including OpenMP, SYCL, Kokkos, RAJA, HIP, and CUDA,
and the compiler technology required for each. In the space of
programming models, there is a trade off between user control and the
potential for compiler optimizations, and work exploring compiler
optimizations for parallel programs will be highlighted. Finally,
we'll discuss auto-tuning and the potential advantages of using
just-in-time compilation to maximize performance.


### Mike Heroux, Sandia National Laboratories
##### The Extreme-scale Scientific Software Stack for Collaborative Open Source Software

Open source, community-developed reusable scientific software represents a large and growing body of capabilities. Linux distributions, vendor software stacks and individual disciplined software product teams provide the scientific computing community with usable holistic software environments containing core open source software components. At the same time, new software capabilities make it into these distributions in a largely ad hoc fashion.
The Extreme-scale Scientific Software Stack (E4S),first announced in November 2018, along with its community-organized scientific software development kits (SDKs), is a new community effort to create lightweight cross-team coordination of scientific software development, delivery and deployment and a set of support tools an processes targeted at improving scientific software quality via improved practices, policy, testing and coordination.
[E4S](https://e4s.io), which announced the release of Version 1.0 in November 2019, is an open architecture effort, welcoming teams that are developing technically compatible and high-quality products to participate in the community. E4S and the SDKs are sponsored by the US Department of Energy Exascale Computing Project (ECP), driven by our need to effectively develop, test, deliver and deploy our open source software products on next generation platform to the scientific community.
In this presentation, we introduce E4S, discuss its design and implementation goals and show examples of success and challenges so far. We will also discuss our connection with other key community efforts we rely upon for our success and describe how collaboration around E4S can be realized.


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
