.. _pointsalonglines:

라인을 따라 일정 간격의 포인트 생성
============================================================

각각의 라인 피처별로 설정한 거리 간격으로 라인을 따라 포인트를 생성합니다.

**Syntax**

PointsAlongLines (SimpleFeatureCollection lineFeatures, Expression distance) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - lineFeatures
     - 포인트를 생성할 라인 또는 폴리곤 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - distance
     - 포인트를 생성할 일정 간격의 거리를 나타내는 숫자, 필드 또는 표현식입니다.
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
     - 출력 포인트 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures 파라미터는 라인 또는 폴리곤 레이어 이어야 한다.
 - distance 파라미터는 필드 또는 Function Expression 수식을 사용할 수 있다.


**Examples**
