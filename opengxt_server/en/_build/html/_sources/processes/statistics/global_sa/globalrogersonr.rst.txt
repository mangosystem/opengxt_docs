.. _globalrogersonr:

Global Rogerson's R
===================

Detect spatial clusters based on feature locations and attribute values using the Global Rogerson's R statistic.

**Syntax**

GlobalRogersonR (SimpleFeatureCollection inputFeatures, String xField, String yField, DistanceMethod distanceMethod, Double kappa) : RogersonRProcessResult

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

   * - distanceMethod
     - Specifies how distances are calculated from each feature to neighboring features.
     - DistanceMethod
     - Euclidean
     - 

   * - kappa
     - Measure of the importance of distance.
     - Double
     - 1.0
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
     - RogersonRProcessResult
     - 
     - ✓

**Constraints**

 - distanceMethod: Euclidean(Default), Manhattan

**Examples**

