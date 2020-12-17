.. _rasterflowdirection:

흐름 방향
===============

D8 방법을 사용하여 각 셀에서 아래쪽 경사 방향의 이웃 또는 이웃하는 셀들로부터 흐름 방향의 래스터를 만듭니다.

**Syntax**

RasterFlowDirection (GridCoverage2D inputCoverage) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 표고값을 저장(DEM, DSM 등)한 입력 래스터 레이어입니다.
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
     - 흐름 방향이 계산된 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - 좌표체계, NoData는 입력 데이터의 값을 따른다.

**Examples**

  .. image:: images/rasterflowdirection.png
