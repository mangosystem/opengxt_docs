.. _histogramgridcoverage:

래스터 히스토그램
===========================

래스터 레이어 전체 또는 사용자가 설정한 영역에 대한 셀값별 빈도수를 계산합니다.

**Syntax**

HistogramGridCoverage (GridCoverage2D inputCoverage, Integer bandIndex, Geometry cropShape) : HistogramProcessResult

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 히스토그램을 계산할 입력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - bandIndex
     - 0 부터 시작하는 밴드 인덱스, 기본 인덱스는 0입니다.
     - Integer
     - 0
     -

   * - cropShape
     - 폴리곤 또는 멀티폴리곤 유형의 잘라낼 영역을 설정합니다.
     - Geometry
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
     - 출력 히스토그램
     - HistogramProcessResult
     -
     - ✓

**Constraints**

 - cropShape의 Geometry 타입은 Polygon 또는 MultiPolygon이어야 한다.
 - bandIndex는 zero-base이며, 0이 기본값이다.
 - Output은 XML로 반환한다.


**Examples**

  .. code-block::

    <?xml version="1.0" encoding="utf-8"?>
    <Histogram>
      <TypeName>landuse</TypeName>
      <PropertyName>Value</PropertyName>
    <Area>25498176.913556</Area>
    <CellSize>30.0</CellSize>
      <HistogramItem>
        <Value>1</Value>
        <Frequency>876</Frequency>
      </HistogramItem>
      <HistogramItem>
        <Value>2</Value>
        <Frequency>543</Frequency>
      </HistogramItem>
      <HistogramItem>
        <Value>3</Value>
        <Frequency>292</Frequency>
      </HistogramItem>
      <HistogramItem>
        <Value>4</Value>
        <Frequency>1345</Frequency>
      </HistogramItem>
      ...
    </Histogram>
