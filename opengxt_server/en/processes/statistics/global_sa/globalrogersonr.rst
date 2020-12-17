.. _globalrogersonr:

Rogerson의 전역적 R 통계량
=========================================================

Rogerson의 전역적 R 통계량을 계산합니다.

**Syntax**

GlobalRogersonR (SimpleFeatureCollection inputFeatures, String xField, String yField, DistanceMethod distanceMethod, Double kappa) : RogersonRProcessResult

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 통계량을 계산할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - xField
     - 수치형 입력 변수 X 필드 변수를 설정합니다.
     - String
     -
     - ✓

   * - yField
     - 수치형 입력 변수 Y 필드 변수를 설정합니다.
     - String
     -
     - ✓

   * - distanceMethod
     - 분석 대상 피처로부터 이웃 피처까지의 거리를 계산하는 방법을 설정합니다.
     - DistanceMethod
     - Euclidean
     -

   * - kappa
     - 거리에 대한 중요도를 설정합니다.
     - Double
     - 1.0
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
     - 출력 레이어입니다.
     - RogersonRProcessResult
     -
     - ✓

**Constraints**

 - distanceMethod: Euclidean(기본값), Manhattan
 - Output은 XML로 반환한다.

**Examples**

.. code-block:: XML
  
    <?xml version="1.0" encoding="UTF-8"?>
    <GlobalRogersonsR>
      <TypeName>seoul_series</TypeName>
      <XField>a1_2005</XField>
      <YField>a3_2005</YField>
      <Observed_Index>0.10881633</Observed_Index>
      <Expected_Index>0.00005314</Expected_Index>
      <Variance>0</Variance>
      <Z_Score>39315316.41203745</Z_Score>
      <P_Value>0</P_Value>
      <Conceptualization>InverseDistance</Conceptualization>
      <DistanceMethod>Euclidean</DistanceMethod>
      <RowStandardization>None</RowStandardization>
      <DistanceThreshold>6740.77538129</DistanceThreshold>
      <Kappa>1</Kappa>
    </GlobalRogersonsR>
