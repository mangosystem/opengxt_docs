.. _localmoransi:

국지적 Moran I 통계량
=============================================

Anselin의 국지적 Moran I 통계량을 계산합니다.

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
     - 통계량을 계산할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - inputField
     - 수치형 입력 필드 변수를 설정합니다.
     - String
     -
     - ✓

   * - spatialConcept
     - 피처들 간에 공간 관계를 설정하는 방식을 선택합니다.
     - SpatialConcept
     - InverseDistance
     -

   * - distanceMethod
     - 분석 대상 피처로부터 이웃 피처까지의 거리를 계산하는 방법을 설정합니다.
     - DistanceMethod
     - Euclidean
     -

   * - standardization
     - 통계량 계산시 행 표준화 적용 여부를 설정합니다.
     - StandardizationMethod
     - None
     -

   * - searchDistance
     - 역거리 혹은 고정 거리 옵션 선택 시 기준 값을 지정합니다.
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

 - spatialConcept: InverseDistance(기본값), InverseDistanceSquared, FixedDistance, ZoneOfIndifference, KNearestNeighbors, ContiguityEdgesNodes, ContiguityEdgesOnly, ContiguityNodesOnly, WeightsFromFile
 - distanceMethod: Euclidean(기본값), Manhattan
 - standardization: None(기본값), Row
 - Output 레이어는 inputFeatures의 모든 필드를 포함해서 LMiIndex, LMiZScore, LMiPValue, LMizValue, LMiwzValue, COType 필드가 추가된다.

**Examples**
