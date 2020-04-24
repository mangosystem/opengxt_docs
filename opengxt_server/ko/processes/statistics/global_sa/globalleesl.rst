.. _globalleesl:

Lee의 전역적 L 통계량
==========================================

Lee의 전역적 L 통계량을 계산합니다.

**Syntax**

GlobalLeesL (SimpleFeatureCollection inputFeatures, String xField, String yField, SpatialConcept spatialConcept, DistanceMethod distanceMethod, StandardizationMethod standardization, Double searchDistance, Boolean selfNeighbors) : LeesLProcessResult

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
     - LeesLProcessResult
     -
     - ✓

**Constraints**

 - spatialConcept: InverseDistance(기본값), InverseDistanceSquared, FixedDistance, ZoneOfIndifference, KNearestNeighbors, ContiguityEdgesNodes, ContiguityEdgesOnly, ContiguityNodesOnly, WeightsFromFile
 - distanceMethod: Euclidean(기본값), Manhattan
 - standardization: None(기본값), Row
 - Output은 XML로 반환한다.

**Examples**

  .. code-block::

    <?xml version="1.0" encoding="utf-8"?>
    <GlobalLeesL>
      <TypeName>korea_sgg</TypeName>
      <PropertyName>a + b</PropertyName>
      <Observed_Index>0.42206509</Observed_Index>
      <Expected_Index>0.090566</Expected_Index>
      <Variance>0</Variance>
      <Z_Score>0</Z_Score>
      <P_Value>1</P_Value>
      <Conceptualization>0.42206509</Conceptualization>
      <DistanceMethod>Euclidean</DistanceMethod>
      <RowStandardization>Row</RowStandardization>
      <DistanceThreshold>0</DistanceThreshold>
    </GlobalLeesL>
