.. _euclideandistance:

유클리드 거리 분석
==============================

입력한 피처를 이용하여 래스터 유클리드 거리 분석을 수행합니다.

**Syntax**

EuclideanDistance (SimpleFeatureCollection inputFeatures, Double maximumDistance, Double cellSize, ReferencedEnvelope extent) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 유클리드 분석을 수행할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - maximumDistance
     - 설정한 이 거리를 초과하는 지역은 거리 계산에서 제외됩니다.
     - Double
     - 1.7976931348623157E308
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
     - 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - maximumDistance 파라미터를 설정하면 설정한 거리 이상의 지역들은 No Data값을 할당한다.
 - extent 파라미터를 설정하지 않으면 inputFeatures 레이어의 범위를 사용한다.
 - cellSize 파라미터를 설정하지 않으면 Extent의 Width와 Height 중 작은 값을 250으로 나눈 값을 사용한다.

**Examples**

  .. image:: images/euclideandistance.png
