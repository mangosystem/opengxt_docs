.. _rasterreproject:

Reproject
=========

Reprojects the raster dataset from one projection to another.

**Syntax**

RasterReproject (GridCoverage2D inputCoverage, CoordinateReferenceSystem targetCRS, ResampleType resamplingType, Double cellSize, CoordinateReferenceSystem forcedCRS) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - The raster dataset for which you want to change the spatial resolution.
     - GridCoverage2D
     - 
     - ✓

   * - targetCRS
     - Target coordinate reference system to use for reprojection.
     - CoordinateReferenceSystem
     - 
     - ✓

   * - resamplingType
     - The resampling algorithm to be used. NEAREST(default), BILINEAR, BICUBIC.
     - ResampleType
     - NEAREST
     - 

   * - cellSize
     - The cell size for the output raster.
     - Double
     - 0.0
     - 

   * - forcedCRS
     - Coordinate reference system to use for input raster dataset.
     - CoordinateReferenceSystem
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
     - Output raster.
     - GridCoverage2D
     - 
     - ✓

**Constraints**

 - resamplingType: NEAREST(Default), BILINEAR, BICUBIC

**Examples**

