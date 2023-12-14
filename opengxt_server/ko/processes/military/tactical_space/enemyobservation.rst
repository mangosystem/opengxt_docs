.. _enemyobservation:

적종팀 은거 및 관측 분석
====================================
적지종심작전부대가 적으로 부터의 관측회피를 위한 은거가 양호한 지역에서 최적의 관측효과를 얻을 수 있는 최적지를 분석하
 - 기본 원리: 적합지 - 부적합지
 - 상세 원리: (경사도∩식생도∩수송도) - (토질도+배수도(부적합지)) + 식생도(DMZ)

**Syntax**

EnemyObservation(SimpleFeatureCollection slopeFeatures, SimpleFeatureCollection forestFeatures, SimpleFeatureCollection soilFeatures, SimpleFeatureCollection townFeatures, SimpleFeatureCollection drainageFeatures, SimpleFeatureCollection dmzFeatures, Season season, Geometry maskArea): SimpleFeatureCollection

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

   * - dmzFeatures
     - 식생도(DMZ) 적합지 레이어입니다.
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
