.. _rasterhillshade:

음영기복도 생성
========================

DEM 래스터 데이터를 이용하여 음영기복도를 생성합니다.

**Syntax**

RasterHillshade (GridCoverage2D inputCoverage, Double azimuth, Double altitude, Double zFactor) : GridCoverage2D

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

   * - azimuth
     - 태양광에 대한 수평(방위) 각입니다. 기본값은 315도입니다.
     - Double
     - 315.0
     -

   * - altitude
     - 태양광의 수직(고도) 각입니다. 기본값은 45 도입니다.
     - Double
     - 45.0
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
     - 음영기복도 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - azimuth 파라미터의 값은 0도에서 360도까지 북쪽에서 시계방향으로 측정한 태양의 각 방향이다. 기본 방위각은 315도 (NW)를 사용한다.
 - altitude 파라미터는 수평선 위에서의 태양의 조도값으로 0 (수평선)에서 90 (수직)까지의 값을 사용한다. 기본 고도값은 45도를 사용한다.
 - 좌표체계의 x, y단위와 z값의 단위가 다르면 zFactor값을 x, y 단위로 적절하게 환산해서 설정한다.

**Examples**

  .. image:: images/rasterhillshade.png
