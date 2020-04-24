.. _clipwithgeometry:

폴리곤 지오메트리로 잘라내기
=============================================

잘라낼 폴리곤 지오메트리와 중첩하는 입력 피처를 잘라냅니다.

**Syntax**

ClipWithGeometry (SimpleFeatureCollection inputFeatures, Geometry clipGeometry) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 입력 레이어.
     - SimpleFeatureCollection
     -
     - ✓

   * - clipGeometry
     - 잘라낼 폴리곤 지오메트리입니다.
     - Geometry
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
     - 출력 레이어.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - clipGeometry는 반드시 Polygon 또는 MultiPolygon이어야 한다.

**Examples**
