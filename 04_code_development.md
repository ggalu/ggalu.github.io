---
layout: page
title: Code Development
navigation: 5
---

# Code Development

1. **[voxelDVC - global Digital Volume Correlation (click)](#voxeldvc)**


***
{: style="border-top: 0.3rem solid #606c76"}

## voxelDVC

![voxelDVC logo](/images/code/voxeldvc_logo.svg){: width="600" }

voxelDVC is a GPU-accelerated program for Digital Volume Correlation (DVC). Given a reference volume and a deformed volume of the same specimen, recorded by X-ray computed tomography before and after loading, it computes the displacement field on a structured finite-element mesh of eight-node hexahedra. The solver is matrix-free, so its memory use grows only with the number of voxels, and high-resolution volumes can be processed on a single GPU.

The source code is available under the MIT licence at **[github.com/ggalu/voxelDVC](https://github.com/ggalu/voxelDVC){:target="_blank"}**.

### associated publication:

|  |  |
|----------------------- |--------------------------------|
| ![SoftwareX](/images/code/softwarex_cover.jpg){: width="120" style="min-width: 120px" } | G.C. Ganzenmüller, voxelDVC: a matrix-free, GPU-native global Digital Volume Correlation solver for high-resolution computed tomography, *SoftwareX* 36, 103111, **2026**. DOI: **[10.1016/j.softx.2026.103111](https://doi.org/10.1016/j.softx.2026.103111){:target="_blank"}**. |

