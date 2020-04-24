.. _calculatelength:

Calculate Length
================

Adds the length field to the input features and calculates feature's length.

**Syntax**

CalculateLength (SimpleFeatureCollection inputFeatures, String lengthField, DistanceUnit lengthUnit) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input line or polygon features to be calculated.
     - SimpleFeatureCollection
     - 
     - ✓

   * - lengthField
     - Length field that will be calculated. geom_len is a default.
     - String
     - geom_len
     - 

   * - lengthUnit
     - Length unit that will be applied.
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

 - lengthUnit: Default(Default), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles

**Examples**

