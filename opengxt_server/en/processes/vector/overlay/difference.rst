.. _difference:

차집합
=========

두 레이어간의 차집합 중첩분석을 수행합니다. 입력 레이어의 속성값만 유지됩니다.

**Syntax**

Difference (SimpleFeatureCollection inputFeatures, SimpleFeatureCollection differenceFeatures) : SimpleFeatureCollection

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
     - 차집합에 사용할 중첩 레이어입니다.
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

 - 출력 레이어의 피처 타입과 필드는 inputFeatures 레이어를 따른다.

**Examples**

두 폴리곤 레이어간 Difference Overlay 분석을 수행한 결과입니다.

  .. image:: images/difference.png
