.. _escaperange:

침투 적 도주 범위 분석
====================================
아군 후방지역에 침투한 적이 주민신고나 아군 부대에 식별되어 도주할 경우 예상 도주 범위를 판단하는데 활용하기 위해 제작된 모델로 식별원점을 기준으로, 도주속도, 분석 범위, 기상 지연 계수, 시간 범위 설정을 기준으로 시간대별로 도주 가능한 범위를 폴리곤과 선으로 결과 값 표출

**Syntax**

EscapeRange(Geometry origin, GridCoverage2D speedRaster, Double radius, DistanceUnit radiusUnit, WeatherFactor weatherFactor, Integer startTime, Integer endTime, Geometry maskArea): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - origin
     - 식별 원점 포인트 지오메트리입니다.
     - Geometry
     -
     - ✓

   * - speedRaster
     - 도주속도를 계산한 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - radius
     - 도주속도 최대 분석 반경입니다.
     - Double
     -
     - ✓

   * - radiusUnit
     - 분석반경 단위입니다. 기본값은 Meters 입니다.
     - DistanceUnit
     - Meters
     - ✓

   * - weatherFactor
     - 기상지연 계수입니다. Normal(일반): 1, Foggy(안개): 1.3, Rainy(강우/적설): 1.6, Night(야간): 1.1
     - WeatherFactor
     - Normal
     - ✓

   * - startTime
     - 분 단위의 시작 시간입니다.
     - Integer
     -
     - ✓

   * - endTime
     - 분 단위의 종료시간입니다.
     - Integer
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
