.. _near:

Calculate Nearest Neighbor Distance
===================================

Calculates distance and additional proximity information between the input features and the closest feature in another features.

**Syntax**

Near (SimpleFeatureCollection inputFeatures, SimpleFeatureCollection nearFeatures, String nearIdField, Double maximumDistance, DistanceUnit distanceUnit) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - Input Features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - nearFeatures
     - Near Features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - nearIdField
     - Near ID field.
     - String
     - 
     - 

   * - maximumDistance
     - Maximum distance.
     - Double
     - 0.0
     - 

   * - distanceUnit
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

 - distanceUnit: Default(Default), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles

**Examples**

