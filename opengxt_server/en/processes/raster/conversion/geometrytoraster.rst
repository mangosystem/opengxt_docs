.. _geometrytoraster:

지오메트리를 래스터로 변환
==========================================

지오메트리를 설정한 값과 픽셀 유형에 맞게 래스터로 변환합니다.

**Syntax**

GeometryToRaster (Geometry inputGeometry, CoordinateReferenceSystem forcedCRS, Number defaultValue, RasterPixelType pixelType, Double cellSize, ReferencedEnvelope extent) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputGeometry
     - 래스터 레이어로 변환할 입력 지오메트리입니다.
     - Geometry
     -
     - ✓

   * - forcedCRS
     - 입력 지오메트리의 좌표체계입니다.
     - CoordinateReferenceSystem
     -
     -

   * - defaultValue
     - 래스터의 해당 픽셀에 저장될 기본값으로 1을 기본값으로 합니다.
     - Number
     - 1
     -

   * - pixelType
     - 출력 래스터 레이어의 픽셀 유형입니다.
     - RasterPixelType
     - INTEGER
     -

   * - cellSize
     - 출력 래스터 레이어의 셀 크기입니다.
     - Double
     - 0.0
     -

   * - extent
     - 출력 래스터 레이어의 공간 범위입니다. 이 값을 설정하지 않으면 지오메트리의 공간 범위를 기본값으로 사용합니다.
     - ReferencedEnvelope
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
     - 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - pixelType: BYTE, SHORT, INTEGER(기본값), FLOAT, DOUBLE
 - forcedCRS 파라미터가 Null이면 inputGeometry의 CRS값을 사용하며, 이때 inputGeometry의 CRS를 반드시 설정해야 한다.
 - defaultValue 파라미터가 Null이면 기본값으로 1(Integer) 값을 사용한다.
 - pixelType 파라미터가 Null이면 기본값으로 Integer를 사용한다.
 - pixelType 파라미터는 BYTE, SHORT, INTEGER, FLOAT, DOUBLE 값을 사용할 수 있다.
 - extent 파라미터를 설정하지 않으면 inputGeometry의 범위를 사용한다.
 - cellSize 파라미터를 설정하지 않으면 Extent의 Width와 Height 중 작은 값을 250으로 나눈 값을 사용한다.

**Examples**
