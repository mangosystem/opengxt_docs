.. _rastersurfacearea:

표면적 계산
====================================

DEM 등 지형 래스터 레이어를 이용하여 표고값을 고려한 표면적을 계산합니다.

**Syntax**

RasterSurfaceArea(GridCoverage2D inputCoverage, Geometry cropShape): SimpleFeatureCollection

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
     - 표면적을 계산할 폴리곤 또는 멀티폴리곤입니다.
     - Geometry
     -
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
     - 평면 및 표면적이 계산된 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - cropShape의 Geometry 타입은 Polygon 또는 MultiPolygon이어야 한다.
 - 출력 레이어는 area(평면 면적), surface(표면적) 필드를 포함한다.
