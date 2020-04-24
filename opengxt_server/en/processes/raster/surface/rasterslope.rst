.. _rasterslope:

Slope
=====

Identifies the slope (gradient, or rate of maximum change in z-value) from each cell of a raster surface.

**Syntax**

RasterSlope (GridCoverage2D inputCoverage, SlopeType slopeType, Double zFactor) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - The input surface raster.
     - GridCoverage2D
     - 
     - ✓

   * - slopeType
     - Determines the measurement units of the output slope data. Degree(default), Percentrise.
     - SlopeType
     - Degree
     - 

   * - zFactor
     - The number of ground x,y units in one surface z unit.
     - Double
     - 1.0
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

 - slopeType: Degree(Default), Percentrise

**Examples**

