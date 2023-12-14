.. _penetration:

공중침투 분석
====================================
공중침투 낙하지점 최적지 분석은 낙하산 착륙을 위한 경사와 식생, 공중 및 지상장애물 등을 고려한 분석이며, 적의 종심작전부대 강하 및 공중강습작전을 위한 계획수립이나 낙하산에 의한 적 공중 침투 낙하지점을 판단하는데 활용
 - 기본 원리: 적합지 - 부적합지
 - 상세원리: (경사도∩식생도∩식생도(산림)) - (도심지+배수도+송전선(버퍼))

**Syntax**

Penetration(SimpleFeatureCollection slopeFeatures, SimpleFeatureCollection vegetationFeatures, SimpleFeatureCollection forestFeatures, SimpleFeatureCollection townFeatures, SimpleFeatureCollection drainageFeatures, SimpleFeatureCollection transFeatures, Double distance, DistanceUnit distanceUnit,  Geometry maskArea): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - slopeFeatures
     - 경사도 적합지 레이어입니다. 기본값은 20% 이하입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - vegetationFeatures
     - 식생도 적합지 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - forestFeatures
     - 식생도(산림) 적합지 레이어입니다.
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

   * - transFeatures
     - 송전선 부적합지 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - distance
     - 송전선 버퍼 거리입니다. 기본값은 100m입니다.
     - Double
     - 100
     - ✓

   * - distanceUnit
     - 송전선 버퍼 거리 단위입니다. 기본값은 Meter입니다.
     - DistanceUnit
     - Meters
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
