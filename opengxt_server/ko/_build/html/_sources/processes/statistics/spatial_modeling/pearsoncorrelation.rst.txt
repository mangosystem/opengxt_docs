.. _pearsoncorrelation:

피어슨 상관 계수
===========================

피어슨 상관 계수는 두 변수의 공분산을 표준 편차의 곱으로 나눔으로써 구합니다.

**Syntax**

Pearson (SimpleFeatureCollection inputFeatures, String inputFields) : PearsonResult

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 피어슨 상관계수를 계산할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - inputFields
     - 피어슨 상관계수를 계산할 속성을 담고 있는 쉼표로 구분된 숫자 필드의 목록입니다.
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
     - 피어슨 상관계수 분석결과입니다.
     - PearsonResult
     -
     - ✓

**Constraints**

 - Output은 XML로 반환한다.

**Examples**

pop2008, pop_den 두 필드를 이용하여 Pearson 상관 계수를 분석한 결과는 다음의 XML 포맷으로 반환됩니다.

  .. code-block::

    <?xml version="1.0" encoding="utf-8"?>
    <PearsonResult>
      <PropertyName Name="pop2008">
        <Item Name="pop2008">
          <Value>1.0</Value>
        </Item>
        <Item Name="pop_den">
          <Value>0.3002549407911261</Value>
        </Item>
      </PropertyName>
      <PropertyName Name="pop_den">
        <Item Name="pop2008">
          <Value>0.3002549407911261</Value>
        </Item>
        <Item Name="pop_den">
          <Value>1.0</Value>
        </Item>
      </PropertyName>
    </PearsonResult>
