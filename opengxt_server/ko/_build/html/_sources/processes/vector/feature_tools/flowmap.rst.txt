.. _flowmap:

라인 피처에서 Flow Map 생성
=========================================================

시-종점 속성을 가진 라인 피처에서 Flow Map 폴리곤 피처를 생성합니다.

**Syntax**

FlowMap (SimpleFeatureCollection lineFeatures, Expression odValue, Expression doValue, Double maxSize) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - lineFeatures
     - 시-종점 구간으로 구성된 라인 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - odValue
     - 시점-종점 표현식입니다. 예)  [field] 또는 [field] * 0.5 등...
     - Expression
     -
     - ✓

   * - doValue
     - 종점-시점 표현식입니다. 예)  [field] 또는 [field] * 0.5 등...
     - Expression
     -
     -

   * - maxSize
     - Flow Map 생성시 사용할 최대 화살표의 크기를 설정합니다.
     - Double
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
     - Flow Map 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - lineFeatures 파라미터는 라인 레이어 이어야 한다.
 - maxSize 파라미터가 Null 또는 0이면 lineFeatures의 Extent의 넓이와 높이 중 작은값을 20으로 나눈 값을 사용한다.


**Examples**
