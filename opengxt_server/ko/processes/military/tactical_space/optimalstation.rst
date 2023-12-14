.. _optimalstation:

주둔 최적지 분석
====================================
최적의 주둔지역을 토질, 경사율, 은폐율, 급수원과 배수관계, 주둔부대 수용면적, 병참선 등을 고려하여 분석하며, 비접근지역 지휘소 및 부대주둔지역 선정지에 활용
 - 기본 원리: 적합지 - 부적합지
 - 상세 원리: (경사도∩식생도∩수송도) - (토질도+배수도(부적합지))

**Syntax**

OptimalStation(SimpleFeatureCollection slopeFeatures, SimpleFeatureCollection vegetationFeatures,  SimpleFeatureCollection soilFeatures, SimpleFeatureCollection roadFeatures, Double roadBuffer, SimpleFeatureCollection drainageFeatures, Double drainageBuffer, DistanceUnit bufferUnit, SimpleFeatureCollection drainageExFeatures, Double minimumArea, AreaUnit areaUnit, Geometry maskArea): SimpleFeatureCollection

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

   * - soilFeatures
     - 토질도 부적합지 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - roadFeatures
     - 수송도 적합지 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - roadBuffer
     - 수송도 분석 거리입니다. 기본값은 300미터 입니다.
     - Double
     - 300
     - ✓

   * - drainageFeatures
     - 배수도 적합지 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - drainageBuffer
     - 배수도 분석거리입니다. 기본값은 3,000미터입니다.
     - Double
     - 3000
     - ✓

   * - bufferUnit
     - 분석거리 단위입니다. 기본값은 Meters 입니다.
     - DistanceUnit
     - Meters
     - ✓

   * - drainageExFeatures
     - 배수도 부적합지 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - minimumArea
     - 배수도(부적합지) 최소면적입니다. 기본값은 30,000 제곱미터입니다.
     - Double
     - 30000
     - ✓

   * - areaUnit
     - 배수도 부적합지 면적 단위입니다. 기본값은 제곱미터입니다.
     - AreaUnit
     - SuareMeters
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
