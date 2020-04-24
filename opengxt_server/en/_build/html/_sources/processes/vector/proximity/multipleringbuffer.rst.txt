.. _multipleringbuffer:

Multiple Ring Buffer
====================

Creates a new features of buffer features using a set of buffer distances.

**Syntax**

MultipleRingBuffer (SimpleFeatureCollection inputFeatures, String distances, DistanceUnit distanceUnit, Boolean outsideOnly, Boolean dissolve) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input point, line, or polygon features to be buffered.
     - SimpleFeatureCollection
     - 
     - ✓

   * - distances
     - The comma separated list of buffer distances.
     - String
     - 
     - ✓

   * - distanceUnit
     - The desired linear unit.
     - DistanceUnit
     - Default
     - 

   * - outsideOnly
     - The area inside of the input polygon features will excluded from the resulting buffer.
     - Boolean
     - true
     - 

   * - dissolve
     - Determines if buffers will be dissolved to resemble rings around the input features.
     - Boolean
     - false
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
     - The output multiple buffers.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 - distanceUnit: Default(Default), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles

**Examples**

