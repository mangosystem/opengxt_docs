.. _mediancenter:

중앙값중심점 생성
===========================

각 피처에 대한 전체 유클리드 거리를 최소화하는 위치의 중심점을 생성합니다.

**Syntax**

MedianCenter (SimpleFeatureCollection inputFeatures, String weightField, String caseField, String attributeFields) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 중앙값중심점을 계산하는데 사용될 입력 피처 레이어를 설정합니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - weightField
     - 가중평균 중심점을 생성하는데 사용될 필드를 설정합니다.
     - String
     -
     -

   * - caseField
     - 그룹별 중심을 적용하는 경우 그룹을 구분하는데 사용되는 필드를 설정합니다.
     - String
     -
     -

   * - attributeFields
     - 중앙값을 계산할 (쉼표로 구분된) 숫자 필드 또는 목록입니다.
     - String
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
     - 저장할 결과 포인트 레이어를 설정합니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures의 Centroid를 이용하여 계산한다.

**Examples**
