.. _extendline:

라인 세그먼트 연장
==============================

지정된 거리 내에서 첫 번째 교차하는 피쳐로 라인 세그먼트를 확장합니다.

**Syntax**

ExtendLine (SimpleFeatureCollection lineFeatures, Double length, Boolean extendTo) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - lineFeatures
     - 라인 세그먼트를 연장할 라인 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - length
     - 선분을 교차 피처까지 연장할 수 있는 최대 거리입니다.
     - Double
     - 0.0
     - ✓

   * - extendTo
     - 지정된 연장 길이 내에서 라인 세그먼트를 다른 연장된 라인 세그먼트로 연장할 수 있는지 여부를 설정합니다.
     - Boolean
     - true
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
     - 세그먼트를 연장한 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - lineFeatures 레이어는 라인 타입 이어야 한다.
 - length 파라미터는 라인의 세그먼트가 확장할 수 있는 최대 거리이며, lineFeatures의 거리 단위를 사용한다.
 - extendTo 파라미터가 True인 경우 모든 세그먼트가 length만큼 확장한 라인을 적용한다.


**Examples**
