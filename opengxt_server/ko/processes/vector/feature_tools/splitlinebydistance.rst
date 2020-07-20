.. _splitlinebydistance:

거리값 또는 표현식으로 라인 분할
======================================================

설정한 거리값(값, 필드, 표현식)에 따라 분할한 라인 피처를 생성합니다.

**Syntax**

SplitLineByDistance (SimpleFeatureCollection lineFeatures, Expression distance) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - lineFeatures
     - 분할할 라인 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - distance
     - 개수를 표현하는 숫자, 필드 또는 계산식을 설정합니다. 예) 10 또는 필드 또는 geomLength( [geom] ) / 10.
     - Expression
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
     - 분할한 출력 라인 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures 파라미터는 라인 또는 폴리곤 레이어 이어야 한다.
 - distance 파라미터는 필드 또는 Function Expression 수식을 사용할 수 있다.

**Examples**

폴리곤 피처의 boundary를 100미터 간격의 라인으로 분할한 결과입니다.

  .. image:: images/splitlinebydistance.png

