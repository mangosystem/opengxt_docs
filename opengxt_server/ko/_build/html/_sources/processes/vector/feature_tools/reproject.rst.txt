.. _reproject:

좌표체계 변환
=====================

벡터 레이어를 새로운 좌표체계로 변환합니다.

**Syntax**

Reproject (SimpleFeatureCollection inputFeatures, CoordinateReferenceSystem forcedCRS, CoordinateReferenceSystem targetCRS) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 좌표체계를 변환할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - forcedCRS
     - 입력 레이어의 좌표체계를 정의합니다. 입력 레이어의 좌표체계가 설정된 경우에도 이 좌표체계로 재정의하여 좌표변환을 수행합니다.
     - CoordinateReferenceSystem
     -
     -

   * - targetCRS
     - 이 좌표체계로 원본 입력 레이어의 좌표체계를 변환합니다.
     - CoordinateReferenceSystem
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
     - 좌표체계를 변환한 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - targetCRS가 Null인 경우 inputFeatures를 반환한다.
 - forcedCRS가 Null인 경우 inputFeatures의 CRS를 사용하고, 만일 inputFeatures의 좌표체계가 정의되어 있지 않으면 inputFeatures를 반환한다.
