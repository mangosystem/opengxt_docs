.. _globalleesl:

Global Lee's L
==============

Measures spatial autocorrelation based on feature locations and attribute values using the Global Lee's L statistic.

**Syntax**

GlobalLeesL (SimpleFeatureCollection inputFeatures, String xField, String yField, SpatialConcept spatialConcept, DistanceMethod distanceMethod, StandardizationMethod standardization, Double searchDistance, Boolean selfNeighbors) : LeesLProcessResult

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The features for which spatial autocorrelation will be calculated.
     - SimpleFeatureCollection
     - 
     - ✓

   * - xField
     - The numeric field used in assessing spatial autocorrelation.
     - String
     - 
     - ✓

   * - yField
     - The numeric field used in assessing spatial autocorrelation.
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
     - Result Document.
     - LeesLProcessResult
     - 
     - ✓

**Constraints**

 - spatialConcept: InverseDistance(Default), InverseDistanceSquared, FixedDistance, ZoneOfIndifference, KNearestNeighbors, ContiguityEdgesNodes, ContiguityEdgesOnly, ContiguityNodesOnly, WeightsFromFile
 - distanceMethod: Euclidean(Default), Manhattan
 - standardization: None(Default), Row

**Examples**

