.. _rasterrotate:

Rotate
======

Turns a raster dataset around the specified pivot point by the angle specified angle in degrees.

**Syntax**

RasterRotate (GridCoverage2D inputCoverage, Point anchorPoint, Double angle, ResampleType interpolation) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - The input raster to be converted.
     - GridCoverage2D
     - 
     - ✓

   * - anchorPoint
     - The pivot point around which to rotate the raster. The default is the lower left corner of the input raster dataset.
     - Point
     - 
     - 

   * - angle
     - The angle in degrees to rotate the raster.
     - Double
     - 0.0
     - ✓

   * - interpolation
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
     - Output Raster.
     - GridCoverage2D
     - 
     - ✓

**Constraints**

 - interpolation: NEAREST(Default), BILINEAR, BICUBIC

**Examples**

