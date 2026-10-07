---
layout: page
title: Code Development
navigation: 5
---

# Code Development

1. **[voxelDVC - global Digital Volume Correlation (click)](#voxeldvc)**
2. **[sigmaSPH - Smoothed Particle Hydrodynamics for fluids and solids (click)](#sigmasph)**


***
{: style="border-top: 0.3rem solid #606c76"}

## voxelDVC

![voxelDVC logo](/images/code/voxeldvc_logo.svg){: width="600" }

voxelDVC is a GPU-accelerated program for Digital Volume Correlation (DVC). Given a reference volume and a deformed volume of the same specimen, recorded by X-ray computed tomography before and after loading, it computes the displacement field on a structured finite-element mesh of eight-node hexahedra. The solver is matrix-free, so its memory use grows only with the number of voxels, and high-resolution volumes can be processed on a single GPU.

The source code is available under the MIT licence at **[github.com/ggalu/voxelDVC](https://github.com/ggalu/voxelDVC){:target="_blank"}**.

### associated publication:

|  |  |
|----------------------- |--------------------------------|
| ![SoftwareX](/images/code/softwarex_cover.jpg){: width="120" style="min-width: 120px" } | G.C. Ganzenmüller, voxelDVC: a matrix-free, GPU-native global Digital Volume Correlation solver for high-resolution computed tomography, *SoftwareX*, accepted for publication, **2026**. |


***
{: style="border-top: 0.3rem solid #606c76"}

## sigmaSPH

| ![sigmaSPH hypervelocity impact](/images/code/sigmasph_hvi.jpg){: width="1024" } |
|:--:|
| *Debris cloud of an aluminium sphere (Al 2017-T4) that has perforated a 2 mm aluminium disc at 6.7 km/s, computed with sigmaSPH.* |

sigmaSPH is a GPU-accelerated Smoothed Particle Hydrodynamics (SPH) code written in [Taichi](https://taichi-lang.org/){:target="_blank"}. It simulates weakly compressible fluids and elastic-plastic solids at large deformation, in 3D, 2D plane strain and 2D axisymmetry. For solids, it provides equations of state for shock loading, J2 and Johnson-Cook plasticity, several damage models, and particle shifting in an arbitrary Lagrangian-Eulerian (ALE) formulation, which makes it suited to impact and fracture problems.

The source code is available under the MIT licence at **[github.com/ggalu/sigmaSPH](https://github.com/ggalu/sigmaSPH){:target="_blank"}**. Every release is archived on Zenodo, https://doi.org/10.5281/zenodo.23084820.

### associated publication:
- G.C. Ganzenmüller, Hourglass control for solid SPH-ALE: Stability and convergence under tensile loading, submitted to *Computer Methods in Applied Mechanics and Engineering*, **2026**. Preprint: **[SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=7560377){:target="_blank"}**.
