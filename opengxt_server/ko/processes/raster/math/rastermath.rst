.. _rastermath:

래스터 수학연산
========================

표현식을 사용하여 래스터에서 수학 연산을 수행합니다.

**Syntax**

RasterMath (GridCoverage2D inputCoverage, Integer bandIndex, Expression expression) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 계산할 입력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - bandIndex
     - 0 부터 시작하는 밴드 인덱스, 기본 인덱스는 0입니다.
     - Integer
     - 0
     -

   * - expression
     - 래스터 셀 값을 평가할 수학 계산식입니다. 예) log(Value * 250)
     - Expression
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
     - 수학 계산식을 이용하여 계산한 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - expression 파라미터에서 사용할 수 있는 함수는 GeoTools의 Filter Function 을 사용한다.

**Examples**
