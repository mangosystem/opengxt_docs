.. _focallq:

지역 특화도(Focal LQ) 분석
=========================================================

피처 레이어의 두 필드값과 공간가중치를 계산하여 Focal Location Quotients (Focal LQ, 지역 특화도) 분석을 수행합니다.

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
     - Focal LQ를 계산할 2개 이상의 숫자 필드를 가진 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - xField
     - X 값 필드입니다.
     - Expression
     -
     - ✓

   * - yField
     - Y 값 필드 입니다.
     - Expression
     -
     - ✓

   * - spatialConcept
     - 피처 간의 공간 관계를 어떻게 정의할 것인지를 설정합니다.
     - SpatialConcept
     - FixedDistance
     -

   * - distanceMethod
     - 각각의 피처와 이웃 피처의 거리를 계산하는데 사용되는 알고리즘 입니다: Euclidean(기본값) 또는 Manhattan.
     - DistanceMethod
     - Euclidean
     -

   * - searchDistance
     - 최대 탐색 반경입니다. 탐색 반경이 0인 경우 최근린 이웃 지수를 활용하여 내부적으로 적절한 탐색 반경을 계산해서 사용합니다.
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
     - 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - spatialConcept: InverseDistance, InverseDistanceSquared, FixedDistance(기본값), ZoneOfIndifference, KNearestNeighbors, ContiguityEdgesNodes, ContiguityEdgesOnly, ContiguityNodesOnly, WeightsFromFile
 - distanceMethod: Euclidean(기본값), Manhattan
 - Output 레이어의 필드는 flq, flqd, fz 값을 반환한다.

**Examples**

전국 시군구의 두 필드를 이용하여 지역 특화도를 분석 후 시각화한 결과는 다음과 같습니다.

  .. image:: images/focallq.png
