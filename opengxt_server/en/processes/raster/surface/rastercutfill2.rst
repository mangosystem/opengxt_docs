.. _rastercutfill2:

성절토량 계산 2
====================================

성절토 전과 후의 DEM을 이용하여 절성토량을 계산합니다.

**Syntax**

RasterCutFill2 (GridCoverage2D beforeCoverage, GridCoverage2D afterCoverage, Geometry cropShape): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - beforeCoverage
     - 성절토 전 입력 지형 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - afterCoverage
     - 성절토 후 지형 래스터 레이어입니다.
     - GridCoverage2D
     - 
     - ✓

   * - cropShape
     - 지형 래스터 레이어를 잘라낼 폴리곤 또는 멀티폴리곤 지오메트리입니다.
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
     - 성절토량이 계산된 출력 레이어입니다. 지오메트리가 포함되어 있지 않습니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - cropShape의 Geometry 타입은 Polygon 또는 MultiPolygon이어야 한다.
 - 절성토량이 계산된 출력 레이어는 category, count, area, volume 필드를 포함한다.
 - category 필드의 값은 -1(성토, Fill), 0(변화없음), 1(절토, Cut) 값으로 구분한다.
 - count 필드는 폴리곤을 구성하는 래스터 셀의 갯수이다.
 - area 필드는 폴리곤을 구성하는 래스터 셀의 면적 합니다.
 - volume 필드는 폴리곤을 구성하는 래스터의 절/성토량이다.
 - area와 volume의 단위는 입력 래스터 데이터의 좌표계를 따르며, 입력 래스터 데이터는 미터 단위의 좌표계를 사용해야 올바른 절/성토량이 계산된다.

**Examples**

DEM으로부터 특정 영역(버퍼영역)의 절성토량을 계산한 출력 레이어의 예입니다.
category, count, area, volume 속성정보를 포함합니다.

  .. image:: images/rastercutfill-table.png