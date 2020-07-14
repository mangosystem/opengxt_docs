.. _wedgebuffer:

웨지(Wedge) 버퍼
====================================

방위각, 웨지각, 반경(값, 필드, 거리값 표현식)을 이용하여 포인트 레이어의 웨지 버퍼를 생성합니다.

**Syntax**

WedgeBuffer (SimpleFeatureCollection pointFeatures, Expression azimuth, Expression wedgeAngle, Expression innerRadius, Expression outerRadius, DistanceUnit radiusUnit) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - pointFeatures
     - 입력 포인트 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - azimuth
     - 방위각 (나침반 방향) 표현식입니다. 예) 45 또는 [field] 또는 [field] * 0.5 등 ...
     - Expression
     -
     - ✓

   * - wedgeAngle
     - 쐐기 각도 표현식입니다. 예) 45 또는 [field] 또는 [field] * 0.5 등 ...
     - Expression
     -
     - ✓

   * - innerRadius
     - 내부 반경 표현식입니다. 예) 25 또는 [field] 또는 [field] * 0.5 등...
     - Expression
     -
     -

   * - outerRadius
     - 외부 반경 표현식입니다. 예) 100 또는 [field] 또는 [field] * 0.5 등...
     - Expression
     -
     - ✓

   * - radiusUnit
     - 반경 단위입니다.
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

 - radiusUnit: Default(기본값), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles
 - pointFeatures 는 포인트 타입이어야 한다.
 - azimuth, wedgeAngle, innerRadius, outerRadius expression은 숫자, 숫자가 리턴되는 함수 식 모두 가능하다.
 - innerRadius, outerRadius 파라미터 값은 비교하여 값이 큰 쪽을 outerRadius값으로 사용하며, 둘 중 하나는 0보다 큰 값이어야 한다.
 - 각 파라미터의 값은 다음을 말한다.

  .. image:: images/wedge_parameters.png


**Examples**

포인트 레이어의 속성을 이용하여 Wedge 버퍼를 수행한 결과입니다.

  .. image:: images/wedgebuffer.png
