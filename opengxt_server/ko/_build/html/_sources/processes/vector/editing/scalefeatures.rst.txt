.. _scalefeatures:

피처 크기 변경
========================

x, y 축척값을 사용하여 피쳐의 크기를 변경합니다.

**Syntax**

ScaleFeatures (SimpleFeatureCollection inputFeatures, Expression scaleX, Expression scaleY, Point anchor) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 크기를 조절할 입력 레이어입니다.
     - SimpleFeatureCollection
     - 
     - ✓

   * - scaleX
     - X 방향의 피처의 지오메트리 크기에 대한 축척값입니다. 반드시 0보다 커야 하며, 1.0은 원본 값과 동일합니다.
     - Expression
     - 0.0
     - ✓

   * - scaleY
     - Y 방향의 피처의 지오메트리 크기에 대한 축척값입니다. 반드시 0보다 커야 하며, 1.0은 원본 값과 동일합니다.
     - Expression
     - 0.0
     - ✓

   * - anchor
     - 크기 조절시 사용되는 기준 포인트입니다. 기본값은 입력 피처 레이어 범위의 중심점입니다.
     - Point
     - 
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
     - 크기를 조절한 출력 레이어입니다.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

 

**Examples**

