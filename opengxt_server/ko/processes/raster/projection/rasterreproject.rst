.. _rasterreproject:

래스터 좌표체계 변환
=================================

래스터를 새로운 좌표체계로 변환합니다.

**Syntax**

RasterReproject (GridCoverage2D inputCoverage, CoordinateReferenceSystem targetCRS, ResampleType resamplingType, Double cellSize, CoordinateReferenceSystem forcedCRS) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 좌표체계를 변환할 입력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - targetCRS
     - 좌표체계 변환에 사용할 대상 좌표체계 입니다.
     - CoordinateReferenceSystem
     -
     - ✓

   * - resamplingType
     - 좌표체계 변환에 사용되는 리샘플링 방법을 설정합니다. NEAREST(기본값), BILINEAR, BICUBIC.
     - ResampleType
     - NEAREST
     -

   * - cellSize
     - 출력 레이어의 셀 크기입니다.
     - Double
     - 0.0
     -

   * - forcedCRS
     - 입력 래스터 레이어의 원본 좌표체계를 정의합니다.
     - CoordinateReferenceSystem
     -
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
     - 좌표체계를 변환한 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - resamplingType: NEAREST(기본값), BILINEAR, BICUBIC
 - targetCRS, forcedCRS 파라미터는 반드시 [EPSG:코드번호] 형식이어야 한다.
 - cellSize 파라미터를 설정하지 않으면 원본 셀 크기를 사용하며, 만약 지리좌표계에서 투영 좌표계로 변환하는 경우에는 해당 단위로 환산한 셀 크기가 적용된다.
 - forcedCRS 파라미터를 설정하면 원본 래스터 데이터의 좌표체계를 설정한 좌표체계로 정의하여 변환한다.


**Examples**
