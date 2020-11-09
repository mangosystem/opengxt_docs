.. _rasterslope:

경사도 분석
==================

DEM 래스터 데이터를 이용하여 경사도 분석을 수행합니다.

**Syntax**

RasterSlope (GridCoverage2D inputCoverage, SlopeType slopeType, Double zFactor) : GridCoverage2D

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

   * - slopeType
     - 경사도 측정 단위를 설정합니다. Degree(도, 기본값), Percentrise(퍼센트).
     - SlopeType
     - Degree
     -

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
     - 경사도가 계산된 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - slopeType: Degree(기본값), Percentrise
 - slopeType 파라미터는 Degree 또는 Percentrise 값을 사용하며, Null이면 Degree 값을 적용한다.
 - 좌표체계의 x, y단위와 z값의 단위가 다르면 zFactor값을 x, y 단위로 적절하게 환산해서 설정한다.

**Examples**

  .. image:: images/rasterslope.png
