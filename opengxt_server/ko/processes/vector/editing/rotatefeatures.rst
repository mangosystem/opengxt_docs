.. _rotatefeatures:

피처 회전
===============

앵커 포인트 및 각도 (도 단위)를 사용하여 피쳐를 회전합니다.

**Syntax**

RotateFeatures (SimpleFeatureCollection inputFeatures, Point anchor, Expression angle) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 회전할 입력 레이어입니다.
     - SimpleFeatureCollection
     - 
     - ✓

   * - anchor
     - 피처 레이어를 회전시킬 피벗 포인트입니다. 기본값은 입력 피처 레이어 범위의 중심점입니다.
     - Point
     - 
     - 

   * - angle
     - 도 단위의 회전 각도입니다.
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
     - 회전한 출력 레이어입니다.
     - SimpleFeatureCollection
     - 
     - ✓

**Constraints**

  - anchor 파라미터는 Point 지오메트리 유형이다.
  - angle 파라미터는 도 단위의 회전 각도이며 Expression 표현식을 사용하여 각도를 정의할 수 있다.

**Examples**

폴리곤의 Centroid를 기준으로 45도 회전한 결과입니다.

  .. image:: images/rotatefeatures.png

