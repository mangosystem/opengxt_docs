.. _rastertri:

Terrain Ruggedness Index
========================================================================

DEM 래스터 데이터를 이용하여 TRI(지형 험상 지수, Terrain Ruggedness Index)를 추출합니다. TRI는 중앙 셀과 주변 셀의 차이값을 평균한 값입니다.

**Syntax**

RasterTRI (GridCoverage2D inputCoverage) : GridCoverage2D

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
     - TRI(지형 험상 지수)값이 계산된 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**


**Examples**

  .. image:: images/rastertri.png
