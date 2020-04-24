.. _fishnetsize:

크기로 격자 그리드 생성
=======================================

가로, 세로 크기로 격자 그리드를 생성합니다.

**Syntax**

FishnetSize (ReferencedEnvelope extent, SimpleFeatureCollection boundsSource, Boolean boundaryInside, Double width, Double height) : SimpleFeatureCollection

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
     - 격자를 생성할 영역 레이어입니다. 해당 영역과 교차하는 격자만 반환합니다.
     - SimpleFeatureCollection
     -
     -

   * - boundaryInside
     - 격자 생성 영역 레이어가 폴리곤일 경우 폴리곤 내부에만 격자를 생성하는 옵션입니다.
     - Boolean
     - false
     -

   * - width
     - 격자의 너비를 설정합니다.
     - Double
     -
     - ✓

   * - height
     - 격자의 높이를 설정합니다.
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
     - 출력 격자 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - boundsSource 파라미터를 설정한 경우 boundsSource와 Intersect되는 격자만 생성한다.
 - boundsSource 파라미터를 설정하고 boundaryInside 파라미터가 True인 경우 boundsSource 내부에 포함되는 격자만 생성한다.


**Examples**
