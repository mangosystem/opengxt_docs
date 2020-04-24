.. _identity:

아이덴터티
===============

두 레이어간의 아이덴터티 중첩분석을 수행합니다.

**Syntax**

Identity (SimpleFeatureCollection inputFeatures, SimpleFeatureCollection identityFeatures) : SimpleFeatureCollection

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

   * - identityFeatures
     - 아이덴터티 레이어입니다.
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
     - 출력 레이어
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures, identityFeatures는 반드시 Polygon 또는 MultiPolygon 피처 타입이어야 한다.
 - 출력 레이어는 inputFeatures, identityFeatures의 필드값을 모두 포함한다.


**Examples**
