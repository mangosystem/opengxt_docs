.. _kerneldensity:

Kernel Density
==============

Calculates a magnitude per unit area from point features using a kernel function to fit a smoothly tapered surface to each point.

**Syntax**

KernelDensity (SimpleFeatureCollection inputFeatures, KernelType kernelType, String populationField, Double searchRadius, Double cellSize, ReferencedEnvelope extent) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input point features for which to calculate the density.
     - SimpleFeatureCollection
     - 
     - ✓

   * - kernelType
     - Kernel functions: Binary, Cosine, Distance, Epanechnikov, Gaussian, InverseDistance, Quadratic(default), Quartic(biweight), Triangular, Triweight, Tricube
     - KernelType
     - Quadratic
     - 

   * - populationField
     - The field denoting population values for each feature.
     - String
     - 
     - 

   * - searchRadius
     - The search radius within which to calculate density.
     - Double
     - 0.0
     - 

   * - cellSize
     - The cell size for the output raster.
     - Double
     - 0.0
     - 

   * - extent
     - The extent for the output raster.
     - ReferencedEnvelope
     - 
     - 

**Process Outputs**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - result
     - The output kernel density raster.
     - GridCoverage2D
     - 
     - ✓

**Constraints**

 - kernelType: Binary, Cosine, Distance, Epanechnikov, Gaussian, InverseDistance, Quadratic(Default), Quartic, Triangular, Triweight, Tricube

**Examples**

