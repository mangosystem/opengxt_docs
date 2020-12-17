.. _knearestneighborcircle:

K-최근린 이웃 원 생성
=================================

두 레이어간의 k-최근린 이웃에 대한 원 폴리곤을 생성합니다.

**Syntax**

KNearestNeighborCircle (SimpleFeatureCollection inputFeatures, SimpleFeatureCollection nearFeatures, Integer neighbor, Double maximumDistance, DistanceUnit distanceUnit): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 포인트, 라인, 폴리곤 유형의 입력 레이어입니다. 거리는 입력 피처의 중심점을 이용하여 계산합니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - nearFeatures
     - 포인트, 라인, 폴리곤 유형의 거리를 계산할 이웃 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - neighbor
     - 원을 생성할 최근린 이웃 수를 설정합니다.
     - Integer
     - 1
     - 

   * - maximumDistance
     - 최근린 이웃을 탐색할 최대 거리입니다. 기본값은 0이며 만약 거리 기본값이 0인 경우, 최근린 피처는 거리에 상관 없이 탐색합니다.
     - Double
     - 0.0
     -

   * - distanceUnit
     - 탐색 거리의 단위입니다.
     - DistanceUnit
     - Default
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
     - 최근린 이웃 원 출력 폴리곤 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - distanceUnit: Default(Default), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles
 - maximumDistance 파라미터의 기본값은 0이며 만약 거리 기본값이 0인 경우, 최근린 피처는 거리에 상관 없이 탐색한다.

**Examples**

Neighbor 파라미터를 3으로 설정하고 실행한 K-Nearest Neighbor Circle을 실행한 결과입니다.

  .. image:: images/knearestneighborcircle.png
