.. _overset_overview:

########################
Optimization with OpenVSP, OpenMDAO and Overset-Meshes
########################
This tutorial will mainly explain how overset meshes for ADFlow are generated. We will use OpenVSP to create 
the geometry, generate a surface mesh with Pointwise (subject to charge) and extrude the volume mesh with pyhyp.

OpenVSP does not only provide the geometry, it can also be hooked up with pygeo. This means, the mesh 
can be warped based on OpenVSP variables thus allowing optimization without the hassle of generating an FFD control
box. This capability will also be showed.

We will do this process on the `ONERA M6 Wing <https://www.grc.nasa.gov/WWW/wind/valid/m6wing/m6wing.html>`_. It is 
a common example to validate flow solvers in the transonic regime. Note that an overset mesh might not be needed
for a simple geometry like a wing.

Table of Contents
=================

.. toctree::
   :maxdepth: 1

   overset_theory
   overset_vsp
   overset_surface_mesh



Directory Structure
===================
::

    overset
    |-- geo
    |   |-- onera_m6.vsp
    |   |-- profile_m6.dat