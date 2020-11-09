.. _linedensity:

라인 밀도분석
=====================

설정한 탐색반경을 이용하여 라인 피처에 대한 밀도분석을 수행합니다.

**Syntax**

LineDensity (SimpleFeatureCollection inputFeatures, String populationField, Double searchRadius, Double cellSize, ReferencedEnvelope extent) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 밀도를 계산할 라인 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - populationField
     - 각 피처에 대한 모집단 값을 나타내는 필드입니다.
     - String
     -
     -

   * - searchRadius
     - 밀도를 계산할 탐색 반경입니다.
     - Double
     - 0.0
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
     - 출력 밀도 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - searchRadius 파라미터를 설정하지 않으면 Extent의 Width와 Height 중 작은 값을 30으로 나눈 값을 사용한다.
 - extent 파라미터를 설정하지 않으면 inputFeatures 레이어의 범위를 사용한다.
 - cellSize 파라미터를 설정하지 않으면 Extent의 Width와 Height 중 작은 값을 250으로 나눈 값을 사용한다.


**Examples**

  .. image:: images/linedensity.png
