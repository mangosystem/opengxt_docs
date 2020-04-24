.. _rasterhighlow:

Find Highest/Lowest Points
==========================

Finds the highest or lowest points for a surface raster.

**Syntax**

RasterHighLowPoints (GridCoverage2D inputCoverage, Integer bandIndex, Geometry cropShape, HighLowType valueType) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - The input raster to be processed.
     - GridCoverage2D
     - 
     - ✓

   * - bandIndex
     - The zero-based band index, default index is a 0.
     - Integer
     - 0
     - 

   * - cropShape
     - The Polygon or MultiPolygon to clip raster.
     - Geometry
     - 
     - 

   * - valueType
     - Value Type(Both, High, Low). Default is High.
     - HighLowType
     - High
     - ✓

**Process Outputs**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - result
     - Result Points.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 - valueType: Both, High(Default), Low

**Examples**

