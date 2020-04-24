.. _dissolve:

디졸브
=========

특정 필드값과 속성 집계 함수를 이용하여 디졸브를 수행합니다.

**Syntax**

Dissolve (SimpleFeatureCollection inputFeatures, String dissolveField, String statisticsFields, Boolean useMultiPart) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 디졸브를 수행할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - dissolveField
     - 디졸브를 수행할 고유값을 가진 필드입니다.
     - String
     -
     - ✓

   * - statisticsFields
     - 속성값을 요약할 필드와 요약통계 함수를 설정합니다. 통계 필드 목록은 쉼표로 구분하여 작성할 수 있으며 요약함수.필드명 형식입니다. 사용 가능한 요약함수는 다음과 같습니다: First, Last, Sum, Mean, Min, Max, Std, Count.
     - String
     -
     -

   * - useMultiPart
     - 출력 레이어에서 같은 값을 가진 피처의 멀티파트를 허용할 지 여부를 설정합니다. 기본값은 예(참)입니다. 만약 아니오(거짓)일 경우 멀티파트 지오메트리를 싱글파트 지오메트리로 분리하여 새로운 피처로 저장합니다.
     - Boolean
     - true
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
     - 디졸브를 수행한 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - useMultiPart가 False이면 Dissolve된 피처들을 Single Part로 변환하여 반환한다.
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
