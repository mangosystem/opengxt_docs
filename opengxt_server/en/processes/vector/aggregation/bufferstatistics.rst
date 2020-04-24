.. _bufferstatistics:

Point Aggregation using Buffer
==============================

Calculates count or statistics for the points inside each feature's buffer zone.

**Syntax**

BufferPointStatistics (SimpleFeatureCollection inputFeatures, Double distance, DistanceUnit distanceUnit, SimpleFeatureCollection pointFeatures, String countField, String statisticsFields) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - Input features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - distance
     - Search distance.
     - Double
     - 0.0
     - ✓

   * - distanceUnit
     - The desired linear unit.
     - DistanceUnit
     - Default
     - 

   * - pointFeatures
     - Point features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - countField
     - Count field.
     - String
     - count
     - 

   * - statisticsFields
     - Statistics Fields: Function.PropertyName(First, Last, Sum, Mean, Min, Max, Std, Count)
     - String
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
     - Output Features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 - distanceUnit: Default(Default), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles

**Examples**

