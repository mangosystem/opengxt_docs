.. _statisticsfeatures:

피처 레이어 요약 통계
====================================

피처 레이어의 필드(여러 필드 사용 가능)값에 대한 요약 통계(최소값, 최대값, 평균, 합, 분산, 표준편차, 범위 등)를 계산합니다.

**Syntax**

StatisticsFeatures (SimpleFeatureCollection inputFeatures, String inputFields, String caseField) : DataStatisticsResult

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 요약 통계를 계산할 필드를 포함하고 있는 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - inputFields
     - 요약통계를 계산할 단일 필드 또는 쉼표로 구분된 숫자 필드 목록입니다.
     - String
     -
     - ✓

   * - caseField
     - 요약 통계를 그룹화하여 계산할 그룹 필드입니다.
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
     - 출력 통계 정보입니다.
     - DataStatisticsResult
     -
     - ✓

**Constraints**

 - caseField 파라미터가 설정되면 caseField의 고유값별로 통계정보가 생성된다.
 - Output은 XML로 반환한다.


**Examples**

  .. code-block::

    <?xml version="1.0" encoding="utf-8"?>
    <DataStatistics>
      <Item>
        <TypeName>korea_sgg</TypeName>
        <CaseValue>강원도</CaseValue>
        <PropertyName>a3_2000</PropertyName>
        <Count>18</Count>
        <InvalidCount>0</InvalidCount>
        <Minimum>0.24774</Minimum>
        <Maximum>7.81668</Maximum>
        <Range>7.56894</Range>
        <Ranges>0.24774 - 7.81668</Ranges>
        <Sum>79.64533043000002</Sum>
        <Mean>4.424740579444445</Mean>
        <Variance>6.976857255428096</Variance>
        <StandardDeviation>2.641374122578643</StandardDeviation>
        <CoefficientOfVariance>0.5969557028607279</CoefficientOfVariance>
      </Item>
      <Item>
        <TypeName>korea_sgg</TypeName>
        <CaseValue>경기도</CaseValue>
        <PropertyName>a3_2000</PropertyName>
        <Count>31</Count>
        <InvalidCount>0</InvalidCount>
        <Minimum>0.0</Minimum>
        <Maximum>15.46253</Maximum>
        <Range>15.46253</Range>
        <Ranges>0.0 - 15.46253</Ranges>
        <Sum>271.03358996</Sum>
        <Mean>8.74301903096774</Mean>
        <Variance>21.209124717119646</Variance>
        <StandardDeviation>4.605336547649872</StandardDeviation>
        <CoefficientOfVariance>0.5267444267635456</CoefficientOfVariance>
    </Item>
    ...
    </DataStatistics>
