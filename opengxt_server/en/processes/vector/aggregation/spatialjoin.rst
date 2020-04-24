.. _spatialjoin:

Join Features By Spatial
========================

Joins attributes from one feature to another based on the spatial relationship.

**Syntax**

SpatialJoin (SimpleFeatureCollection inputFeatures, SimpleFeatureCollection joinFeatures, SpatialJoinType joinType, Double searchRadius, DistanceUnit radiusUnit) : SimpleFeatureCollection

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

   * - joinFeatures
     - Join features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - joinType
     - Join Type. KeepAllRecord(default) or OnlyMatchingRecord.
     - SpatialJoinType
     - KeepAllRecord
     - 

   * - searchRadius
     - Search Radius.
     - Double
     - 0.0
     - 

   * - radiusUnit
     - The desired linear unit.
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
     - Output Features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 - joinType: KeepAllRecord(Default), OnlyMatchingRecord
 - radiusUnit: Default(Default), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles

**Examples**

