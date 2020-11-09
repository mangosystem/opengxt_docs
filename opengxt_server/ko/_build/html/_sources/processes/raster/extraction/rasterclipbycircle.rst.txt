.. _rasterclipbycircle:

원으로 래스터 추출
==============================

중심점과 반경으로 래스터를 추출합니다.

**Syntax**

RasterClipByCircle (GridCoverage2D inputCoverage, Geometry center, Double radius, Boolean inside) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 추출할 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - center
     - 추출할 영역을 설정할 원의 중심점 지오메트리입니다.
     - Geometry
     -
     - ✓

   * - radius
     - 추출할 영역을 정의하는 원의 반경입니다. 중심점 지오메트리의 좌표체계 단위를 사용합니다.
     - Double
     - 0.0
     - ✓

   * - inside
     - 입력 래스터에서 원의 내부만 추출 여부를 설저합니다. 기본값은 참(True)이며, 만약 거짓(False)일 경우 원을 제외한 외부의 래스터만 추출합니다.
     - Boolean
     - true
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

 - inside 파라미터가 False인 경우 원을 제외한 지역을 반환한다.

**Examples**

  .. image:: images/rasterclipbycircle.png
