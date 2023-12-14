.. _cover:

엄폐 분석
====================================
직사화기로부터 보호되고, 간접 화력으로부터 부분적으로 보호되는 지역을 지형의 경사율, 식생의 분포, 토질 및 배수관계 등을 고려하여 분석
  - 기본 원리: 적합지 - 부적합지
  - 상세 원리: (경사도+식생도(산림)+토질도) - (도심지+배수도)

**Syntax**

Cover(SimpleFeatureCollection slopeFeatures, SimpleFeatureCollection forestFeatures, SimpleFeatureCollection soilFeatures, SimpleFeatureCollection townFeatures, SimpleFeatureCollection drainageFeatures, Geometry maskArea): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - slopeFeatures
     - 경사도 적합지 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - forestFeatures
     - 식생도(산림) 적합지 레이어입니다.
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
