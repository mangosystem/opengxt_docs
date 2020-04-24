.. _rasterclipbygeometry:

폴리곤으로 래스터 추출
====================================

설정한 폴리곤 지오메트리로 래스터를 추출합니다.

**Syntax**

RasterClipByGeometry (GridCoverage2D inputCoverage, Geometry cropShape) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 잘라낼 입력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - cropShape
     - 래스터를 잘라낼 폴리곤 또는 멀티폴리곤 지오메트리입니다.
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
     - 잘라낸 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - cropShape의 Geometry 타입은 Polygon 또는 MultiPolygon이어야 한다.

**Examples**
