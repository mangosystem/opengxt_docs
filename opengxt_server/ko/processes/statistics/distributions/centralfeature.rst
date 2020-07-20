.. _centralfeature:

중심 피처 찾기
========================

입력 피쳐들의 지리적 중심점에 가장 가까운 피처를 반환합니다.

**Syntax**

CentralFeature (SimpleFeatureCollection inputFeatures, DistanceMethod distanceMethod, String weightField, String selfPotentialWeightField, String caseField) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 중심 피처를 찾는데 사용될 입력 피처 레이어를 설정합니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - distanceMethod
     - 분석 대상 피처로부터 이웃 피처까지의 거리를 계산하는 방법을 설정합니다.
     - DistanceMethod
     - Euclidean
     -

   * - weightField
     - 가중평균 중심점을 생성하는데 사용될 필드를 설정합니다.
     - String
     -
     -

   * - selfPotentialWeightField
     - 자기 자신과 다른피처와의 거리 또는 가중치 값을 나타내는 필드를 설정합니다.
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

 - distanceMethod: Euclidean(기본값), Manhattan
 - inputFeatures의 Centroid를 이용하여 계산한다.

**Examples**

서울시 아파트 분포에 대한 시군구별 Central Feature를 분석한 결과입니다.

  .. image:: images/centralfeature.png
