.. _kmeansclustering:

K- 평균 군집화
===========================

K- 평균 군집화를 수행합니다.

**Syntax**

KMeansClustering (SimpleFeatureCollection inputFeatures, String targetField, Integer numberOfClusters, Boolean asCircle) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 군집화할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - targetField
     - 군집화 ID가 저장될 숫자 필드를 설정합니다.
     - String
     - cluster
     - ✓

   * - numberOfClusters
     - 그룹별로 군집화 할 수 를 설정합니다.
     - Integer
     - 5
     - ✓

   * - asCircle
     - 군집화 결과를 원 폴리곤으로 출력합니다.
     - Boolean
     - false
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
     - 군집화 결과가 속성으로 저장된 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - targetField 파라미터를 설정하지 않으면 기본값 cluster 필드를 사용한다.
 - numberOfClusters 파라미터를 설정하지 않으면 기본값 5를 사용한다.


**Examples**
