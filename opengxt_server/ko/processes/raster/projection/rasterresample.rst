.. _rasterresample:

리샘플링
============

래스터를 설정한 셀 크기와 리샘플 방법에 따라 리샘플링 합니다.

**Syntax**

RasterResample (GridCoverage2D inputCoverage, Double cellSize, ResampleType resamplingType) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 래스터 셀 크기(공간 해상도)를 변경할 입력 래스터 레이어입니다.
     - GridCoverage2D
     - 
     - ✓

   * - cellSize
     - 새로운 출력 래스터의 셀 크기를 설정합니다. 0보다 큰 값을 반드시 설정해야 합니다.
     - Double
     - 0.0
     - ✓

   * - resamplingType
     - 리샘플링 방법을 설정합니다. NEAREST(기본값), BILINEAR, BICUBIC.
     - ResampleType
     - NEAREST
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
     - 리샘플링한 출력 래스터 레이어입니다.
     - GridCoverage2D
     - 
     - ✓

**Constraints**

 - resamplingType: NEAREST(기본값), BILINEAR, BICUBIC

**Examples**

