.. _calculatelength:

길이 계산
===============

입력 레이어에 길이 필드를 추가한 후 길이를 계산합니다.

**Syntax**

CalculateLength (SimpleFeatureCollection inputFeatures, String lengthField, DistanceUnit lengthUnit) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 길이를 계산할 라인 또는 폴리곤 레이어.
     - SimpleFeatureCollection
     -
     - ✓

   * - lengthField
     - 계산될 길이 필드. geom_len 이 기본값 입니다.
     - String
     - geom_len
     -

   * - lengthUnit
     - 계산될 길이의 단위입니다.
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
     - 출력 레이어.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - lengthUnit: Default(기본값), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles
 - inputFeatures 파라미터는 폴리곤 또는 라인 피처 타입이어야 한다.
 - 길이(둘레) 계산값은 inputFeatures의 좌표계 단위를 따른다.


**Examples**
