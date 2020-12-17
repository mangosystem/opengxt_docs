.. _clustergam:

공간 클러스터 탐색: Openshaw의 GAM
================================================

Openshaw의 Geographical Analysis Machine(GAM) 알고리즘을 이용한 공간 클러스터를 탐색합니다.

**Syntax**

ClusterGAM (SimpleFeatureCollection popFeatures, Expression popField, SimpleFeatureCollection caseFeatures, Expression caseField, Double minRadius, Double maxRadius, Double radiusIncrement, Double overlapRatio, FitnessFunctionType functionType, Double threshold): SimpleFeatureCollection, GridCoverage2D

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

   * - minRadius
     - The radius of the smallest circle to consider.
     - Double
     - 0
     - 

   * - maxRadius
     - The radius of the largest circle to consider.
     - Double
     - 0
     - 

   * - radiusIncrement
     - How much to change the size of the circles by. If radius increment is 0, the default value is minimum radius / 2.0.
     - Double
     - 0
     - 

   * - overlapRatio
     - How much should the circles overlap by (0 ~ 1). the default value is 0.5.
     - Double
     - 0.5
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

 - minRadius의 값이 0보다 작은 경우 popFeatures 레이어 범위의 1/150을 사용한다.
 - maxRadius의 값이 minRadius의 값보다 작은 경우 minRadius 값의 5배를 사용한다.
 - radiusIncrement의 값이 0보다 작으면 minRadius값의 1/2값을 사용한다.
 - overlapRatio는 0에서 1 사이의 값을 사용해야 하고, 기본값은 0.5이다.
 - threshold의 기본값은 0.01이다.


**Examples**

  .. image:: images/clustergam.png
