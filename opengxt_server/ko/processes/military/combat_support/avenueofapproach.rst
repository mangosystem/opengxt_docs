.. _avenueofapproach:

피아접근로 분석
====================================
아군과 적군이 접근 가능한 경로 분석으로, 작전부대 규모 및 보유장비 기동에 양호한 도로망 판단 및 도로사용 제한 시 야지 기동이 적합한 기동 공간을 분석
  - 기본 원리: 적합지 - 부적합지
  - 상세 원리: 도로를 제외한 지역, (경사도∩식생도) - (토질도+배수도+도심지)
  - 상세 원리: 도로만 한정한 지역, 날씨 유형과 도로의 표면상태, 차선 수를 고려하여 도로를 피아접근로 양호, 보통, 불량으로 구분


**Syntax**

AvenueOfApproach(SimpleFeatureCollection slopeFeatures, SimpleFeatureCollection forestFeatures,  SimpleFeatureCollection soilFeatures, SimpleFeatureCollection townFeatures, SimpleFeatureCollection drainageFeatures, SimpleFeatureCollection roadFeatures,  Geometry maskArea): SimpleFeatureCollection

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

   * - roadFeatures
     - 수송도 레이어입니다.
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
