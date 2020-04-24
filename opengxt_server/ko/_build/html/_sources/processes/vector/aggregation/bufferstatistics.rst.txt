.. _bufferstatistics:

버퍼를 이용한 포인트 집계
==========================================

각 피처로부터 탐색반경만큼 버퍼 실행 후 그 안에 포함된 포인트의 갯수 또는 속성정보를 가져옵니다.

**Syntax**

BufferPointStatistics (SimpleFeatureCollection inputFeatures, Double distance, DistanceUnit distanceUnit, SimpleFeatureCollection pointFeatures, String countField, String statisticsFields) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 속성정보가 계산될 벡터 레이어
     - SimpleFeatureCollection
     -
     - ✓

   * - distance
     - 탐색 반경
     - Double
     - 0.0
     - ✓

   * - distanceUnit
     - 탐색 반경의 거리단위입니다.
     - DistanceUnit
     - Default
     -

   * - pointFeatures
     - 탐색 대상 포인트 레이어
     - SimpleFeatureCollection
     -
     - ✓

   * - countField
     - 포인트수 필드.
     - String
     - count
     -

   * - statisticsFields
     - 집계필드 목록: Function.PropertyName(First, Last, Sum, Mean, Min, Max, Std, Count)
     - String
     -
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
     - 출력 레이어.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - distanceUnit: Default(기본값), Meters, Kilometers, Inches, Feet, Yards, Miles, NauticalMiles
 - countField는 폴리곤 내에 포함되는 포인트의 개수가 저장되며, 기본값은 count이다.
 - Statistics Fields는 다음과 같이 [함수명.필드명] 구조로 입력하며 사용 가능한 함수는 다음과 같다. 예) Sum.pop, Mean.pop

 .. list-table::
    :widths: 60 20

    * - **입력값**
      - **반환 필드명**

    * - First: String 필드, 대상 Feature의 첫 번째 값
      - SUM_필드명

    * - Last: String 필드, 대상 Feature의 마지막 값
      - LST_필드명

    * - Sum: Numeric 필드, 대상 Feature의 합
      - 셀의 평균값(기본값)

    * - Mean: Numeric 필드, 대상 Feature의 평균값
      - AVG_필드명

    * - Min: Numeric 필드, 대상 Feature의 최소값
      - MIN_필드명

    * - Max: Numeric 필드, 대상 Feature의 최대값
      - MAX_필드명

    * - Std: Numeric 필드, 대상 Feature의 표준편차
      - STD_필드명

    * - Var: Numeric 필드, 대상 Feature의 분산
      - VAR_필드명

    * - Range: Numeric 필드, 대상 Feature의 범위
      - RNG_필드명

    * - Count: 대상 Feature의 수	FST_필드명
      - CNT_필드명

**Examples**
