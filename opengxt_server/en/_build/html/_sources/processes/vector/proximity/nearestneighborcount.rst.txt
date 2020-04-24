.. _nearestneighborcount:

Calculate Neighbors Count
=========================

Calculates features count between the input features and the closest feature in another features.

**Syntax**

NearestNeighborCount (SimpleFeatureCollection inputFeatures, String countField, SimpleFeatureCollection nearFeatures, Double searchRadius, DistanceUnit radiusUnit) : SimpleFeatureCollection

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

   * - countField
     - Count field. The default is count.
     - String
     - count
     - 

   * - nearFeatures
     - Near Features.
     - SimpleFeatureCollection
     - 
     - ✓

   * - searchRadius
     - Search radius. Search radius must be greater than 0.
     - Double
     - 0.0
     - ✓

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

 - radiusUnit: Default(Default), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles

**Examples**

