.. _kerneldensity:

커널 밀도분석
=====================

포인트 피처를 이용하여 설정한 커널 함수에 따른 밀도분석을 수행합니다.

**Syntax**

KernelDensity (SimpleFeatureCollection inputFeatures, KernelType kernelType, String populationField, Double searchRadius, Double cellSize, ReferencedEnvelope extent) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 커널 밀도를 계산할 포인트 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - kernelType
     - 커널 함수입니다: Binary, Cosine, Distance, Epanechnikov, Gaussian, InverseDistance, Quadratic(기본값), Quartic(biweight), Triangular, Triweight, Tricube
     - KernelType
     - Quadratic
     -

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
     - 출력 레이어의 셀 크기입니다.
     - Double
     - 0.0
     -

   * - extent
     - 출력 래스터의 분석 범위입니다.
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
     - 출력 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - kernelType: Binary, Cosine, Distance, Epanechnikov, Gaussian, InverseDistance, Quadratic(기본값), Quartic, Triangular, Triweight, Tricube
 - extent 파라미터를 설정하지 않으면 inputFeatures 레이어의 범위를 사용한다.
 - cellSize 파라미터를 설정하지 않으면 Extent의 Width와 Height 중 작은 값을 250으로 나눈 값을 사용한다.
 - searchRadius 파라미터를 설정하지 않으면 Extent의 Width와 Height 중 작은 값을 30으로 나눈 값을 사용한다.
 - 커널 함수는 `Kernel (statistics) <https://en.wikipedia.org/wiki/Kernel_%28statistics%29>`_ 참고

**Examples**

  .. image:: images/kerneldensity.png
