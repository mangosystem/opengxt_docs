.. _rastershift:

위치 이동
===============

x, y의 이동 값에 따라 래스터를 새로운 지리적 위치로 이동합니다.

**Syntax**

RasterShift (GridCoverage2D inputCoverage, Double xShift, Double yShift) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 변환에 사용될 입력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - xShift
     - X축 방향의 이동값을 설정합니다. -값이면 왼쪽, +값이면 오른쪽으로 이동합니다.
     - Double
     - 0.0
     -

   * - yShift
     - Y축 방향의 이동값을 설정합니다. -값이면 아래쪽, +값이면 위쪽으로 이동합니다.
     - Double
     - 0.0
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
     - X, Y 방향으로 이동한 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - Multi-Band래스터를 지원한다.
 - xShift, yShift 값의 단위는 입력 래스터 좌표체계의 거리 단위를 사용한다.
 - xShift 파라미터의 값이 0보다 크면 오른쪽, 작으면 왼쪽으로 이동한다.
 - yShift 파라미터의 값이 0보다 크면 위쪽, 작으로 아래쪽으로 이동한다.


**Examples**
