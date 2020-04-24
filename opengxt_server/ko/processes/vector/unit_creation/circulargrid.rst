.. _circulargrid:

원형 그리드 생성
===========================

원의 반경과 범위를 설정하여 원형 그리드를 생성합니다.

**Syntax**

CircularGrid (ReferencedEnvelope extent, SimpleFeatureCollection boundsSource, Double radius, CircularType circularType) : SimpleFeatureCollection

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
     - 그리드를 생성할 영역 레이어입니다. 해당 영역과 교차하는 원형 그리드만 반환합니다.
     - SimpleFeatureCollection
     -
     -

   * - radius
     - 원의 반경
     - Double
     -
     - ✓

   * - circularType
     - 원의 유형입니다: Grid(default), Hex.
     - CircularType
     - Grid
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
     - 출력 원형 그리드 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - circularType: Grid(기본값), Hex
 - boundsSource를 설정한 경우 boundsSource와 Intersect되는 원을 생성한다.
 - circularType이 Grid인 경우 격자형식의 원을, Hex인 경우 헥사곤 생성 규칙을 따른다.


**Examples**
