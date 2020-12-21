.. _regularpoints:

격자 포인트 생성
=======================================

공간 범위와 영역 폴리곤 원본 내에 포함된 격자 포인트를 생성합니다.

**Syntax**

RegularPoints (ReferencedEnvelope extent, SimpleFeatureCollection boundsSource, SizeUnit unit, Double width, Double height) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - extent
     - 포인트가 생성될 공간 범위입니다.
     - ReferencedEnvelope
     -
     - ✓

   * - boundsSource
     - 포인트를 생성할 영역 레이어입니다. 해당 영역과 교차하는 포인트만 반환합니다.
     - SimpleFeatureCollection
     -
     -

   * - unit
     - 포인트 너비 또는 높이의 단위입니다. Count(기본값), Distance(포인트 생성 범위 좌표계의 단위를 따름).
     - SizeUnit
     - 
     - Count

   * - width
     - 포인트가 생성될 가로 방향의 거리 간격 또는 개수입니다.
     - Double
     -
     - ✓

   * - height
     - 포인트가 생성될 세로 방향의 거리 간격 또는 개수입니다.
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
     - 출력 포인트 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - unit: Count(기본값), Distance(extent 좌표계의 단위를 따름).
 - boundsSource 파라미터를 설정한 경우 boundsSource와 Intersect되는 포인트만 생성한다.


**Examples**

폴리곤 레이어 영역을 extent와 boundsSource로 설정하고 가로, 세로 1,500 미터(extent의 좌표 단위)의 격자 포인트를 생성한 예입니다.

  .. image:: images/regularpoints.png
