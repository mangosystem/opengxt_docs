.. _rasterresample:

Resample
========

Changes the spatial resolution of raster and set rules for aggregating or interpolating values across the new pixel sizes.

**Syntax**

RasterResample (GridCoverage2D inputCoverage, Double cellSize, ResampleType resamplingType) : GridCoverage2D

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

   * - cellSize
     - The cell size of the new raster.
     - Double
     - 0.0
     - ✓

   * - resamplingType
     - The resampling algorithm to be used. NEAREST(default), BILINEAR, BICUBIC.
     - ResampleType
     - NEAREST
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

