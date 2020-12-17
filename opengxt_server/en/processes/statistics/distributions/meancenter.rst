.. _meancenter:

평균중심점 생성
========================

입력 피쳐들의 지리적 중심점을 산출합니다.

**Syntax**

MeanCenter (SimpleFeatureCollection inputFeatures, String weightField, String caseField, String dimensionField) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 평균중심점을 계산하는데 사용될 입력 피처 레이어를 설정합니다.
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

   * - dimensionField
     - 속성 값의 평균을 계산할 필드를 설정합니다.
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

서울시 아파트 분포에 대한 시군구별 Mean Center를 분석한 결과입니다.

  .. image:: images/meancenter.png
