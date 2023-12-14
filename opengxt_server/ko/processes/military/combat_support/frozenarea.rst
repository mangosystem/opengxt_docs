.. _frozenarea:

상습 결빙지역 분석
====================================
수치 고도 자료와 경사를 이용한 동계 기동장비 이동에 제한을 주는 결빙 도로지역을 추출한 결과로서, 동계 안전한 부대 이동계획을 수립 하는데 활용
 - 기본 원리: 수송도 ∩ 결빙지역
 - 상세 원리: 수송도(버퍼) ∩ 결빙지역(수치고도자료로 분석한 결빙지역)

**Syntax**

FrozenArea(SimpleFeatureCollection roadFeatures, double distance, DistanceUnit distanceUnit, SimpleFeatureCollection slopeFeatures, SimpleFeatureCollection aspectFeatures, SimpleFeatureCollection hillshadeFeatures, Geometry maskArea): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - roadFeatures
     - 수송도 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - distance
     - 수송도 분석거리입니다. 기본값은 30미터입니다.
     - Double
     - 30
     - ✓

   * - distanceUnit
     - 수송도 분석거리 단위입니다. 기본값은 Meters 입니다.
     - DistanceUnit
     - Meters
     - ✓

   * - slopeFeatures
     - 경사도 레이어입니다. 기본값은 10도 이상입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - aspectFeatures
     - 사면향 레이어입니다. 기본값은 북서(292.5~360도), 정북(0,360), 북동(0~67.5)입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - hillshadeFeatures
     - 음영 레이어입니다. 기본값은 광원의 방위각 180도, 높이각 29도에서의 음영(0~50) 기준입니다.
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
