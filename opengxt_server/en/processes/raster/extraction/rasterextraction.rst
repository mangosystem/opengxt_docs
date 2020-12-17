.. _rasterextraction:

셀값으로 래스터 추출
=================================

설정한 필터 표현식에 해당하는 래스터를 추출합니다.

**Syntax**

RasterExtraction (GridCoverage2D inputCoverage, Integer bandIndex, Filter filter) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 추출할 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - bandIndex
     - 0 부터 시작하는 밴드 인덱스, 기본 인덱스는 0입니다.
     - Integer
     - 0
     -

   * - filter
     - 래스터의 셀값을 추출할 필터 표현식입니다. 예) Value > 250
     - Filter
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
     - 필터 표현식으로 추출한 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - filter 파라미터의 필드 이름은 반드시 Value 이어야 한다.
 - filter 파라미터는 공간 필터를 사용할 수 있다.

**Examples**

  .. image:: images/rasterextraction.png
