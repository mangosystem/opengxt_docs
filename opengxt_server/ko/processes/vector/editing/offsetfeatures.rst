.. _offsetfeatures:

피처 위치 변경
========================

X, Y 값을 사용하여 피처의 위치를 변경합니다.

**Syntax**

OffsetFeatures (SimpleFeatureCollection inputFeatures, Expression offsetX, Expression offsetY) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 변환할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - offsetX
     - X축 이동 거리입니다.
     - Expression
     - 0.0
     - ✓

   * - offsetY
     - Y축 이동 거리입니다.
     - Expression
     - 0.0
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
     - 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - 원본 위치를 기준으로 offsetX 값이 양수이면 우, 음수이면 좌로 이동하고, offsetY 값이 양수이면 상, 음수이면 하로 이동한다.

**Examples**
