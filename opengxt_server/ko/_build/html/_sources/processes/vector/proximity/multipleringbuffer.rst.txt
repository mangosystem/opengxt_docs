.. _multipleringbuffer:

다중 링 버퍼
=====================

거리값, 필드값 또는 필드의 조합을 이용한 여러 개의 거리 표현식들을 정의하여  다중 링 버퍼를 생성합니다.

**Syntax**

MultipleRingBuffer (SimpleFeatureCollection inputFeatures, String distances, DistanceUnit distanceUnit, Boolean outsideOnly, Boolean dissolve) : SimpleFeatureCollection

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

   * - distances
     - 쉼표로 구분된 버퍼 거리 목록입니다.
     - String
     -
     - ✓

   * - distanceUnit
     - 거리 단위입니다.
     - DistanceUnit
     - Default
     -

   * - outsideOnly
     - 입력 폴리곤 피처 내부 영역이 결과 버퍼에서 제외할 지 여부를 설정합니다.
     - Boolean
     - true
     -

   * - dissolve
     - 버퍼한 피처가 중첩되는 경우 디졸브를 수행할 지 여부를 설정합니다.
     - Boolean
     - false
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
 - inputFeatures는 포인트, 라인, 폴리곤 모두 가능하다.
 - Dissolve 파라미터 값이 True인 경우 inputFeatures의 속성값은 무시되고 거리값만, False인 경우 inputFeatures의 속성값을 유지한다.


**Examples**

시군구청 포인트를 250,500,750,1000,1250,1500미터 간격으로 Buffer 분석을 처리한 결과입니다.

  .. image:: images/multipleringbuffer.png
