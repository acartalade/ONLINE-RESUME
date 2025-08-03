.. |br| raw:: html

   <br />

.. _Skills-and-Areas:

Skills and areas of modeling
============================

My approach in CEA projects
---------------------------

.. admonition:: My approach in CEA projects
   :class: important

   After talking with the experimental scientists involved in the same project (see :ref:`Involvement-CEA-Projects`), I derive the Partial Derivative Equations (PDEs) for the target application. Since 2009 [R8]_, their numerical implementation is performed with the Lattice Boltzmann Methods (LBM -- see :bdg-link-primary:`Overview of LBM <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/src_doc/05_COURSES/Course_LBM/02_Overview_LBM.html>`). Since 2012 the derivation of those PDEs are based on the phase-field methods which combine rigorously the interface-capturing with the thermodynamic of the system (see :bdg-link-primary:`Basic concepts of phase-field theory <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/src_doc/05_COURSES/Course_PF/01_Fundamentals_PF.html>`).
   The applications are the phenomena observed in the nuclear glasses for waste management (see :numref:`target-Fig-Observation`. They are related to fluid flows, material science and porous media. The whole approach is summarized in :numref:`target-Fig-Approach`. Below are presented some keywords of my skills and areas of modeling.

   .. container:: twocol

      .. container:: leftside

         .. _target-Fig-Observation:
   
         .. figure:: ./FIGS/Fig_Observations.png
            :name: Fig-CEA-Cad
            :figclass: align-center
            :align: center
            :height: 230
            :width: 450
            :scale: 100 %
      
            Observations made by experimental scientists

      .. container:: rightside

         .. _target-Fig-Approach:
   
         .. figure:: ./FIGS/Fig_MyApproach.png
            :name: Fig-CEA-Cad
            :figclass: align-center
            :align: center
            :height: 230
            :width: 450
            :scale: 100 %
      
            My approach in the CEA projects


Mathematical and numerical methods 
----------------------------------

Implementation and practice of mathematical and numerical methods

.. admonition:: Phase-field modeling and Lattice Boltzmann Method

   .. container:: twocol

      .. container:: leftside

         **Phase-field Methods**: derivation of interface-tracking models for various applications such as two-phase flows (see e.g. :bdg-link-primary:`Mathematical model of two-phase flow <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/src_doc/02_MODELS/01_Fluid_Fluid/Model_NSAC_Comp.html>`) with or without phase change, crystal growth, dissolution of porous media and surfactant, Ostwald ripening :math:`\bullet` Derivation of constitutive laws :math:`\bullet` Asymptotic expansions between sharp interface and diffuse interface [P12]_ :math:`\bullet` Implementation in LBM_Saclay, verifications with the analytical solutions of Stefan's problem & benchmarks. 

      .. container:: rightside

         **Lattice Boltzmann Methods**: derivation and implementation of numerical schemes for various PDEs (Navier-Stokes, Advection-diffusion, fractional Eq., phase-field models, ...) (see e.g. :bdg-link-primary:`Equilibrium distribution function <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/src_doc/03_LBM_Schemes/A_Basic-LBM/03_Equilibrium-Functions_LBMSaclay.html>`) :math:`\bullet` :bdg-link-primary:`Chapman-Enskog expansion <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/src_doc/05_COURSES/Course_LBM/05_Chapman-Enskog.html>` [P7]_ :math:`\bullet` Programmer of a 3D LBM Fortran code SILABE3D [H1]_ (2009–2018) :math:`\bullet` involved in the development of the C++ multi-architecture HPC code LBM_Saclay :math:`\bullet` BGK, TRT and MRT [P10]_ collision operators :math:`\bullet` Adaptative Mesh Refinement with Lax-Wendroff scheme. 

.. admonition:: Supervisor of LBM_Saclay code
   :class: hint
   
   .. container:: twocol

      .. container:: leftside

         Since 2018, I am involved in the development of the C++ multi-architecture HPC code :bdg-link-info:`LBM_Saclay code <https://codev-tuleap.cea.fr/projects/lbmsaclay/>` for which I am the supervisor. LBM_Saclay has evolved from SILABE3D and can run on several architectures (CPU and GPU) e.g. Jean-Zay V100 (IDRIS) and Topaze A100 (CCRT). Several LBM schemes are implemented for simulating various phase-field models for Multiphase/Multicomponent (MPMC) flows with phase change. Videos of simulations can be watched by clicking on the red buttons of boxes «Fluid dynamics & thermic» and «Materials science & thermodynamics».
      
      .. container:: rightside

         I participate in writing the documentation of LBM_Saclay (see the html version on :bdg-link-primary:`LBM_Saclay's documentation <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/index.html>`) [R18]_, and specifications for code maintenance [r6]_. The code is mainly applied for R&D purposes, I facilitate the meetings of LBM_Saclay team for coordination. It is also used in the 16h training session on «An introduction of Lattice Boltzmann Methods» in the doctoral school SMEMaG (public: PhD students). It is also used to practice "phase-field models" taught at CEA--INSTN (engineers) and Sorbonne University (M2 students).

.. admonition:: Other mathematical methods

   .. container:: twocol

      .. container:: leftside

         Adjoint state method and optimization: in order to identify PDEs parameters, derivation of adjoint problems in continuous and discrete forms :math:`\bullet` Fortran implementation in a 2D finite element code and a finite difference code :math:`\bullet` Coupling with optimization algorithms e.g. with Hessian approximation such as BFGS with bound constraints [T1]_, [P5]_, [P9]_.
   
      .. container:: rightside

         Other methods: implementation and practice of finite difference method [R1]_ & [R2]_ and finite element methods [T1]_ with a direct solver :math:`\bullet` Euler explicit & implicit time-schemes :math:`\bullet` Continuous Time Random Walks and Volume Averaging Methods.

High Performance Computing & Informatics
----------------------------------------

.. admonition:: High Performance Computing & Informatics

   .. container:: twocol
      
      .. container:: leftside

         **Programming skills**: developer of SILABE3D (Fortran 77/90/2000) and LBM_Saclay (C++), ``makefile``, ``CMake``, Version control system with ``git``, debugger, architecture portability with ``Kokkos``. Coupling with math librairies (lapack, slatec, numerical recipes).

         **Post-processing**:  ``paraview``, ``gnuplot``,  ``python``.

         **Writing documentation** with ``Sphinx`` and ``rst`` files, deployment with GitHub pages.

      .. container:: rightside

         **High Performance Computing (HPC)**: practice of MPI commands in SILABE3D. Involved in the development of LBM_saclay: parallelization with MPI and multi-architecture portability with Kokkos library [R18]_. Batch scripts (SGE, slurm);

         **Operating System**: Linux, shell scripts, Windows. **Analytical calculus**: ``wxmaxima``
         
         **Writing skills**: ``LaTeX``, ``BibTeX``, ``LyX``; presentations with ``Beamer``, ``tikz``; figures with ``Matcha``.
         
Areas of modeling and simulations
---------------------------------

.. admonition:: Videos of simulations
   :class: error

   .. rst-class:: align-center

      |br|
      **Videos of simulations can be watched by clicking on the red buttons below** |br|
      |br|

.. admonition:: Computational Fluid Dynamics and thermodynamics
   :class: hint

   .. container:: twocol

      .. container:: leftside

         **Single phase flows**: Navier-Stokes (NS) :math:`\bullet` Incompressible flows and low Mach number :math:`\bullet` Eq. of state for compressible flows formulations :math:`\bullet` Natural convection with Boussinesq approximation [R8]_ :math:`\bullet` Non-Newtonian flows.

         **Immiscible two-phase flows**: phase-field models for :bdg-link-danger:`3D bubbles dynamics & buoyancy <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/_static/Vid3D_Buoyancy.webm>` :math:`\bullet` Spinodal decomposition, :bdg-link-danger:`Phase separation <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/_static/Vid_Separation.webm>`, :bdg-link-danger:`Nucleation and growth <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/_static/Vid_Nucleation.webm>`, with NS/Cahn-Hilliard model :math:`\bullet` NS/Conservative Allen-Cahn model for :bdg-link-danger:`3D Rayleigh-Taylor instability <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/_static/Vid3D_RT-2modes_900x900x512_Crop.webm>`, rising and :bdg-link-danger:`3D falling droplet <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/_static/Vid3D_Falling-Droplet_Compare_vA-vB_2views.webm>`, :bdg-link-danger:`2D Taylor bubble <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/_static/Vid_Taylor-Bubble2D_Compare_5Mo.webm>`, splash.

      .. container:: rightside

         **Two-phase flows with phase change**: phase-field model for liquid/gas phase change [P11]_, :bdg-link-danger:`Film Boiling <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/_static/Vid_FilmBoiling.webm>`. **Two-phase with surfactant**: surfactant effect on coalescence, rising and falling droplets. **Two-phase interacting with a solid phase**: :bdg-link-danger:`Leak of static and moving tank <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/_static/Vid_Container-Hole_Move-noMove.webm>` and :bdg-link-danger:`droplet on wetting and non-wetting surface <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/_static/Vid_Contact-Angle_Wetting_Surface.webm>`

         **Three-phase flows**: :bdg-link-danger:`Three-phase spinodal decomposition <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/_static/Vid_ThreePhases_Spinodal_Test22_vE.webm>` :math:`\bullet` Spreading lens :math:`\bullet` :bdg-link-danger:`2D simultaneous splashing droplet with Rayleigh-Taylor instability <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/_static/Vid_ThreePhases_RayleighTaylor_Splashing.webm>` or rising droplet :math:`\bullet` Simulations of surface tension effect for :bdg-link-danger:`3D separation of three immiscible fluids <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/_static/Vid3D_RT_Compare_vB-vC-vD_Publi.webm>`.

.. admonition:: Materials science and thermodynamics
   :class: hint

   .. container:: twocol

      .. container:: leftside

         **Solid-liquid phase transition**: phase-field models simulated by LBM for :bdg-link-danger:`3D crystal growth <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/_static/Vid3D_Crystal_100.webm>` [P7]_; pure substance [R12]_ and binary mixture [R13]_ :math:`\bullet` Functionals of free energy and grand-potential [P12]_ :math:`\bullet` Anisotropic surface tension and :bdg-link-danger:`Three interacting crystals <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/_static/Vid_3crystals.webm>` [P8]_ :math:`\bullet` «Enthalpy-porosity» approach for solidification.
         **Coupling with fluid flow**: simuls of phase-field model for :bdg-link-danger:`3D crystal growth with fluid flow <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/_static/Vid3D_Crystal-Flow.webm>` effect [P6]_.

      .. container:: rightside

         **Liquid-liquid mass transfer**: Ostwald ripening with fluid flow effect [P13]_ :math:`\bullet` derivation of phase-field model for ternary phase diagram and simplification for modeling the thermodynamic database (Calphad).

         **Dissolution and precipitation**: phase-field model of :bdg-link-danger:`Dissolution of porous media <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/_static/Vid_Dissolution_CT.webm>` (pore-scale) of binary [P12]_ and ternary mixtures.

.. rst-class:: align-center

   See other videos of simulations on LBM_Saclay's documentation (:bdg-link-primary:`Videos gallery of simulations with LBM <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/src_doc/02_MODELS/01_Fluid_Fluid/Model_NSAC_Comp.html>` and :bdg-link-primary:`run_training_lbm <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/src_doc/01_USER_GUIDE/RUN_TRAINING_LBM/runtraininglbm.html>`)

.. admonition:: Flow and transport in porous media
   :class: note

   .. container:: twocol

      .. container:: leftside

         **Flow and Transport in (un)saturated porous media**: hydrogeology of CEA-Cadarache :numref:`target-Fig-Cad` – watershed scale) [T1]_ :math:`\bullet` Dual-porosity models (:numref:`Fig-BEETI-device` – column scale) [R7]_ :math:`\bullet` Effective diffusion (Pore-scale) [R10]_ :math:`\bullet` Darcy-Brinkman-Forchheimer model [R8]_ and equation of Richards :math:`\bullet` Hydrodynamic dispersion.

         **Fractional Advection-Diffusion models**: LBM for fractional Eq. (PDEs with derivatives of real order in space) [P5]_ and time [P9]_

         .. _target-Fig-Cad:
   
         .. figure:: ./FIGS/Fig_CEA-Cad.png
            :name: Fig-CEA-Cad
            :figclass: align-center
            :align: center
            :height: 120
            :width: 450
            :scale: 100 %
      
            Finite element simulation of underground flow

      .. container:: rightside

         Validations and comparisons with equivalent random walks. Inverse problem on fractional parameter.

         .. _Fig-BEETI-device:
   
         .. figure:: ./FIGS/Fig_BEETI.png
            :name: Fig-CEA-Cad
            :figclass: align-center
            :align: center
            :height: 230
            :width: 450
            :scale: 100 %
      
            BEETI device

