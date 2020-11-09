.. _rasterprofile:

래스터 단면도 분석
==============================

래스터에서 보간된 z 값을 포함하는 포인트 피처를 생성합니다.

**Syntax**

RasterProfile (GridCoverage2D inputCoverage, Geometry userLine, Double interval) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 단면도를 측정할 입력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - userLine
     - 단면도 측정에 사용할 라인스트링 또는 멀티라인스트링 지오메트리입니다.
     - Geometry
     -
     - ✓

   * - interval
     - 단면도를 측정할 거리 간격입니다. 기본 거리 = 지오메트리의 길이 / 20.
     - Double
     - 20.0
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
     - 출력 레이어
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - interval 파라미터가 설정되지 않으면 userLine 길이를 20으로 나눈 값을 적용한다.
 - Output 포인트 레이어는 distance(누적 거리)와 value(높이값 등 래스터의 셀 값) 필드를 포함한다.

**Examples**

  .. image:: images/rasterprofile.png
