.. tab-set::

   .. tab-item:: Supervisor of LBM_Saclay code
   
      .. grid:: 2
         :gutter: 4
         :margin: 0 0 0 0

         .. grid-item-card::
            :columns: 6

            .. figure:: ./source/FIGS/Logo_LBM_Saclay.png
               :class: align-left
               :height: 300
               :width: 260
               :scale: 40
      
            Since 2018, I am involved in the development of the C++ multi-architecture HPC LBM_Saclay code for which I am the supervisor. The source code can be found on the :bdg-link-info:`Codev-Tuleap repository <https://codev-tuleap.cea.fr/projects/lbmsaclay/>`. LBM_Saclay has evolved from the fortran code SILABE3D and can run on several architectures (CPU and GPU) e.g. Jean-Zay V100 (IDRIS) and Topaze A100 (CCRT). Several LBM schemes are implemented for simulating various phase-field models for Multiphase/Multicomponent (MPMC) flows with phase change (Watch :bdg-ref-danger:`videos of simulations <Areas of modeling>`). 
      
         .. grid-item-card::
            :columns: 6

            .. figure:: ./source/FIGS/Logo-Workforce_LBM_Saclay.png
               :class: align-left
               :height: 300
               :width: 280
               :scale: 40
               
            I participate in writing the documentation of LBM_Saclay (see the html version on :bdg-link-primary:`LBM_Saclay's documentation <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/index.html>`) [R18]_, and specifications for code maintenance [r6]_. The code is mainly applied for R&D purposes, I facilitate the meetings of LBM_Saclay team for coordination. It is also used in the 16h training session on «An introduction of Lattice Boltzmann Methods» in the doctoral school SMEMaG (public: PhD students). It is also used to practice "phase-field models" taught at CEA--INSTN (engineers) and Sorbonne University (M2 students). 

   .. tab-item:: My approach in CEA projects

      In the CEA projects to which I contribute (see :bdg-ref-black-line:`Involvement-CEA-Projects`), after discussion with the experimental scientists who are involved in the same project, my approach is divided into three main stages described below. More details are given in :bdg-ref-black-line:`Skills-and-Areas`.

      .. grid:: 2
         :gutter: 4
         :margin: 0 0 0 0

         .. grid-item-card::
            :columns: 6

            1) **Derivation of Partial Derivative Equations** (PDEs) for the target application. Since 2012, the derivation of such PDEs is based on the *phase-field theory* which combines rigorously the interface-capturing with the thermodynamic of the system (see :bdg-link-primary:`Fundamentals of phase-field theory <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/src_doc/05_COURSES/Course_PF/01_Fundamentals_PF.html>`).
            2) **Writing the numerical schemes of those PDEs**. Since 2009 [R8]_, the derivation of numerical schemes are based on the *Lattice Boltzmann Methods* (LBM -- see :bdg-link-primary:`Overview of Lattice Boltzmann Methods <https://cea-lbm-saclay.github.io/LBM_Saclay_Documentation/src_doc/05_COURSES/Course_LBM/02_Overview_LBM.html>`). After **code implementation**, **verifications** are performed with academic test cases.
            3) **Running HPC simulations** for diverse phenomenologies of «fluid dynamics and thermodynamics», «material science» and «flow & transport in porous media». My whole approach is summarized in Fig. 1.

         .. grid-item-card::
            :columns: 6
         
            .. figure:: ./source/FIGS/Fig_MyApproach.png
               :name: Fig-MyApproach
               :figclass: align-center
               :align: center
               :height: 230
               :width: 450
               :scale: 100 %
      
               My approach in the CEA projects.
      
      .. div:: sd-py-2

      .. grid:: 3
         :margin: 1 1 1 1

         .. grid-item::
            :columns: 1

            |br|

         .. grid-item::
            :columns: 10

            .. dropdown:: ...
               :icon: comment

               The applications depend on the projects that support my activities. For example, in SIVIT, the phenomena are those observed in the nuclear glasses for waste management. In SIACY, they are relative to the liquid-liquid extraction devices, and in VESTA they concern the maturation of gels.

         .. grid-item::
            :columns: 1

            |br|

   .. tab-item:: Scales of modelling
      
      .. rst-class:: align-center

         See all details of my involvements in :bdg-ref-black-line:`Involvement-CEA-Projects`

      .. tab-set::

         .. tab-item:: 2002--2005

            .. grid:: 2
               :gutter: 4
               :margin: 0 0 0 0

               .. grid-item-card::
                  :columns: 6

                  **Kilometric-scale**: Au début de ma carrière j'ai travaillé sur les méthodes de “problème inverse” en géosciences, tout d'abord dans le cadre de ma thèse soutenue en 2002, puis dans les activités de mon labo au SFME sur la thématique du stockage des déchets en partenariat avec l'ANDRA. En Fig 2, je donne un exemple d'application de ces méthodes pour la simulation des écoulements sous le site du CEA/Cadarache. La problématique était de savoir si en situation accidentelle d'une INB, un contaminant pouvait polluer une source d'eau potable à l'extérieur du site.

               .. grid-item-card::
                  :columns: 6

                  .. _target-Fig-Cad:
   
                  .. figure:: ./source/FIGS/Fig_CEA-Cad.png
                     :name: Fig-CEA-Cad
                     :figclass: align-center
                     :align: center
                     :height: 120
                     :width: 450
                     :scale: 100 %
      
                     Finite element simulation of underground flow

         .. tab-item:: 2004--2013

            .. grid:: 2
               :gutter: 4
               :margin: 0 0 0 0

               .. grid-item-card::
                  :columns: 6

                  **Metric-scale**: ensuite j'ai travaillé dans le cadre du projet “Maîtrise des risques et Impacts sur l'environnement” sur les transferts dans les milieux poreux insaturés. Pour cela je me suis intéressé sur une manip en colonne bien instrumentée au DRMP (Fig. 3) et qui a permis de valider des modèles basés sur les équations fractionnaires. Cette thématique a conduit à un projet ANR TRAM pour “transport anormal en milieu poreux” en collaboration avec l'IFPEN et l'université d'Avignon et pour lequel j'étais le responsable CEA.

               .. grid-item-card::
                  :columns: 6

                  .. container:: sphinx-features
   
                     .. figure:: ./source/FIGS/Fig-Anomalous.png
                        :name: Fig-CEA-Beeti
                        :figclass: align-center
                        :align: center
                        :height: 140
                        :width: 450
                        :scale: 100 %

                        Anomalous transport studied on BEETI device
                     

         .. tab-item:: Since 2012

            .. grid:: 2
               :gutter: 4
               :margin: 0 0 0 0

               .. grid-item-card::
                  :columns: 6

                  **Micrometric-scale**: je m'intéresse aux modèles de suivi d'interfaces sur plusieurs phénomènes observés dans les verres nucléaires pour la vitrification des déchets. À cette échelle, les simulations permettent de prévoir les conditions d'apparition d'une nouvelle phase liquide (séparation de phase) ou solide (cristallisation) qui peuvent impacter les propriétés physiques des colis. Elles permettent aussi de faire le pont entre les simul de dynamique moléculaire du DPME et les approches homogénéisées à l'échelle métrique.

                  Pour mener à bien mes simulations, j'ai dialogué avec des hydrogéologues des bassins versants, des spécialistes de science du sol, et des physico-chimistes du verre. Ensuite j'ai fait le pont avec les mathématiques appliquées.

               .. grid-item-card::
                  :columns: 6

                  .. _target-Fig-Observation:
   
                  .. figure:: ./source/FIGS/Fig_Observations.png
                     :name: Fig-CEA-Mar
                     :figclass: align-center
                     :align: center
                     :height: 220
                     :width: 450
                     :scale: 100 %
      
                     Observations made by experimental scientists in SIVIT and VESTA projects

               

   