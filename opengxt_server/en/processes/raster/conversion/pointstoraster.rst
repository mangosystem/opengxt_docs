.. _pointstoraster:

Points To Raster
================

Converts point features to a raster dataset.

**Syntax**

PointsToRaster (SimpleFeatureCollection inputFeatures, String inputField, PointAssignmentType cellAssignment, Double cellSize, ReferencedEnvelope extent) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The point or multipoint input feature dataset to be converted to a raster.
     - SimpleFeatureCollection
     - 
     - ✓

   * - inputField
     - The field used to assign values to the output raster.
     - String
     - 
     - ✓

   * - cellAssignment
     - The method to determine how the cell will be assigned a value when more than one feature falls within a cell. MostFrequent(Default), Sum, Mean, StandardDeviation, Maximum, Minimum, Range, Count
     - PointAssignmentType
     - MostFrequent
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
     - The output raster.
     - GridCoverage2D
     - 
     - ✓

**Constraints**

 - cellAssignment: MostFrequent(Default), Sum, Mean, StandardDeviation, Maximum, Minimum, Range, Count

**Examples**

