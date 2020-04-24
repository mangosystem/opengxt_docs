.. _centralfeature:

Central Feature
===============

Identifies the most centrally located feature in a point, line, or polygon feature class.

**Syntax**

CentralFeature (SimpleFeatureCollection inputFeatures, DistanceMethod distanceMethod, String weightField, String selfPotentialWeightField, String caseField) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - The features containing a distribution of features from which to identify the most centrally located feature.
     - SimpleFeatureCollection
     - 
     - ✓

   * - distanceMethod
     - Specifies how distances are calculated from each feature to neighboring features
     - DistanceMethod
     - Euclidean
     - 

   * - weightField
     - The numeric field used to weight distances in the origin-destination distance matrix.
     - String
     - 
     - 

   * - selfPotentialWeightField
     - The field representing self-potential. the distance or weight between a feature and itself.
     - String
     - 
     - 

   * - caseField
     - The field used to group features for separate central feature computations.
     - String
     - 
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
     - A point features that will contain the features representing the centers of the input features.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 - distanceMethod: Euclidean(Default), Manhattan

**Examples**

