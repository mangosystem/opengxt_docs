.. _intersect:

인터섹트
============

두 레이어간의 인터섹트 중첩분석을 수행합니다. 두 레이어의 속성값은 유지됩니다.

**Syntax**

Intersect (SimpleFeatureCollection inputFeatures, SimpleFeatureCollection overlayFeatures) : SimpleFeatureCollection

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

   * - overlayFeatures
     - 인터섹트할 중첩 레이어입니다.
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

 - 입력 피처 레이어는 Point, Line, Polygon모두 가능하며, 출력 레이어의 피처 타입은 inputFeatures 레이어를 따른다.
 - 출력 레이어는 inputFeatures, overlayFeatures의 필드값을 모두 포함한다.


**Examples**

두 폴리곤 레이어간 Intersect Overlay 분석을 수행한 결과입니다. 두 레이어의 속성값을 모두 포함합니다.

  .. image:: images/intersect.png
