.. _polygonsalonglines:

라인을 따라 일정 간격의 폴리곤 생성
============================================================

라인을 따라 일정 거리 간격과 폭을 이용하여 폴리곤을 생성합니다.

**Syntax**

PolygonsAlongLines (SimpleFeatureCollection lineFeatures, Expression distance, Expression width, Double quadrantSegments) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - lineFeatures
     - 폴리곤 생성의 기준이 되는 참조할 라인 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - distance
     - 거리를 나타내는 숫자, 필드 또는 표현식입니다. 예) 1000 또는 [field] 또는 [field] * 0.5 등...
     - Expression
     -
     - ✓

   * - width
     - 폭을 나타내는 숫자, 필드 또는 표현식입니다. 예) 1000 또는 [field] 또는 [field] * 0.5 등...
     - Expression
     -
     - ✓

   * - quadrantSegments
     - 병합 여부를 나타내는 마지막 세그먼트 길이 팩터입니다. 이 값은 0(기본값, 병합하지 않음)에서 1까지의 실수 값이어야 합니다.
     - Double
     - 0.0
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
     - 출력 레이어이빈다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - lineFeatures 파라미터는 라인 또는 폴리곤 레이어 이어야 한다.
 - distance, width 파라미터는 필드 또는 Function Expression 수식을 사용할 수 있다.
 - distance, width 파라미터의 거리 단위는 lineFeatures의 좌표계 단위를 사용한다.


**Examples**
