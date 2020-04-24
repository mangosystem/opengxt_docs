.. _joincountstatistics:

조인 카운트 통계량
==============================

이진 데이터에 대한 전역적 공간 자기상관을 측정합니다. (예 : 1 또는 B (검정) , 0 또는 W (흰색)로 정의된 관측값 사용).

**Syntax**

JoinCount (SimpleFeatureCollection inputFeatures, Filter blackExpression, ContiguityType contiguityType) : JoinCountProcessResult

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 조인 카운트 통계량을 계산할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - blackExpression
     - 1 또는 참(블랙) 값을 나타내는 블랙 표현식입니다. 예) [pop] > 1500
     - Filter
     -
     - ✓

   * - contiguityType
     - 이웃 정의 유형 (Queen, Rook, Bishops).
     - ContiguityType
     - Queen
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
     - 조인 카운트 통계량입니다.
     - JoinCountProcessResult
     -
     - ✓

**Constraints**

 - contiguityType: Queen(기본값), Rook, Bishops
 - blackExpression 파라미터는 필드 또는 필드를 조합한 수식 모두 가능하다.
 - Output은 XML로 반환한다.


**Examples**

  .. code-block::

    <?xml version="1.0" encoding="utf-8"?>
    <JoinCountStatistics>
      <TypeName>sgg</TypeName>
      <ContiguityType>Queen</ContiguityType>
      <FeatureCount>25</FeatureCount>
      <BlackCount>11</BlackCount>
      <WhiteCount>14</WhiteCount>
      <NumberOfJoins>56</NumberOfJoins>
      <ObservedBB>11</ObservedBB>
      <ObservedWW>18</ObservedWW>
      <ObservedBW>27</ObservedBW>
      <ExpectedBB>10.8416</ExpectedBB>
      <ExpectedWW>17.561600000000002</ExpectedWW>
      <ExpectedBW>27.5968</ExpectedBW>
      <StdDevBB>5.487588556005269</StdDevBB>
      <StdDevWW>6.831669500202715</StdDevWW>
      <StdDevBW>3.9479960283667954</StdDevBW>
      <ZScoreBB>0.028865137825731742</ZScoreBB>
      <ZScoreWW>0.06417172259094052</ZScoreWW>
      <ZScoreBW>-0.15116529898002093</ZScoreBW>
    </JoinCountStatistics>
