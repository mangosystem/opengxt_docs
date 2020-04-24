.. _localrogersonr:

Rogerson의 국지적 R 통계량
=========================================================

Rogerson의 국지적 R 통계량을 계산합니다.

**Syntax**

LocalRogersonR (SimpleFeatureCollection inputFeatures, String xField, String yField, DistanceMethod distanceMethod, Double kappa) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 통계량을 계산할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - xField
     - 수치형 입력 변수 X 필드 변수를 설정합니다.
     - String
     -
     - ✓

   * - yField
     - 수치형 입력 변수 Y 필드 변수를 설정합니다.
     - String
     -
     - ✓

   * - distanceMethod
     - 분석 대상 피처로부터 이웃 피처까지의 거리를 계산하는 방법을 설정합니다.
     - DistanceMethod
     - Euclidean
     -

   * - kappa
     - 거리에 대한 중요도를 설정합니다.
     - Double
     - 1.0
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
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - distanceMethod: Euclidean(기본값), Manhattan

**Examples**
