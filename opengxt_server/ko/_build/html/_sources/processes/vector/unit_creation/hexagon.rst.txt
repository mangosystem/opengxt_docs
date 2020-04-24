.. _hexagon:

헥사곤 그리드 생성
==============================

크기와 범위를 설정하여 헥사곤 그리드를 생성합니다.

**Syntax**

Hexagon (ReferencedEnvelope extent, SimpleFeatureCollection boundsSource, Double sideLen, HexagonOrientation orientation) : SimpleFeatureCollection

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

   * - sideLen
     - 헥사곤 격자의 크기로 중심점에서 꼭지점까지의 거리입니다. 단위는 입력 레이어의 좌표계 단위입니다.
     - Double
     -
     - ✓

   * - orientation
     - 헥사곤 방향을 설정합니다. FLAT(기본값), ANGLED.
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
     - 출력 헥사곤 그리드 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - orientation: ANGLED, FLAT(기본값)
 - boundsSource 파라미터를 설정한 경우 boundsSource와 Intersect되는 헥사곤만 생성한다.
 - sideLen 파라미터는 헥사곤 중심에서 모서리와의 거리를 말한다.


**Examples**
