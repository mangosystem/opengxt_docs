.. _randompoints:

랜덤 포인트 생성
===========================

직사각형 또는 폴리곤 영역으로 랜덤 포인트를 생성합니다

**Syntax**

RandomPoints (ReferencedEnvelope extent, SimpleFeatureCollection polygonFeatures, Integer pointCount) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - extent
     - 랜덤 포인트가 생성될 영역입니다
     - ReferencedEnvelope
     -
     - ✓

   * - polygonFeatures
     - 랜덤 포인트가 생성될 폴리곤 레이어입니다.
     - SimpleFeatureCollection
     -
     -

   * - pointCount
     - 생성할 포인트의 갯수입니다.
     - Integer
     - 1000
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
     - 랜덤 포인트 피처컬렉션
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - BoundingBox 또는 폴리곤 레이어를 기준 레이어로 사용할 수 있다.

**Examples**
