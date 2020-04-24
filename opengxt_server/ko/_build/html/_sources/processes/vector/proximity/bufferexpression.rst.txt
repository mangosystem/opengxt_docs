.. _bufferexpression:

버퍼
======

거리값, 필드값 또는 필드의 조합을 이용한 거리 표현식을 정의하여  버퍼를 생성합니다.

**Syntax**

BufferFeatures (SimpleFeatureCollection inputFeatures, Expression distance, DistanceUnit distanceUnit, Integer quadrantSegments) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 버퍼를 적용할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - distance
     - 거리를 설정하기 위해 사용되는 거리 표현식입니다. 예) 1000 또는 [field] 또는 [field] * 0.5 등...
     - Expression
     -
     - ✓

   * - distanceUnit
     - 거리 단위입니다.
     - DistanceUnit
     - Default
     -

   * - quadrantSegments
     - 원의 사분면을 나타내는데 사용되는 세그먼트의 개수입니다.
     - Integer
     - 8
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
     - 출력 레이어.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - distanceUnit: Default(기본값), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles
 - inputFeatures는 포인트, 라인, 폴리곤 모두 가능하다.
 - distance expression은 숫자, 숫자가 리턴되는 `함수식 <http://docs.geoserver.org/stable/en/user/filter/function_reference.html>`_ 모두 가능하다.


**Examples**
