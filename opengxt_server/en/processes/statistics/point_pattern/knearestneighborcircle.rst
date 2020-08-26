.. _knearestneighborcircle:

K-Nearest Neighbor Circle
=================================

Creates a k-nearest neighbor circle polygons from two features.

**Syntax**

KNearestNeighborCircle (SimpleFeatureCollection inputFeatures, SimpleFeatureCollection nearFeatures, Integer neighbor, Double maximumDistance, DistanceUnit distanceUnit): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The input features that can be point, line, polygon. The nearest distance is calculated using the centroid of the input feature.
     - SimpleFeatureCollection
     -
     - ✓

   * - nearFeatures
     - The near features that can be point, line, polygon.
     - SimpleFeatureCollection
     -
     - ✓

   * - neighbor
     - The number of neighbors to be considered.
     - Integer
     - 1
     - 

   * - maximumDistance
     - The maximum distance to search for near features. The default is 0. If the distance is 0, the nearest feature is searched regardless of distance.
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
     - The output polygon features.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - distanceUnit: Default(Default), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles

**Examples**

