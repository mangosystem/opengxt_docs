.. _calculatearea:

면적 또는 둘레 계산
=================================

폴리곤 레이어의 면적 및 둘레를 계산합니다.

**Syntax**

CalculateArea (SimpleFeatureCollection inputFeatures, String areaField, AreaUnit areaUnit, String perimeterField, DistanceUnit perimeterUnit) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 면적을 계산할 폴리곤 레이어
     - SimpleFeatureCollection
     -
     - ✓

   * - areaField
     - 면적이 계산될 필드. geom_area 가 기본값 입니다.
     - String
     - geom_area
     -

   * - areaUnit
     - 출력 면적 단위.
     - AreaUnit
     - Default
     -

   * - perimeterField
     - 둘레가 계산될 필드입니다.
     - String
     -
     -

   * - perimeterUnit
     - 출력 둘레 단위.
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

 - areaUnit: Default(기본값), SquareMeters, SquareKilometers, SquareFeet, SquareYards, SquareMiles, Hectare, Acre
 - perimeterUnit: Default(기본값), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles
 - inputFeatures는 반드시 폴리곤 이어야 한다.
 - 면적, 둘레의 계산값은 inputFeatures의 좌표계 단위를 따른다.


**Examples**
