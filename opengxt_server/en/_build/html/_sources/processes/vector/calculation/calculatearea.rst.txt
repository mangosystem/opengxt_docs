.. _calculatearea:

Calculate Area or Perimeter
===========================

Calculates feature's area or perimeter.

**Syntax**

CalculateArea (SimpleFeatureCollection inputFeatures, String areaField, AreaUnit areaUnit, String perimeterField, DistanceUnit perimeterUnit) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input polygon features to be calculated.
     - SimpleFeatureCollection
     - 
     - ✓

   * - areaField
     - Area field that will be calculated. geom_area is a default.
     - String
     - geom_area
     - 

   * - areaUnit
     - The output area unit.
     - AreaUnit
     - Default
     - 

   * - perimeterField
     - Perimeter field that will be calculated.
     - String
     - 
     - 

   * - perimeterUnit
     - The output perimeter unit.
     - DistanceUnit
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
     - Output features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 - areaUnit: Default(Default), SquareMeters, SquareKilometers, SquareFeet, SquareYards, SquareMiles, Hectare, Acre
 - perimeterUnit: Default(Default), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles

**Examples**

