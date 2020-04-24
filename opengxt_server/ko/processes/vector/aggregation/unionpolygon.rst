.. _unionpolygon:

폴리곤 합치기
=====================

폴리곤 레이어의 모든 피처를 유니언한 레이어를 생성합니다

**Syntax**

UnionPolygon (SimpleFeatureCollection polygonFeatures, Boolean preserveHole) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - polygonFeatures
     - 유니언할 폴리곤 레이어.
     - SimpleFeatureCollection
     -
     - ✓

   * - preserveHole
     - 폴리곤의 홀을 유지하거나 제거합니다.
     - Boolean
     - true
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
     - 결과
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - preserveHole 파라미터가 False이면 모든 Interior Ring은 제거한 폴리곤을 반환한다.

**Examples**
