.. _tininterpolation:

Triangulated Irregular Network(TIN) 보간
===========================================================================

입력 피처에 대해 Triangulated Irregular Network(TIN) (TPS) 보간법을 적용한 래스터를 생성합니다.

**Syntax**

TINInterpolation (SimpleFeatureCollection inputFeatures, Expression inputField, RasterPixelType pixelType, Double cellSize, ReferencedEnvelope extent) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 보간할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - inputField
     - 각각의 샘플 포인트에 대한 높이 또는 크기 등 값을 포함한 필드입니다.
     - Expression
     -
     - ✓

   * - pixelType
     - 출력 래스터 레이어의 픽셀 유형입니다.
     - RasterPixelType
     - Float
     -

   * - cellSize
     - 출력 래스터 레이어의 셀 크기입니다.
     - Double
     - 0.0
     -

   * - extent
     - 출력 래스터 레이어의 공간 범위입니다.
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
     - 보간한 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

- pixelType: BYTE, SHORT, INTEGER, FLOAT(기본값), DOUBLE
- extent 파라미터를 설정하지 않으면 inputFeatures 레이어의 범위를 사용한다.
- cellSize 파라미터를 설정하지 않으면 Extent의 Width와 Height 중 작은 값을 250으로 나눈 값을 사용한다.
- 입력 레이어가 라인스트링, 폴리곤인 경우 모든 버텍스를 추출하여 보간에 사용한다.

**Examples**

  .. image:: images/tininterpolation.png
