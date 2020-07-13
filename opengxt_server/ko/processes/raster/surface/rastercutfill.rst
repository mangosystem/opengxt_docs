.. _rastercutfill:

성절토량 계산
====================================

DEM과 관심영역의 기준 높이를 이용하여 절성토량을 계산합니다.

**Syntax**

RasterCutFill(GridCoverage2D inputDEM, Geometry cropShape, Double baseHeight): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - DEM 등 입력 지형 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - cropShape
     - 지형 래스터 레이어를 잘라낼 폴리곤 또는 멀티폴리곤 지오메트리입니다.
     - Geometry
     -
     - ✓

   * - baseHeight
     - 잘라낼 영역 지오메트리의 기준 높이입니다. 기본값은 -9999이며, 기본값을 사용하는 경우 영역에 포함되는 입력 래스터 레이어의 평균값을 기준 높이값으로 사용합니다.
     - Double
     - -9999
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
     - 절성토량이 계산된 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - cropShape의 Geometry 타입은 Polygon 또는 MultiPolygon이어야 한다.
 - 기본값은 -9999이며, 기본값을 사용하는 경우 영역에 포함되는 입력 래스터 레이어의 평균값을 기준 높이값으로 사용합니다.

**Examples**
