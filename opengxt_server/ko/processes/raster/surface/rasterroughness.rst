.. _rasterroughness:

지표의 거칠기(Roughness)
======================================================

DEM 래스터 데이터를 이용하여 거칠기(Roughness)를 추출합니다. Roughness란 표면의 불규칙성의 정도를 말하며, 중심 셀과 그 주변 셀 중 가장 큰 값을 계산합니다.

**Syntax**

RasterRoughness (GridCoverage2D inputCoverage) : GridCoverage2D

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
     - 지표의 거칠기가 계산된 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**


**Examples**

  .. image:: images/rasterroughness.png
