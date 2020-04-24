.. _polargridsfromfeatures:

피처 레이어 방사형 그리드
==========================================

피처 레이어의 중심으로부터 여러 개의 반경을 이용한 방사형 그리드를 생성합니다.

**Syntax**

PolarGridsFromFeatures (SimpleFeatureCollection origin, String radius, DistanceUnit radiusUnit, RadialType radialType, Integer sides) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - origin
     - 방사형 그리드의 중심점입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - radius
     - 쉼표로 구분된 반경값(단위: 입력 레이어 좌표계 기준) 목록입니다 : 예) 200, 300, 400, 500.
     - String
     -
     - ✓

   * - radiusUnit
     - 반경의 거리 단위입니다.
     - DistanceUnit
     - Default
     -

   * - radialType
     - 방사 유형입니다:  Polar(기본값), Base.
     - RadialType
     - Polar
     -

   * - sides
     - 면의 개수. 기본값은 8입니다.
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
     - 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - radiusUnit: Default(기본값), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles
 - radialType: Base, Polar(기본값)
 - 출력 레이어의 각 셀에는 angle, radius 값이 계산된다.
 - sides 파라미터의 기본값(8)을 사용하는 경우 azimuth 필드가 추가되고 NE, N, NW, W, SW, S, SE, E 등의 방향값이 계산된다.


**Examples**
