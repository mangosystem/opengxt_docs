.. _densify:

라인의 버텍스 추가
==============================

지오메트리에 포함된 선분을 따라 허용오차 간격의 버텍스를 삽입합니다.

**Syntax**

Densify (SimpleFeatureCollection inputFeatures, Expression tolerance) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 버텍스를 추가할 라인 또는 폴리곤 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - tolerance
     - 버텍스를 추가할 거리 간격 표현식입니다 예) 10.0 또는 필터 표현식.
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
     - 버텍스를 추가한 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - tolerance 파라미터는 수 또는 수식을 사용할 수 있다.

**Examples**
