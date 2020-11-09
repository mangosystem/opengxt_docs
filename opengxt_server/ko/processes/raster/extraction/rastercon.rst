.. _rastercon:

래스터 조건 평가
===========================

래스터의 각 셀값에 대해 if / else 조건부를 평가하여 참인 경우와 거짓인 경우에 해당하는 셀값의 래스터를 생성합니다.

**Syntax**

RasterCon (GridCoverage2D inputCoverage, Integer bandIndex, Filter filter, Integer trueValue, Integer falseValue) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 조건에 사용될 입력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - bandIndex
     - 0 부터 시작하는 밴드 인덱스, 기본 인덱스는 0입니다.
     - Integer
     - 0
     -

   * - filter
     - 참 거짓을 판단할 수 있는 필터 표현식을 정의합니다. 예) Value > 250
     - Filter
     -
     - ✓

   * - trueValue
     - 조건 필터 표현식의 값이 참(True)일 경우 래스터 셀에 할당할 값입니다.
     - Integer
     - 1
     - ✓

   * - falseValue
     - 조건 필터 표현식의 값이 거짓(False)일 경우 래스터 셀에 할당할 값입니다.
     - Integer
     - -2147483648
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
     - 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - filter 파라미터의 필드 이름은 반드시 Value 이어야 한다.
 - trueValue와 falseValue 파라미터는 반드시 Integer값이어야 한다.
 - falseValue 파라미터값이 Null인 경우 NoData값을 적용한다.

**Examples**

  .. image:: images/rastercon.png
