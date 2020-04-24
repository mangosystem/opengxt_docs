.. _statisticsgridcoverage:

래스터 요약 통계
===========================

래스터 레이어의 요약 통계(최소값, 최대값, 평균, 합, 분산, 표준편차, 범위 등)를 계산합니다.

**Syntax**

StatisticsGridCoverage (GridCoverage2D inputCoverage, Geometry cropShape, Integer bandIndex) : DataStatisticsResult

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 요약통계를 계산할 입력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - cropShape
     - 폴리곤 또는 멀티폴리곤 유형의 잘라낼 영역을 설정합니다.
     - Geometry
     -
     -

   * - bandIndex
     - 0 부터 시작하는 밴드 인덱스, 기본 인덱스는 0입니다.
     - Integer
     - 0
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
     - 요약통계 결과입니다.
     - DataStatisticsResult
     -
     - ✓

**Constraints**

 - cropShape이 Null이면 입력 래스터의 전체 셀을 대상으로 통계를 작성한다.
 - cropShape의 Geometry 타입은 Polygon 또는 MultiPolygon이어야 한다.
 - bandIndex는 zero-base이며, 0이 기본값이다.
 - Output은 XML로 반환한다.


**Examples**

  .. code-block::

    <?xml version="1.0" encoding="utf-8"?>
    <DataStatistics>
    <Item>
      <TypeName>dem</TypeName>
      <PropertyName>Value</PropertyName>
      <Count>678064</Count>
      <InvalidCount>0</InvalidCount>
      <Minimum>1.0</Minimum>
      <Maximum>754.0</Maximum>
      <Range>753.0</Range>
      <Ranges>1.0 - 754.0</Ranges>
      <Sum>4.2785658E7</Sum>
      <Mean>63.09973394841785</Mean>
      <Variance>7285.154424054373</Variance>
      <StandardDeviation>85.35311607700315</StandardDeviation>
      <CoefficientOfVariance>1.3526699834705607</CoefficientOfVariance>
      <NoData class="double">-9999</NoData>
    </Item>
    </DataStatistics>
