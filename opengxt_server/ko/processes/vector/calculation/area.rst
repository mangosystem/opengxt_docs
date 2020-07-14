.. _area:

면적 계산
===============

폴리곤 피처 각각의 면적 합을 계산합니다.

**Syntax**

SumAreas (SimpleFeatureCollection inputFeatures, Filter filter, AreaUnit areaUnit) : Double

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 폴리곤 레이어.
     - SimpleFeatureCollection
     -
     - ✓

   * - filter
     - 필터 표현식
     - Filter
     -
     -

   * - areaUnit
     - 출력 면적 단위.
     - AreaUnit
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
     - 레이어의 면적
     - Double
     -
     - ✓

**Constraints**

 - areaUnit: Default(기본값), SquareMeters, SquareKilometers, SquareFeet, SquareYards, SquareMiles, Hectare, Acre
 - 폴리곤 레이어와 필터를 이용하여 피처의 Geometry 면적 합을 반환한다.

**Examples**

폴리곤 레이어의 모든 피처의 면적 합을 Double 값으로 반환합니다.