.. _focallq:

Focal Location Quotients
========================

Calculates a Focal Location Quotients (Focal LQ).

**Syntax**

FocalLQ (SimpleFeatureCollection inputFeatures, Expression xField, Expression yField, SpatialConcept spatialConcept, DistanceMethod distanceMethod, Double searchDistance) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The features for which the focal LQ will be calculated.
     - SimpleFeatureCollection
     - 
     - ✓

   * - xField
     - X Value Field.
     - Expression
     - 
     - ✓

   * - yField
     - Y Value Field.
     - Expression
     - 
     - ✓

   * - spatialConcept
     - Specifies how spatial relationships among features are conceptualized.
     - SpatialConcept
     - FixedDistance
     - 

   * - distanceMethod
     - Specifies how distances are calculated from each feature to neighboring features.
     - DistanceMethod
     - Euclidean
     - 

   * - searchDistance
     - The maximum search distance.
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
     - Output features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 - spatialConcept: InverseDistance, InverseDistanceSquared, FixedDistance(Default), ZoneOfIndifference, KNearestNeighbors, ContiguityEdgesNodes, ContiguityEdgesOnly, ContiguityNodesOnly, WeightsFromFile
 - distanceMethod: Euclidean(Default), Manhattan

**Examples**

