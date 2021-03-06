 FEATool Multiphysics Changelog
================================


2019-10-14 version 1.11.1
-------------------------

- Support for IGES and STEP CAD file import
- Improved feature and boundary recognition for STL CAD file import
- Geometry and grid export to web browser
- Support for parsing space derivatives in time equation coefficients


2019-08-01 version 1.11
-----------------------

- Dedicated and improved treatment of internal/interior boundaries
- Fluid-structure interaction physics mode and solver
- MUMPS and iterative (GMRES and BiCGStab with ILU(k)) linear solvers
- Support for Gmsh v3/4 GEO file format geometry import and export
- New polyhedron, ellipsoid, cone, and torus geometry object primitives
- Support for external BRL-CAD and OpenCASCADE (Gmsh) geometry engines
- New examples and tutuorials for thermo-mechanical couplings,
  fluid-structure interaction, and non-Newtonian flow
- Added P1/P2 bubble, Nedelec curl, and Raviart-Thomas vector
  finite element shape functions


2019-04-15 version 1.10
-----------------------

- Finite element GUI script (fes) file format and built-in tutorials
- Support for edge constraints in 3D
- Support multiple STL sections and files during STL CAD file import
- Eigenvalue solver
- Functionality to make geometry object copies
- Deformation postprocessing plot option
- Support for spaces in paths/filenames in external grid generator
- Improved evaluation of expressions in grid points
- GUI improvements


2018-11-30 version 1.9
----------------------

- New compressible Euler equations physics mode
  (inviscid compressible flows)
- New swirl flow physics mode (axisymmetric non-zero
  azimuthal velocity)
- OpenFOAM CFD solver integration improvements
  - Support for general expressions (non-constant)
    in initial and boundary conditions
  - Support axisymmetry and swirl flows
  - Support for inviscid compressible flows
  - Improved k-epsilon/omega turbulence model interface
  - Realtime convergence curves plots
- NACA 4-series pre-defined wing geometry object
- Potential flow velocity field initialization
- Improved resolution of curved geometry boundaries
- Improved parametrization and meshing of curved boundaries
- Automatic shock capturing and stabilization for
  convection dominated flow regimes
- Support for first order P1P1 discretization and
  stabilization of flow problems
- Extended backwards compatibility to MATLAB 2009b
- Click and point evaluation for 2D surface plots
- Added built-in GUI tutorials and model examples


2018-05-17 version 1.8
----------------------

- GUI and CLI support for the external OpenFOAM CFD solver
- New CSG BSP tree based geometry engine
  The new geometry engine is used by default but original
  engine may be enabled with a set_geomlib(1) function call
- STL CAD geometry import and export support in 3D and 2D
- Cleaned up and consistent grid generation interfaces
  (identical boundary and subdomain numbering)
- Cached equation and expression parsing for faster evaluations
- Revised nonlinear Newton assembly and solver framework
  with automatic numeric Jacobian assembly calculation


2018-01-08 version 1.7.1
------------------------

- Built-in support for the external mesh generators Gmsh and Triangle
- Improved Gmsh grid import/export functionality with support for
  boundary information
- Redesigned and simplified grid mode toolbar
- GUI stability improvements and fixes
- GUI geometry export in Gmsh geo and Triangle poly formats
- gridextrude: support for extrusion of unstructured triangular
  simplex grids
- Swirl flow and periodic model examples
- Improved sparse matrix modification performance for Dirichlet
  boundary conditions and non-participating dependent variables
- Social sharing of postprocessing images and results


2017-08-10 version 1.7
----------------------

- FEniCS solve mode integration
- Plotly post mode integration
- Import/export of Dolfin XML grid format
- New physics modes:
  - Darcy's Law
  - Brinkman Equations
  - Electrostatics
  - Euler-Bernoulli Beam
  - Magnetostatics
- Built-in support for axisymmetry
- Solver support for active/inactive dependent variables
  in different subdomains and boundary couplings
- Added function to reconstruct inner boundaries
- Explicit construction of geometry object
  distance functions
- Support for 2nd order derivatives
  and equation definitions
- Parsing of groups of derivatives in parentheses
- New models and examples
- Support arbitrary order quadrature rules for
  all cell types and renamed cubrule* to quadrule*


2017-01-23 version 1.6
----------------------

- Support for external CFD solvers
- 3D fluid flow model examples using external CFD solvers
- Automatic quadrilateral grid generation in 2D
- Uniform grid refinement in 3D
- Projection to geometrical boundaries for uniform
  2D grid refinement and grid cell conversion
- 3 new axisymmetric stress-strain model examples
- New non-linear PDE models (in 1D and 2D ),
  and one new 2D Laplace equation test model
- 3rd-5th order Lagrange shape functions
- Cubic Hermite shape functions in 1D and 2D
- Support for tetrahedral quadrature up to order 5


2016-06-07 version 1.5
----------------------

- Redesigned 3D geometry engine
  - Calculates geometry boundary faces and edges for
    more precision in 3D geometry and grid generation
- 3D slice plot refactored and improved for new geometry engine
- New conforming hex to tet grid conversion method (1 Hex -> 28 Tets)
- GUI menu support for grid conversion and smoothing
- Allow partial rings in ringgrid generation function
- Generalized Navier-Stokes slip boundary conditions
  (supports curved and non-axis aligned boundaries)
- Allow external function calls for coefficients
- Progress waitbars for grid generation and solvers


2016-01-28 version 1.4
----------------------

- New physics mode features:
  - Heat transfer natural convection and radiation boundary conditions
  - Temperature stress-strain coupling in structural mechanics physics modes
  - Artificial and (anisotropic) streamline diffusion for stabilization
    of convection dominated high Re/Pe flows
  - Slip boundary condition option for the Navier-Stokes equations
- Grid import and export in Feat(Flow), GiD, GMV (General Mesh
  Viewer), Gmsh, and Triangle formats
- Define point sources and constraints
- New postprocessing features:
  - Data export in GMV (General Mesh Viewer) format
  - Save and export plots to image files (jpeg, png, eps)
  - Surface height plot option in two dimensions
  - Max and min boundary and subdomain evaluation functions
  - GUI option to evaluate general expressions on points and lines
  - Set colorbar min and max limits
  - Postprocessing plots show a title describing the plot
- New models and examples
- Solver, core, and grid generation fixes and enhancements


2015-08-30 version 1.3
----------------------
- Improved 2D geometry engine (especially boundary assignment
  and treatment of multiple geometry objects)
- Fractional step-theta scheme and HRZ mass lumping for
  time dependent problems
- Newton option for nonlinear stationary problems
- Optimized unstructured grid generation with better treatment
  of multiple subdomains
- Saving to m-script file
- Postprocessing and visualization export to Plotly (web)
- GUI option for model constants and expressions


2015-03-03 version 1.2
----------------------
- Full 3D support
- Implicit (distance/levelset function based) geometry modeling engine
- Unstructured grid generation
- Strong to weak equation formulation parser
- Custom equation(s) physics mode
- Extensibility, call to external grid, solver, and postprocessing supported
- Optimized FEM assembly and transformation Jacobian calculation routines
- Minor bug fixes


2014-11-27 version 1.1
----------------------
- Minor bug fixes


2014-05-17 version 1.0
----------------------
- Initial release


2013-07-25 version 0.9
----------------------
- Preliminary version
