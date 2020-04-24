.. _spatialclumpmap:

Spatial Clump Map
=================

Creates a spatial clump map using point features and distance expression.

**Syntax**

SpatialClumpMap (SimpleFeatureCollection inputFeatures, Expression radius, DistanceUnit radiusUnit, Integer quadrantSegments) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - Input features to be processed.
     - SimpleFeatureCollection
     - 
     - ✓

   * - radius
     - The radius expression used to create distance. ex) 1000 or [field] or [field] * 0.5 etc...
     - Expression
     - 
     - ✓

   * - radiusUnit
     - The desired linear unit.
     - DistanceUnit
     - Default
     - 

   * - quadrantSegments
     - The number of line segments used to represent a quadrant of a circle.
     - Integer
     - 8
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

 - radiusUnit: Default(Default), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles

**Examples**

