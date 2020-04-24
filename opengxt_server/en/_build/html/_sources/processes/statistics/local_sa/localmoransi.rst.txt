.. _localmoransi:

Local Moran's I
===============

Given a set of weighted features, identifies statistically significant hot spots, cold spots, and spatial outliers using the Anselin Local Moran's I statistic.

**Syntax**

LocalMoransI (SimpleFeatureCollection inputFeatures, String inputField, SpatialConcept spatialConcept, DistanceMethod distanceMethod, StandardizationMethod standardization, Double searchDistance) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The features for which cluster/outlier analysis will be performed.
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

