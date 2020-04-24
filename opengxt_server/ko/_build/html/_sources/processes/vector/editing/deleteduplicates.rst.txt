.. _deleteduplicates:

중복 피처 삭제
========================

중복(지오메트리가 동일)된 피처를 찾아서 제거합니다.

**Syntax**

DeleteDuplicates (SimpleFeatureCollection inputFeatures) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 중복 피처를 제거할 입력 레이어입니다.
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
     - 중복 피처가 삭제된 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures는 포인트, 라인, 폴리곤 모두 가능하며, 각 피처의 Geometry가 동일한 경우에만 중복으로 처리한다. 

**Examples**
