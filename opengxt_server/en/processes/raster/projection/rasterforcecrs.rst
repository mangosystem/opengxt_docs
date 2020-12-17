.. _rasterforcecrs:

좌표체계 재정의
========================

기존 래스터의 좌표체계를 설정한 좌표체계로 재정의합니다.

**Syntax**

RasterForceCRS (GridCoverage2D inputCoverage, CoordinateReferenceSystem forcedCRS) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 좌표체계를 정의할 입력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - forcedCRS
     - 정의할 좌표체계를 설정합니다.
     - CoordinateReferenceSystem
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
     - 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - forcedCRS 파라미터는 반드시 [EPSG:코드번호] 형식이어야 한다.

**Examples**

  .. image:: images/rasterforcecrs.png
