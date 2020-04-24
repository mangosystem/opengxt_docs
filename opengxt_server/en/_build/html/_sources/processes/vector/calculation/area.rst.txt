.. _area:

Sum Polygon Feature's Area
==========================

Sum up the areas of all polygon features.

**Syntax**

SumAreas (SimpleFeatureCollection inputFeatures, Filter filter, AreaUnit areaUnit) : Double

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The polygon features to be calculated.
     - SimpleFeatureCollection
     - 
     - ✓

   * - filter
     - The filter to apply.
     - Filter
     - 
     - 

   * - areaUnit
     - The output area unit.
     - AreaUnit
     - Default
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
     - The area of features.
     - Double
     - 
     - ✓

**Constraints**

 - areaUnit: Default(Default), SquareMeters, SquareKilometers, SquareFeet, SquareYards, SquareMiles, Hectare, Acre

**Examples**

