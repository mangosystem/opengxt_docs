.. _countfeatures:

피처 수 계산
=====================

피처 레이어의 피처 수를 계산합니다.

**Syntax**

CountFeatures (SimpleFeatureCollection inputFeatures, Filter filter) : Integer

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 계산할 입력 레이어.
     - SimpleFeatureCollection
     -
     - ✓

   * - filter
     - 필터 표현식
     - Filter
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
     - 피처 수
     - Integer
     -
     - ✓

**Constraints**

 - 레이어와 필터를 이용하여 피처의 수를 계산하여 반환한다.

**Examples**

설정한 필터 표현식과 일치하는 피처의 개수를 Integer 값으로 반환합니다.
