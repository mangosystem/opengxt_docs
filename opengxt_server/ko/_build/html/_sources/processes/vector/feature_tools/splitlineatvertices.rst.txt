.. _splitlineatvertices:

라인을 세그먼트로 분할
====================================

라인/폴리곤 피처의 각 버텍스별(라인 세그먼트)로 분할한 라인을 생성합니다.

**Syntax**

SplitLineAtVertices (SimpleFeatureCollection lineFeatures) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - lineFeatures
     - 세그먼트별로 분할할 라인 또는 폴리곤 레이어입니다.
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
     - 세그먼트로 분할한 출력 라인 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures 파라미터는 라인 또는 폴리곤 레이어 이어야 한다. 

**Examples**
