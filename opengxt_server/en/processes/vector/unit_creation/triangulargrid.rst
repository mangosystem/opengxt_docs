.. _triangulargrid:

삼각형 그리드 생성
==============================

크기와 범위를 설정하여 삼각형 그리드를 생성합니다.

**Syntax**

TriangularGrid (ReferencedEnvelope extent, SimpleFeatureCollection boundsSource, Double size, HexagonOrientation orientation) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - extent
     - 그리드가 생성될 공간 범위입니다.
     - ReferencedEnvelope
     -
     - ✓

   * - boundsSource
     - 그리드를 생성할 영역 레이어입니다. 해당 영역과 교차하는 그리드만 반환합니다.
     - SimpleFeatureCollection
     -
     -

   * - size
     - 삼각형의 크기를 설정합니다.
     - Double
     -
     - ✓

   * - orientation
     - 삼각형 방향을 설정합니다. FLAT(기본값), ANGLED.
     - HexagonOrientation
     - FLAT
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
     - 출력 삼각형 그리드 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - orientation: ANGLED, FLAT(기본값)
 - boundsSource 파라미터를 설정한 경우 boundsSource와 Intersect되는 삼각형만 생성한다.

**Examples**

폴리곤 레이어 영역을 extent와 boundsSource로 설정하고 반경 2500(extent의 좌표 단위)의 Triangular 격자를 생성한 예입니다.

  .. image:: images/triangulargrid.png
