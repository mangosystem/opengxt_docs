.. _rasterflip:

플립
======

래스터의 중심을 기준으로 수평 축을 따라 위쪽에서 아래쪽으로 뒤집어 래스터의 방향을 조정합니다.

**Syntax**

RasterFlip (GridCoverage2D inputCoverage) : GridCoverage2D

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

**Process Outputs**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - result
     - 플립한 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - Multi-Band래스터를 지원한다.

**Examples**
