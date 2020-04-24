.. _spatialclumpmap:

Spatial Clump Map 생성
============================================================

포인트 피처와 반경 표현식을 이용하여 Spatial Clump Map을 생성합니다.

**Syntax**

SpatialClumpMap (SimpleFeatureCollection inputFeatures, Expression radius, DistanceUnit radiusUnit, Integer quadrantSegments) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - radius
     - 거리를 생성할 반경 표현식입니다. 예) 1000 또는 [field] 또는 [field] * 0.5 등...
     - Expression
     -
     - ✓

   * - radiusUnit
     - 반경 단위입니다.
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

 - radiusUnit: Default(기본값), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles
 - quatrantSegments 파라미터의 기본값은 8이다.

**Examples**
