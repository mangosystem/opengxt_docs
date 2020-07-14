.. _nearestneighborcount:

반경 내 피처 수 계산
====================================

입력 피처에서 설정한 탐색 반경에 포함되는 피처의 수를 계산합니다.

**Syntax**

NearestNeighborCount (SimpleFeatureCollection inputFeatures, String countField, SimpleFeatureCollection nearFeatures, Double searchRadius, DistanceUnit radiusUnit) : SimpleFeatureCollection

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

   * - countField
     - 반경 내 피처 수가 저장될 필드입니다. 기본값은 count 입니다
     - String
     - count
     -

   * - nearFeatures
     - 반경 내 피처 수를 계산할 대상 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - searchRadius
     - 탐색 반경입니다. 탐색 반경은 반드시 0보다 커야 합니다.
     - Double
     - 0.0
     - ✓

   * - radiusUnit
     - 탐색 반경의 거리 단위입니다.
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
 - inputFeatures, nearFeatures는 포인트, 라인, 폴리곤 모두 가능하며 두 Geometry간의 최단거리를 계산한다.
 - searchRadius 파라미터의 단위는 inputFeatures 거리단위를 사용하고 0보다 커야 한다.


**Examples**

주요도로에서 500미터 반경 내의 포인트 수를 graduated symbol로 표현한 결과입니다.

  .. image:: images/nearestneighborcount.png
