.. _rasterreclass:

래스터 재분류
=====================

래스터 레이어를 설정한 구간별로 재분류한 래스터를 생성합니다.

**Syntax**

RasterReclass (GridCoverage2D inputCoverage, Integer bandIndex, String ranges, Boolean retainMissingValues) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 재분류할 입력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - bandIndex
     - 0 부터 시작하는 밴드 인덱스, 기본 인덱스는 0입니다.
     - Integer
     - 0
     -

   * - ranges
     - 래스터의 셀값을 재분류하는데 사용할 급간 범위를 설정합니다. 0.0 30.0 1; 30.0 270.0 2; 270.0 365.0 3
     - String
     -
     - ✓

   * - retainMissingValues
     - 재분류 범위에서 제외된 셀값에 NoData를 적용할지 여부를 설정합니다. 기본값은 참(True)으로 분류에세 제외된 원본 셀값을 그대로 출력 셀값에 적용합니다.
     - Boolean
     - true
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
     - 재분류한 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - ranges 파라미터 범위 내의 값들은 NoData값으로 처리한다.

**Examples**
