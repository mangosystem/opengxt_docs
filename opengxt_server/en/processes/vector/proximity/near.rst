.. _near:

최근린 거리값 계산
==============================

입력 피처에서 가장 가까운 피처와의 거리와 관련 정보를 계산합니다.

**Syntax**

Near (SimpleFeatureCollection inputFeatures, SimpleFeatureCollection nearFeatures, String nearIdField, Double maximumDistance, DistanceUnit distanceUnit) : SimpleFeatureCollection

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

   * - nearFeatures
     - 최근린 거리값을 계산할 대상 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - nearIdField
     - 대상 레이어 각 피처의 ID 필드입니다. 설정하면 출력 레이어 필드 값이 계산됩니다.
     - String
     -
     -

   * - maximumDistance
     - 탐색할 최대 거리입니다.
     - Double
     - 0.0
     -

   * - distanceUnit
     - 탐색 거리의 단위입니다.
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
 - nearIdField 필드를 설정하지 않으면 피처의 내부 ID를 사용한다.
 - inputFeatures, nearFeatures는 포인트, 라인, 폴리곤 모두 가능하며 두 Geometry간의 최단거리를 계산한다.
 - maximumDistance가 설정되고 설정된 거리 안에 피처가 없는 경우 Null값이 입력된다.

**Examples**

입력 피처에서 가장 가까운 대상 레이어의 피처와 거리를 계산한 결과입니다.

  .. image:: images/near.png

