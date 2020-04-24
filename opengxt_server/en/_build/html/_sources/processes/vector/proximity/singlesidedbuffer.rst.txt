.. _singlesidedbuffer:

Single-Sided Buffer Features
============================

Buffers a features using a certain distance expression.

**Syntax**

SingleSidedBuffer (SimpleFeatureCollection inputFeatures, Expression distance, DistanceUnit distanceUnit, Integer quadrantSegments) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - Line features to be buffered.
     - SimpleFeatureCollection
     - 
     - ✓

   * - distance
     - The distance expression used to create distance. Positive for the right side, negative for the left side. ex) 1000 or [field] or [field] * 0.5 etc...
     - Expression
     - 
     - ✓

   * - distanceUnit
     - The desired linear unit.
     - DistanceUnit
     - Default
     - 

   * - quadrantSegments
     - the number of line segments used to represent a quadrant of a circle.
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

 - distanceUnit: Default(Default), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles

**Examples**

