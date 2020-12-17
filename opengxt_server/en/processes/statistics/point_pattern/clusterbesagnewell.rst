.. _clusterbesagnewell:

공간 클러스터 탐색: Besag, Julian and Newell, James
====================================================================

Besag, Julian and Newell, James의 알고리즘을 이용한 공간 클러스터를 탐색합니다.

**Syntax**

ClusterBesagNewell (SimpleFeatureCollection popFeatures, Expression popField, SimpleFeatureCollection caseFeatures, Expression caseField, Integer neighbours, FitnessFunctionType functionType, Double threshold): SimpleFeatureCollection, GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - popFeatures
     - The features containing the population at risk.
     - SimpleFeatureCollection
     -
     - ✓

   * - popField
     - The feature attribute with the population at risk.
     - Expression
     - 
     - ✓

   * - caseFeatures
     - The features containing the incidents.
     - SimpleFeatureCollection
     -
     - ✓

   * - caseField
     - The feature attribute with the incidents.
     - Expression
     - 
     - ✓

   * - neighbours
     - The Number of neighbours to be considered. the default value is 10.
     - Integer
     - 10
     - 

   * - functionType
     - The type of fitness function to be used. Poisson(Default), Relative, RelativePercent
     - Expression
     - Poisson
     - 

   * - threshold
     - The significance threshold at which to accept the test.
     - Double
     - 0.01
     - 

**Process Outputs**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - resultCircles
     - Output significant circles.
     - SimpleFeatureCollection
     -
     - ✓

   * - resultDensity
     - Output density results.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - neighbours의 기본값은 10이다.
 - threshold의 기본값은 0.01이다.


**Examples**

  .. image:: images/clusterbesagnewell.png
