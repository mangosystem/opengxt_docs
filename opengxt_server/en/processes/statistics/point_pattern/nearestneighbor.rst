.. _nearestneighbor:

Nearest Neighbor Index
======================

Calculates a nearest neighbor index based on the average distance from each feature to its nearest neighboring feature.

**Syntax**

NearestNeighborIndex (SimpleFeatureCollection inputFeatures, DistanceMethod distanceMethod, Double area) : NearestNeighborResult

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

   * - distanceMethod
     - Specifies how distances are calculated from each feature to neighboring features: Euclidean(default) or Manhattan.
     - DistanceMethod
     - Euclidean
     - 

   * - area
     - A numeric value representing the study area.
     - Double
     - 0.0
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
     - Result Nearest Neighbor Index.
     - NearestNeighborResult
     - 
     - ✓

**Constraints**

 - distanceMethod: Euclidean(Default), Manhattan

**Examples**

