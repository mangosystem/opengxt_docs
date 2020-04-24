.. _localleesl:

Lee의 국지적 L 통계량
==========================================

Lee의 국지적 L 통계량을 계산합니다.

**Syntax**

LocalLeesL (SimpleFeatureCollection inputFeatures, String xField, String yField, SpatialConcept spatialConcept, DistanceMethod distanceMethod, StandardizationMethod standardization, Double searchDistance, Boolean selfNeighbors) : SimpleFeatureCollection

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

   * - xField
     - 수치형 입력 변수 X 필드 변수를 설정합니다.
     - String
     -
     - ✓

   * - yField
     - 수치형 입력 변수 Y 필드 변수를 설정합니다.
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

   * - selfNeighbors
     - 분석 대상 피처 자체를 자신의 이웃 리스트에 포함할 것인지 여부를 선택합니다.
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
     - 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - spatialConcept: InverseDistance(기본값), InverseDistanceSquared, FixedDistance, ZoneOfIndifference, KNearestNeighbors, ContiguityEdgesNodes, ContiguityEdgesOnly, ContiguityNodesOnly, WeightsFromFile
 - distanceMethod: Euclidean(기본값), Manhattan
 - standardization: None(기본값), Row
 - Output 레이어는 inputFeatures의 모든 필드를 포함해서 LLlIndex, LLlZScore, LLlPValue 필드가 추가된다.

**Examples**
