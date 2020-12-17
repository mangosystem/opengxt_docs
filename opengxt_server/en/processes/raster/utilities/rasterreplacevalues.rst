.. _rasterreplacevalues:

래스터 셀값 대체
=================

래스터의 사용자가 지정한 영역내의 셀값을 설정한 값으로 대체합니다.

**Syntax**

RasterReplaceValues (GridCoverage2D inputCoverage, Geometry region, Double replaceValue) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 셀값을 대체할 입력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - region
     - 셀 값을 대체할 폴리곤 또는 멀티폴리곤 지오메트리 영역입니다.
     - Geometry
     -
     - ✓

   * - replaceValue
     - 셀값을 대체할 숫자 값입니다.
     - Double
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
     - 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - MultiPoint, LineString(MultiLineString), Polygon(MultiPolygon)을 지원한다.


**Examples**

  .. image:: images/rasterreplacevalues.png
