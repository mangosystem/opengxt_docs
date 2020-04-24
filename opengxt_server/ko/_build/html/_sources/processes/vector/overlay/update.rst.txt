.. _update:

업데이트
============

두 레이어간의 업데이트 중첩분석을 수행합니다. 업데이트 피처와 중첩되는 입력 피처는 업데이트 피처로 대체됩니다.

**Syntax**

Update (SimpleFeatureCollection inputFeatures, SimpleFeatureCollection updateFeatures) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 입력 폴리곤 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - updateFeatures
     - 업데이트할 폴리곤 레이어 입니다.
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
     - 업데이트 한 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures, identityFeatures는 반드시 Polygon 또는 MultiPolygon 피처 타입이어야 한다.
 - 출력 레이어는 inputFeatures, updateFeatures의 필드값을 모두 포함한다.


**Examples**
