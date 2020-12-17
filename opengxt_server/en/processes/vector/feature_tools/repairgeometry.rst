.. _repairgeometry:

지오메트리 오류 수정
=================================

각 피처의 지오메트리 오류를 검사하고 수정합니다.

**Syntax**

RepairGeometry (SimpleFeatureCollection inputFeatures) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 지오메트리의 오류를 수정할 입력 레이어입니다.
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

 - Null 지오메트리, self-intersection 확인 및 수정
 - 좌표 유효성 검증 coordinates
 - 빈 shell/holes 처리
 - 중복 버텍스 및 포인트 수정
