.. _fieldmaneuver:

야지기동 분석
====================================
적과 아군이 야지를 기동할 수 있는 능력을 경사율, 식생분포, 배수관계, 도심지 등의 자연 및 인공지형을 고려하여 분석
  - 기본 원리: 적합지 - 부적합지
  - 상세 원리: (경사도∩식생도) - (토질도+도심지+배수도)

**Syntax**

FieldManeuver(SimpleFeatureCollection slopeFeatures, SimpleFeatureCollection vegetationFeatures, SimpleFeatureCollection soilFeatures, SimpleFeatureCollection townFeatures, SimpleFeatureCollection drainageFeatures, Geometry maskArea) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - slopeFeatures
     - 경사도 적합지 레이어입니다. 기본값은 45% 이하입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - vegetationFeatures
     - 식생도 적합지 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - soilFeatures
     - 토질도 부적합지 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - townFeatures
     - 도심지 부적합지 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - drainageFeatures
     - 배수도 부적합지 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - maskArea
     - 분석 영역 폴리곤 지오메트리입니다. 최대 분석 범위는 10km * 10km를 넘을 수 없습니다.
     - Geometry
     -
     - ✓

**Process Outputs**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - result
     - 분석 결과입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - maskArea의 최대 분석 범위는 10km * 10km를 넘을 수 없습니다.
