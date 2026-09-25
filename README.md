# Computational Optics: Generation of a 3D Quartic Optical Potential

Numerical simulation developed as part of my **BSc thesis at the Photonics Laboratory, ETH Zurich**.

## Overview

The goal of this project was to investigate the generation of a **three-dimensional quartic optical potential** using the high-numerical-aperture (high-NA) focusing of a structured laser beam.

The proposed optical field is constructed from a superposition of **radially and azimuthally polarized beam components**. When tightly focused by a high-NA optical system, the resulting vectorial electromagnetic field can produce an intensity distribution corresponding to the desired quartic potential.

Because high-NA focusing requires a fully vectorial treatment of the electromagnetic field, the focal field was studied numerically. The simulation was used to determine suitable optical parameters for the experimental setup and to investigate whether a quartic potential could be realized.

The numerical results demonstrate that, for an appropriate choice of parameters, the proposed optical configuration can theoretically generate the desired quartic potential.

## Numerical Model

The simulation consists of the following main steps:

1. Construction of the structured input beam from orthogonal Hermite–Gaussian modes.
2. Transformation of the input field into radial and azimuthal polarization components.
3. Vectorial propagation through a high-NA optical system.
4. Numerical evaluation of the focal electric-field components

$$
E_x(x,y,z), \qquad E_y(x,y,z), \qquad E_z(x,y,z)
$$

5. Calculation and analysis of the resulting intensity distribution

$$
I(x,y,z) \propto |E_x|^2 + |E_y|^2 + |E_z|^2
$$

The focal field is obtained by numerically evaluating the vectorial focusing integral over the angular spectrum of the incident field.

## Implementation

The simulation is implemented in Python using:

- **NumPy** for numerical calculations and complex-valued electromagnetic fields
- **Matplotlib** for visualization
- **Jupyter Notebook** for numerical analysis and documentation

The main notebook is:

`quartic_beam_simulation.ipynb`

It contains the complete workflow from the construction of the input field to the numerical high-NA focusing calculation and visualization of the focal-field distribution.

## Background

This work was carried out as part of my Bachelor thesis in the **Photonics Laboratory at ETH Zurich,  February–June 2023**.

The broader objective of the thesis was to design an optical setup capable of generating and characterizing a three-dimensional quartic potential. The numerical simulations provided a theoretical basis for selecting the experimental parameters and demonstrated the feasibility of the proposed optical configuration.

## Author

**Gian Lampert**  
ETH Zurich
