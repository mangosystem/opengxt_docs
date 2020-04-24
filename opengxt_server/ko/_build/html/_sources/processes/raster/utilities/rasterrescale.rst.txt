.. _rasterrescale:

크기 조절
===============

지정된 x, y 스케일 값으로 래스터의 크기를 조정합니다.

**Syntax**

RasterRescale (GridCoverage2D inputCoverage, Double xScale, Double yScale) : GridCoverage2D

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

   * - xScale
     - X 방향의 래스터 셀 크기에 대한 축척값입니다. 반드시 0보다 커야 하며, 1.0은 원본 값과 동일합니다.
     - Double
     - 1.0
     -

   * - yScale
     - Y 방향의 래스터 셀 크기에 대한 축척값입니다. 반드시 0보다 커야 하며, 1.0은 원본 값과 동일합니다.
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
     - 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - Multi-Band래스터를 지원한다.
 - xScale, yScale 파라미터의 값은 0보다 커야 한다.

**Examples**
