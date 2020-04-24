.. _anova:

분산분석(ANOVA Test)
=====================

분산분석(Analysis of Variance, ANOVA)을 수행합니다.

**Syntax**

Anova (SimpleFeatureCollection inputFeatures, String fields) : AnovaResult

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 분석 변수를 포함하고 있는 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - fields
     - 쉼표로 분리된 분석에 필요한 숫자값을 가진 필드 목록입니다.
     - String
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
     - 분산분석 결과입니다.
     - AnovaResult
     -
     - ✓

**Constraints**

 - Output은 XML로 반환한다.

**Examples**

a1_2000, a2_2000, a3_2000, a4_2000 4개의 필드를 이용하여 분산분석을 수행한 결과는 다음의 XML 포맷으로 반환됩니다.

  .. code-block::

    <?xml version="1.0" encoding="UTF-8"?>
    <Anova>
      <Treatments>
        <Factor>Between Groups</Factor>
        <SumOfSquares>6.205958517716355E9</SumOfSquares>
        <DegreesOfFreedom>3.0</DegreesOfFreedom>
        <MeanSquare>2.068652839238785E9</MeanSquare>
        <FStatistics>303.3275165487872</FStatistics>
        <PValue>1.1102230246251565E-16</PValue>
      </Treatments>
      <Error>
        <Factor>Within Groups</Factor>
        <SumOfSquares>6.547070797481773E8</SumOfSquares>
        <DegreesOfFreedom>96.0</DegreesOfFreedom>
        <MeanSquare>6819865.414043513</MeanSquare>
      </Error>
      <Total>
        <Factor>Total</Factor>
        <SumOfSquares>6.860665597464533E9</SumOfSquares>
        <DegreesOfFreedom>99.0</DegreesOfFreedom>
      </Total>
      <Summary>
        <Group>
          <Group>a1_2000</Group>
          <Count>25</Count>
          <Minimum>7902.3838</Minimum>
          <Maximum>28062.184</Maximum>
          <Sum>455742.91310000006</Sum>
          <Average>18229.716524000003</Average>
          <Variance>2.727945084675026E7</Variance>
        </Group>
        <Group>
          <Group>a2_2000</Group>
          <Count>25</Count>
          <Minimum>96.724518</Minimum>
          <Maximum>105.01617</Maximum>
          <Sum>2515.9517890000006</Sum>
          <Average>100.63807156000003</Average>
          <Variance>4.840012157224312</Variance>
        </Group>
        <Group>
          <Group>a3_2000</Group>
          <Count>25</Count>
          <Minimum>5.2713499</Minimum>
          <Maximum>11.17146</Maximum>
          <Sum>218.94218979999997</Sum>
          <Average>8.757687591999998</Average>
          <Variance>2.508762737460472</Variance>
        </Group>
        <Group>
          <Group>a4_2000</Group>
          <Count>25</Count>
          <Minimum>0.22132</Minimum>
          <Maximum>9.58605</Maximum>
          <Sum>37.27112993</Sum>
          <Average>1.4908451972</Average>
          <Variance>3.4606488978589653</Variance>
        </Group>
      </Summary>
    </Anova>
