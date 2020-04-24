.. _localleess:

Local Lee's S
=============

Calculate Local Lee's S values.

**Syntax**

LocalLeesS (SimpleFeatureCollection inputFeatures, String inputField, SpatialConcept spatialConcept, DistanceMethod distanceMethod, StandardizationMethod standardization, Double searchDistance, Boolean selfNeighbors) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The features for which analysis will be performed.
     - SimpleFeatureCollection
     - 
     - ✓

   * - inputField
     - The numeric field to be evaluated.
     - String
     - 
     - ✓

   * - spatialConcept
     - Specifies how spatial relationships among features are conceptualized.
     - SpatialConcept
     - InverseDistance
     - 

   * - distanceMethod
     - Specifies how distances are calculated from each feature to neighboring features.
     - DistanceMethod
     - Euclidean
     - 

   * - standardization
     - Row Standardization.
     - StandardizationMethod
     - None
     - 

   * - searchDistance
     - Specifies a cutoff distance for Inverse Distance and Fixed Distance options. 
     - Double
     - 0.0
     - 

   * - selfNeighbors
     - Includes itself in its own list of neighbors.
     - Boolean
     - true
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
     - The output features to receive the results fields.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 - spatialConcept: InverseDistance(Default), InverseDistanceSquared, FixedDistance, ZoneOfIndifference, KNearestNeighbors, ContiguityEdgesNodes, ContiguityEdgesOnly, ContiguityNodesOnly, WeightsFromFile
 - distanceMethod: Euclidean(Default), Manhattan
 - standardization: None(Default), Row

**Examples**

