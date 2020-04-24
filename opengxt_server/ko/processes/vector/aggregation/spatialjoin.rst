.. _spatialjoin:

공간 기반 조인
========================

공간관계를 이용하여 두 레이어를 조인합니다.

**Syntax**

SpatialJoin (SimpleFeatureCollection inputFeatures, SimpleFeatureCollection joinFeatures, SpatialJoinType joinType, Double searchRadius, DistanceUnit radiusUnit) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 입력 레이어.
     - SimpleFeatureCollection
     -
     - ✓

   * - joinFeatures
     - 조인 대상 레이어.
     - SimpleFeatureCollection
     -
     - ✓

   * - joinType
     - 조인 유형입니다. KeepAllRecord(기본값) 또는 OnlyMatchingRecord.
     - SpatialJoinType
     - KeepAllRecord
     -

   * - searchRadius
     - 탐색 반경.
     - Double
     - 0.0
     -

   * - radiusUnit
     - 탐색 반경값의 거리 단위입니다.
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

 - joinType: KeepAllRecord(기본값), OnlyMatchingRecord
 - radiusUnit: Default(기본값), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles
 - joinType 파라미터의 값이 KeepAllRecord인 경우 공간 조인이 수행되지 않은 inputFeatures의 모든 피처를 포함하여 반환한다.
 - searchRadius 파라미터 값이 주어지면 searchRadius 내에 포함되는 피처와 조인한다.


**Examples**
