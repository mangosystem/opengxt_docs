.. _localsabinning:

격자 분석을 이용한 공간적 자기상관 분석
=============================================

설정된 격자 내에 입력 포인트의 개수(또는 가중치)를 계산 후 국지적 공간 자기상관 분석을 수행합니다.

**Syntax**

LocalSABinning (SimpleFeatureCollection features, Expression weight, BinningGridType gridType, ReferencedEnvelope extent, Double size, AutoCorrelationMethod saMethod, SpatialConcept spatialConcept, DistanceMethod distanceMethod, StandardizationMethod standardization, Double searchDistance): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - features
     - 통계량을 계산할 입력 포인트 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - weight
     - 가중치 값으로 사용될 숫자형 필드 또는 표현식입니다. 설정 시 이 값의 합이 각각의 격자에 계산됩니다.
     - Expression
     -
     - ✓

   * - gridType
     - 생성할 격자 유형입니다. Hexagon(기본값), Rectangle, Circle
     - BinningGridType
     - Hexagon
     - ✓

   * - extent
     - 격자 생성 범위입니다. 범위가 지정되지 않으면 입력 레이어의 범위와 좌표체계를 기본값으로 합니다.
     - ReferencedEnvelope
     -
     - ✓

   * - size
     - 생성할 격자의 크기 또는 반경입니다.
     - Double
     -
     - ✓

   * - saMethod
     - 공간 자기상관 기법입니다. MoranI(기본값, Anselin Local Moran's I), GetisOrdGiStar(Getis-Ord Gi*), GearyC(Geary's C), LeeS(Lee's S)
     - AutoCorrelationMethod
     - MoranI
     -

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

 - gridType: Hexagon(기본값), Rectangle, Circle
 - saMethod: MoranI(기본값, Anselin Local Moran's I), GetisOrdGiStar(Getis-Ord Gi*), GearyC(Geary's C), LeeS(Lee's S)
 - spatialConcept: InverseDistance(기본값), InverseDistanceSquared, FixedDistance, ZoneOfIndifference, KNearestNeighbors, ContiguityEdgesNodes, ContiguityEdgesOnly, ContiguityNodesOnly, WeightsFromFile
 - distanceMethod: Euclidean(기본값), Manhattan
 - standardization: None(기본값), Row
 - Output 레이어는 inputFeatures의 모든 필드를 포함해서 LMiIndex, LMiZScore, LMiPValue, LMizValue, LMiwzValue, COType 필드가 추가된다.

**Examples**

1km 간격의 헥사곤 격자를 생성하고 포인트 데이터를 집계한 후 분석한 결과입니다.

  .. image:: images/localsabinning-lisa.png
