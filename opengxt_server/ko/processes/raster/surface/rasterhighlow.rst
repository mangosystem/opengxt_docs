.. _rasterhighlow:

최고 최저점 찾기
===========================

지형 래스터에서 설정한 영역에서의 최고/최저점을 찾아 포인트 피처로 변환합니다.

**Syntax**

RasterHighLowPoints (GridCoverage2D inputCoverage, Integer bandIndex, Geometry cropShape, HighLowType valueType) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 최고/최저 지점을 추출할 입력 래스터 레이어입니다.
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

   * - valueType
     - 추출할 값 유형입니다. Both(최고/최저 모두), High(최고점만, 기본값), Low(최저점만).
     - HighLowType
     - High
     - ✓

**Process Outputs**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - result
     - 최고/최저 지점을 담고 있는 출력 포인트 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - valueType: Both, High(기본값), Low
 - cropShape 파라미터는 반드시 Polygon 또는 MultiPolygon이어야 한다.
 - valueType 파라미터는 Both, High, Low 값을 사용하며, Null이면 High 값을 적용한다.

**Examples**

  .. image:: images/rasterhighlow.png
