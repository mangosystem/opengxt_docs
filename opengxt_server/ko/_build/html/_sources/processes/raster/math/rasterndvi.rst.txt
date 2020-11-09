.. _rasterndvi:

식생지수(NDVI) 계산
=======================================

2개의 래스터 밴드로부터 Normalized Difference Vegetation Index (NDVI)를 계산합니다.

**Syntax**

RasterNDVI (GridCoverage2D nirCoverage, Integer nirIndex, GridCoverage2D redCoverage, Integer redIndex) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - nirCoverage
     - 근적외선(near infrared) 밴드 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - nirIndex
     - 0 부터 시작하는 근적외선(Near Infrared) 밴드 인덱스, 기본 인덱스는 0입니다.
     - Integer
     - 0
     - ✓

   * - redCoverage
     - 가시광선(Red) 밴드 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - redIndex
     - 0 부터 시작하는 가시광선(Red) 밴드 인덱스, 기본 인덱스는 0입니다.
     - Integer
     - 0
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
     - 식생지수가 계산된 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - 두 개의 셀값 중 하나가 NoData인 경우 NoData값을 반환한다.

**Examples**

  .. image:: images/rasterndvi.png
