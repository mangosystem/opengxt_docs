.. _rastercurvature:

지표 곡률 분석
========================

 DEM 래스터 데이터를 이용하여 지표면의 곡률을 계산합니다.

**Syntax**

RasterCurvature (GridCoverage2D inputCoverage, Double zFactor) : GridCoverage2D

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

   * - zFactor
     - Z(고도) 단위의 측정 단위가 x, y(선형) 단위의 측정 단위와 같은 경우 Z 계수는 1이지만, 서로 다른 경우 정확한 값 산출을 위해 이 값을 조정해야 합니다.
     - Double
     - 1.0
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

 - 좌표체계의 x, y단위와 z값의 단위가 다르면 zFactor값을 x, y 단위로 적절하게 환산해서 설정한다.

**Examples**
