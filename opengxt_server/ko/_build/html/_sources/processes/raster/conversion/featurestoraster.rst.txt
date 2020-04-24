.. _featurestoraster:

피처를 래스터로 변환
=================================

포인트, 라인, 폴리곤 피처 레이어를 래스터로 변환합니다.

**Syntax**

FeaturesToRaster (SimpleFeatureCollection inputFeatures, String inputField, Double cellSize, ReferencedEnvelope extent) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 래스터로 변환할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - inputField
     - 출력 래스터의 셀 값에 적용될 숫자로 변환가능한 필드입니다.
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
     - 변환된 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - inputField 파라미터는 반드시 Numeric 필드 또는 상수값이어야 한다.
 - extent 파라미터를 설정하지 않으면 inputFeatures의 범위를 사용한다.
 - cellSize 파라미터를 설정하지 않으면 Extent의 Width와 Height 중 작은 값을 250으로 나눈 값을 사용한다. 


**Examples**
