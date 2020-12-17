.. _rasterrotate:

회전
======

지정된 피벗 포인트를 중심으로 도 단위로 지정된 각도값 만큼 래스터를 회전합니다.

**Syntax**

RasterRotate (GridCoverage2D inputCoverage, Point anchorPoint, Double angle, ResampleType interpolation) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 회전할 입력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - anchorPoint
     - 래스터를 회전시킬 피벗 포인트입니다. 기본값은 입력 래스터 데이터 세트의 왼쪽 하단입니다.
     - Point
     -
     -

   * - angle
     - 래스터를 회전할 도 단위의 각도를 설정합니다.
     - Double
     - 0.0
     - ✓

   * - interpolation
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
     - 회전한 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - interpolation: NEAREST(기본값), BILINEAR, BICUBIC
 - Multi-Band래스터를 지원한다.
 - anchorPoint 파라미터가 Null이면 래스터 Extent의 좌하단을 기준으로 한다.
 - angle 파라미터의 단위는 도(Degree) 단위를 사용한다.


**Examples**

  .. image:: images/rasterrotate.png
