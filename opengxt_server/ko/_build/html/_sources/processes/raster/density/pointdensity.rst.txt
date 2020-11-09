.. _pointdensity:

포인트 밀도분석
========================

포인트 피처에 대해 설정한 이웃 정의 방식을 이용하여 밀도분석을 수행합니다.

**Syntax**

PointDensity (SimpleFeatureCollection inputFeatures, String populationField, String neighborhood, Double cellSize, ReferencedEnvelope extent) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 밀도를 계산할 입력 포인트 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - populationField
     - 각 피처에 대한 모집단 값을 나타내는 필드입니다.
     - String
     -
     -

   * - neighborhood
     - 주변 탐색 방법을 정의합니다: Circle + Radius, Rectangle + width + height, default = Circle + Radius(입력 레이어의 범위 중 작은 값을 30으로 나눈 값을 기본값으로 사용합니다)
     - String
     -
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
     - 밀도값이 계산된 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - neighborhood 파라미터를 설정하지 않으면 Circle + 반경(inpueFeatures의 Extent의 Width와 Height 중 작은 값을 30으로 나눈 값)을 사용한다.
 - extent 파라미터를 설정하지 않으면 inputFeatures 레이어의 범위를 사용한다.
 - cellSize 파라미터를 설정하지 않으면 Extent의 Width와 Height 중 작은 값을 250으로 나눈 값을 사용한다.


**Examples**

  .. image:: images/pointdensity.png
