.. _idw:

IDW Interpolation
=================

Interpolates a raster surface from points using an inverse distance weighted (IDW) technique.

**Syntax**

IDW (SimpleFeatureCollection inputFeatures, String inputField, Double power, RadiusType radiusType, Integer numberOfPoints, Double distance, Double cellSize, ReferencedEnvelope extent) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input point features for which to calculate the interpolation.
     - SimpleFeatureCollection
     - 
     - ✓

   * - inputField
     - The field that holds a height or magnitude value for each point.
     - String
     - 
     - ✓

   * - power
     - The exponent(default 2.0) of distance.
     - Double
     - 2.0
     - 

   * - radiusType
     - The search radius type. Variable(Default), Fixed.
     - RadiusType
     - Variable
     - 

   * - numberOfPoints
     - The number of points is an integer value specifying the number of nearest input sample points to be used to perform the interpolation.
     - Integer
     - 12
     - 

   * - distance
     - The distance specifies the distance, in map units, by which to limit the search for the nearest input sample points.
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
     - The output IDW raster.
     - GridCoverage2D
     - 
     - ✓

**Constraints**

 - radiusType: Variable(Default), Fixed

**Examples**

