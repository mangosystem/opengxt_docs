.. _rastersetnull:

래스터 Null값 설정
====================================

필터 표현식에 해당하는 셀값을 Null(NoData)값으로 처리한 래스터를 생성합니다.

**Syntax**

RasterSetNull (GridCoverage2D inputCoverage, Integer bandIndex, Filter filter, Boolean replaceNoData, Double newValue) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 변환할 입력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - bandIndex
     - 0 부터 시작하는 밴드 인덱스, 기본 인덱스는 0입니다.
     - Integer
     - 0
     -

   * - filter
     - NoData로 설정할 필터 표현식입니다. 예) Value > 250
     - Filter
     -
     - ✓

   * - replaceNoData
     - 만약 예(True)이면 기존 NoData값을 새로운 NoData 값으로 대체합니다. 기본값은 아니오(False)입니다.
     - Boolean
     - false
     -

   * - newValue
     - 기존 NoData 값을 대체할 새로운 값을 설정합니다.
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

   * - result
     - Null값이 설정된 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - filter 파라미터의 필드 이름은 반드시 Value 이어야 한다.
 - replaceNoData 파라미터의 값이 True인 경우 기존 NoData값을 newValue 파라미터 값으로 대체한다.


**Examples**
