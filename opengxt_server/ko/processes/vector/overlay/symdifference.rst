.. _symdifference:

대칭 차집합
==================

두 레이어간의 대칭 차집합 중첩분석을 수행합니다. 두 레이어의 속성값은 유지됩니다.

**Syntax**

SymDifference (SimpleFeatureCollection inputFeatures, SimpleFeatureCollection differenceFeatures) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - differenceFeatures
     - 대칭 차집합에 사용할 중첩 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

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

 - 입력 레이어는 폴리곤 피처 타입이어야 하며, 출력 레이어의 피처 타입은 inputFeatures 레이어를 따른다.
 - 출력 레이어는 inputFeatures, differenceFeatures의 속성값을 모두 포함한다.


**Examples**
