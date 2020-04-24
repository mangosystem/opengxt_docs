.. _trimline:

Dangle 라인 제거
====================================

라인의 교차점을 지나 특정 거리만큼 연장된 라인 부분(Dangles)을 제거합니다.

**Syntax**

TrimLine (SimpleFeatureCollection lineFeatures, Double dangleLength, Boolean deleteShort) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - lineFeatures
     - Dangle 라인을 제거할 입력 라인 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - dangleLength
     - 지정된 Dangle 길이보다 짧고 두 끝점 (Dangle)에서 다른 라인에 닿지 않는 라인은 잘립니다.
     - Double
     - 0.0
     - ✓

   * - deleteShort
     - Dangle 길이보다 짧고 독립적으로 떨어져 있는 라인 세그먼트를 삭제할지 여부를 설정합니다. 기본값은 아니오(False)입니다.
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
     - Dangle 라인을 제거한 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - lineFeatures 레이어는 라인 타입 이어야 한다.
 - deleteShort 파라미터가 True이고, 시작/끝점 모두 다른 라인과 교차하지 않는 독립적인 라인이 dangleLength 길이보다 작으면 삭제됩니다.


**Examples**
