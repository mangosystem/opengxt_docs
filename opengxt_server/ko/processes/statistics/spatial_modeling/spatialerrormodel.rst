.. _spatialerrormodel:

Spatial Error Model (SEM)
==========================

Maximum Likelihood Spatial Error Model (공간오차모형, SEM)을 수행하빈다.

**Syntax**

SpatialErrorModel (SimpleFeatureCollection inputFeatures, String dependentVariable, String explanatoryVariables, SpatialConcept spatialConcept, DistanceMethod distanceMethod, StandardizationMethod standardization, Double searchDistance) : SimpleFeatureCollection, SpatialErrorResult

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
     - SpatialErrorResult
     -
     - ✓

**Constraints**

 - Output은 XML로 반환한다.

**Examples**

a1_2000 필드를 종속변수로, a2_2000, a3_2000, a4_2000 필드를 설명변수로 분석한 결과는 다음의 XML 포맷으로 반환됩니다.

.. code-block:: XML

    <?xml version="1.0" encoding="UTF-8"?>
    <SpatialErrorModel>
      <ModelName>Maximum Likelihood Spatial Error</ModelName>
      <Dataset>seoul_series</Dataset>
      <DependentVariable>a1_2000</DependentVariable>
      <NumberOfObservations>25</NumberOfObservations>
      <NumberOfVariables>4</NumberOfVariables>
      <DegreesOfFreedom>21</DegreesOfFreedom>
      <MeanDependentVar>18229.716524000003</MeanDependentVar>
      <SdDependentVar>5222.973372203831</SdDependentVar>
      <LagCoefficient>-0.24851881360049768</LagCoefficient>
      <RSquared>0.2518656668858821</RSquared>
      <PseudoRSquared>0.25196101716592434</PseudoRSquared>
      <SigmaSquareML>1.8812637542498086E7</SigmaSquareML>
      <SeOfRegression>4337.353748830972</SeOfRegression>
      <LogLikelihood>-245.02018916073624</LogLikelihood>
      <AkaikeCriterion>498.0403783214725</AkaikeCriterion>
      <SchwarzCriterion>502.9158816209453</SchwarzCriterion>
      <Summary>
        <Variable>
          <Variable>CONSTANT</Variable>
          <Coefficient>-88317.68976363928</Coefficient>
          <StandardError>37270.805072442025</StandardError>
          <ZStatistic>-2.369621197931709</ZStatistic>
          <Probability>0.017806318045455766</Probability>
        </Variable>
        <Variable>
          <Variable>a2_2000</Variable>
          <Coefficient>995.8416093808737</Coefficient>
          <StandardError>382.5707273790552</StandardError>
          <ZStatistic>2.603026154675402</ZStatistic>
          <Probability>0.009240490401231434</Probability>
        </Variable>
        <Variable>
          <Variable>a3_2000</Variable>
          <Coefficient>693.7113928797462</Coefficient>
          <StandardError>621.213541267178</StandardError>
          <ZStatistic>1.1167035919157267</ZStatistic>
          <Probability>0.2641210995973676</Probability>
        </Variable>
        <Variable>
          <Variable>a4_2000</Variable>
          <Coefficient>136.8233103433231</Coefficient>
          <StandardError>551.1711267400561</StandardError>
          <ZStatistic>0.24824107016014255</ZStatistic>
          <Probability>0.8039478914561922</Probability>
        </Variable>
        <Variable>
          <Variable>lambda</Variable>
          <Coefficient>-0.24851881360049768</Coefficient>
          <StandardError>0.3002979071631366</StandardError>
          <ZStatistic>-0.8275742443502613</ZStatistic>
          <Probability>0.40791166731613593</Probability>
        </Variable>
      </Summary>
    </SpatialErrorModel>
