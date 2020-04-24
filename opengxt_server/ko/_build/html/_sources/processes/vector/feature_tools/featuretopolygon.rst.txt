.. _featuretopolygon:

피처를 폴리곤으로 변환
====================================

입력된 라인 또는 폴리곤 피처에서 닫힌 모든 폴리곤 피처를 생성합니다.

**Syntax**

FeatureToPolygon (SimpleFeatureCollection inputFeatures, Double tolerance, SimpleFeatureCollection labelFeatures) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 폴리곤을 생성할 입력 라인 또는 폴리곤 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - tolerance
     - 허용 오차. 기본값은 0.001 레이어 좌표체계 단위입니다.
     - Double
     - 0.001
     -

   * - labelFeatures
     - 출력 폴리곤 레이어에 속성을 추가할 입력 포인트 레이어입니다.
     - SimpleFeatureCollection
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
     - 출력 레이어
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures 레이어는 라인 또는 폴리곤 타입이어야 한다.
 - tolerance 파라미터의 기본값은 0.001이며, inputFeatures 좌표계의 단위를 사용한다.
 - labelFeatures 레이어는 포인트 타입이어야 한다.
 - labelFeatures 파라미터가 Null이 아니면 이 스키마를 사용하며, 폴리곤 생성 후 폴리곤 내에 포함된 labelFeatures 포인트의 속성값을 할당한다.


**Examples**
