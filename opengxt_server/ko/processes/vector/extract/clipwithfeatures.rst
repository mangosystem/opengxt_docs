.. _clipwithfeatures:

폴리곤 피처로 잘라내기
====================================

클립 폴리곤 피처와 중첩하는 입력 피처를 잘라냅니다.

**Syntax**

ClipWithFeatures (SimpleFeatureCollection inputFeatures, SimpleFeatureCollection clipFeatures) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 입력 피처 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - clipFeatures
     - 입력 피처 레이어를 클립할 폴리곤 레이어입니다.
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
     - 출력 레이어.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - clipFeatures는 반드시 Polygon 또는 MultiPolygon 피처 타입이어야 한다.

**Examples**

임의의 폴리곤 레이어를 이용하여 읍면동경계 폴리곤 레이어를 clip한 예입니다.

  .. image:: images/clipwithfeatures.png
