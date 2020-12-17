.. _sde:

표준 편차 타원체 생성
====================================

지리적 중심점을 기준으로 입력 레이어의 피처들이 집중되거나 분산되는 정도를 표준 편차 타원체를 생성하여 확인합니다.

**Syntax**

StandardDeviationalEllipse (SimpleFeatureCollection inputFeatures, String ellipseSize, String weightField, String caseField) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 표준편차타원체를 생성하는데 사용될 입력 피처 레이어를 설정합니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - ellipseSize
     - 표준 편차 단위의 생성할 타원체의 크기를 설정합니다. 1_STANDARD_DEVIATION(default, 또는 1), 2_STANDARD_DEVIATIONS(또는 2), 3_STANDARD_DEVIATIONS(또는 3)
     - String
     - 1_STANDARD_DEVIATION
     -

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

**Process Outputs**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - result
     - 저장할 결과 레이어를 설정합니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures의 Centroid를 이용하여 계산한다.
 - Ellipse는 일반적으로 1_Standard_Deviation인 경우 68%, 2_Standard_Deviation인 경우 95%, 3_Standard_Deviation인 경우 99%의 피처를 포함한다.

**Examples**

서울시 아파트 분포에 대한 시군구별 Standard Deviational Ellipse를 분석한 결과입니다.

  .. image:: images/sde.png
