.. _variablebuffer:

가변 버퍼
===============

선을 따라 각 정점에서 가변  버퍼를 생성합니다.

**Syntax**

VariableBuffer (SimpleFeatureCollection lineFeatures, Expression startDistance, Expression endDistance, DistanceUnit distanceUnit) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - lineFeatures
     - 버퍼를 적용할 입력 라인 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - startDistance
     - 라인 시작점에서의 버퍼 거리 또는 표현식입니다. 예) 0.0 또는 [field] 또는 [field] * 0.5 등...
     - Expression
     -
     - ✓

   * - endDistance
     - 라인 끝점에서의 버퍼 거리 또는 표현식입니다. 예) 1000 또는 [field] 또는 [field] * 0.5 등...
     - Expression
     -
     - ✓

   * - distanceUnit
     - 거리 단위입니다.
     - DistanceUnit
     - Default
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
     - 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - distanceUnit: Default(기본값), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles
 - inputFeatures는 라인 타입이어야 한다.
 - distance expression은 숫자, 숫자가 리턴되는 `함수식 <http://docs.geoserver.org/stable/en/user/filter/function_reference.html>`_ 모두 가능하다.
 - GeoServer 2.17.x(GeoTools 23.x) 이상의 버전만 지원합니다.


**Examples**

startDistance 0, endDistance 1000 미터 버퍼값을 준 결과입니다.

  .. image:: images/variablebuffer.png
