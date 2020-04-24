.. _pointstatistics:

포인트 집계
==================

각 폴리곤 피처에 포함된 포인트 피처 속성의 통계값을 계산합니다.

**Syntax**

PointStatistics (SimpleFeatureCollection polygonFeatures, SimpleFeatureCollection pointFeatures, String countField, String statisticsFields) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - polygonFeatures
     - 폴리곤 레이어.
     - SimpleFeatureCollection
     -
     - ✓

   * - pointFeatures
     - 포인트 레이어.
     - SimpleFeatureCollection
     -
     - ✓

   * - countField
     - 포인트수 필드.
     - String
     - count
     -

   * - statisticsFields
     - 집계 필드: 함수.필드명(First, Last, Sum, Mean, Min, Max, Std, Count)
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
     - 결과
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures는 폴리곤, pointFeatures는 포인트 피처 타입이어야 한다.
 - countField는 폴리곤 내에 포함되는 포인트의 개수가 저장되며, 기본값은 count이다.
 - Statistics Fields는 다음과 같이 [함수명.필드명] 구조로 입력하며 사용가능한 함수는 다음과 같다. 예) Sum.pop, Mean.pop

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
