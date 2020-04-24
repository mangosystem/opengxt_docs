.. _spatiallagmodel:

Spatial Lag Model (SLM)
=========================

Maximum Likelihood Spatial Lag Model (공간시차모형, SLM)을 수행합니다.

**Syntax**

SpatialLagModel (SimpleFeatureCollection inputFeatures, String dependentVariable, String explanatoryVariables, SpatialConcept spatialConcept, DistanceMethod distanceMethod, StandardizationMethod standardization, Double searchDistance) : SimpleFeatureCollection, SpatialLagResult

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 종속변수와 독립변수를 포함하고 있는 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - dependentVariable
     - 종속변수값을 가진 숫자 필드입니다.
     - String
     -
     - ✓

   * - explanatoryVariables
     - 회귀 분석에 사용할 쉼표로 구분된 설명 변수 숫자 필드의 목록입니다.
     - String
     -
     - ✓

   * - spatialDiagnotics
     - Lagrange multiplier, Moran's I 등 공간 진단을 포함할 지 여부를 설정합니다.
     - Boolean
     -
     - ✓

   * - spatialConcept
     - 피처들 간에 공간 관계를 설정하는 방식을 선택합니다.
     - SpatialConcept
     - InverseDistance
     -

   * - distanceMethod
     - 분석 대상 피처로부터 이웃 피처까지의 거리를 계산하는 방법을 설정합니다.
     - DistanceMethod
     - Euclidean
     -

   * - standardization
     - 통계량 계산시 행 표준화 적용 여부를 설정합니다.
     - StandardizationMethod
     - None
     -

   * - searchDistance
     - 역거리 혹은 고정 거리 옵션 선택 시 기준 값을 지정합니다.
     - Double
     - 0.0
     -

**Process Outputs**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - resFeatures
     - 종속 변수 추정치와 잔차를 포함한 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     -

   * - report
     - 분석 결과입니다.
     - SpatialLagResult
     -
     - ✓

**Constraints**

 - Output은 XML로 반환한다.

**Examples**

a1_2000 필드를 종속변수로, a2_2000, a3_2000, a4_2000 필드를 설명변수로 분석한 결과는 다음의 XML 포맷으로 반환됩니다.

  .. code-block::

    <?xml version="1.0" encoding="UTF-8"?>
    <SpatialLagModel>
      <ModelName>Maximum Likelihood Spatial Lag</ModelName>
      <Dataset>seoul_series</Dataset>
      <DependentVariable>a1_2000</DependentVariable>
      <NumberOfObservations>25</NumberOfObservations>
      <NumberOfVariables>5</NumberOfVariables>
      <DegreesOfFreedom>20</DegreesOfFreedom>
      <MeanDependentVar>18229.716524000003</MeanDependentVar>
      <SdDependentVar>5222.973372203831</SdDependentVar>
      <LagCoefficient>-0.22828542473968091</LagCoefficient>
      <RSquared>0.2761455213123636</RSquared>
      <PseudoRSquared>0.27640866645133527</PseudoRSquared>
      <SpatialPseudoRSquared>0.24256289672449238</SpatialPseudoRSquared>
      <SigmaSquareML>1.895649856469702E7</SigmaSquareML>
      <SeOfRegression>4353.906127226105</SeOfRegression>
      <LogLikelihood>-245.08902967323908</LogLikelihood>
      <AkaikeCriterion>500.17805934647816</AkaikeCriterion>
      <SchwarzCriterion>506.27243847081917</SchwarzCriterion>
      <Summary>
        <Variable>
          <Variable>CONSTANT</Variable>
          <Coefficient>-95376.43702193913</Coefficient>
          <StandardError>41547.093017760526</StandardError>
          <ZStatistic>-2.2956223912264493</ZStatistic>
          <Probability>0.02169748136498197</Probability>
        </Variable>
        <Variable>
          <Variable>a2_2000</Variable>
          <Coefficient>1109.0234412138893</Coefficient>
          <StandardError>433.37762273421095</StandardError>
          <ZStatistic>2.559023316010134</ZStatistic>
          <Probability>0.010496670100781556</Probability>
        </Variable>
        <Variable>
          <Variable>a3_2000</Variable>
          <Coefficient>689.0420222891909</Coefficient>
          <StandardError>620.0027530256691</StandardError>
          <ZStatistic>1.1113531656538684</ZStatistic>
          <Probability>0.2664163810038307</Probability>
        </Variable>
        <Variable>
          <Variable>a4_2000</Variable>
          <Coefficient>62.425662528753676</Coefficient>
          <StandardError>519.9203359561636</StandardError>
          <ZStatistic>0.12006774540555191</ZStatistic>
          <Probability>0.9044294829669831</Probability>
        </Variable>
        <Variable>
          <Variable>W_a1_2000</Variable>
          <Coefficient>-0.22828542473968091</Coefficient>
          <StandardError>0.2815172692688138</StandardError>
          <ZStatistic>-0.8109109090629067</ZStatistic>
          <Probability>0.4174168425394321</Probability>
        </Variable>
      </Summary>
    </SpatialLagModel>
