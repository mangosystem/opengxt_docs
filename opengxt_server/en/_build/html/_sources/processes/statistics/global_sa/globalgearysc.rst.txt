.. _globalgearysc:

Global Geary's c
================

Measures spatial autocorrelation based on feature locations and attribute values using the Global Geary's c statistic.

**Syntax**

GlobalGearysC (SimpleFeatureCollection inputFeatures, String inputField, SpatialConcept spatialConcept, DistanceMethod distanceMethod, StandardizationMethod standardization, Double searchDistance) : GearysCProcessResult

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

   * - inputField
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
     - GearysCProcessResult
     - 
     - ✓

**Constraints**

 - spatialConcept: InverseDistance(Default), InverseDistanceSquared, FixedDistance, ZoneOfIndifference, KNearestNeighbors, ContiguityEdgesNodes, ContiguityEdgesOnly, ContiguityNodesOnly, WeightsFromFile
 - distanceMethod: Euclidean(Default), Manhattan
 - standardization: None(Default), Row

**Examples**

