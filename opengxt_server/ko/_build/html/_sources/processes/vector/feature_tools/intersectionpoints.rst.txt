.. _intersectionpoints:

라인 피처들의 교차점 생성
==========================================

두 라인 피처 레이어와 교차되는 지점을 포인트로 생성합니다. 입력 피처의 속성은 유지되며 교차되는 피처의 ID값을 유지할 수 있습니다.

**Syntax**

IntersectionPoints (SimpleFeatureCollection inputFeatures, SimpleFeatureCollection intersectFeatures, String intersectIDField) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 라인 또는 폴리곤 유형의 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - intersectFeatures
     - 라인 또는 폴리곤 유형의 교차 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - intersectIDField
     - 교차된 피처의 ID가 저장될 필드를 설정합니다.
     - String
     -
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
     - 두 레이어의 교차점 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures, intersectFeatures피처 레이어는 Line, Polygon모두 가능하다.
 - 출력 레이어는 inputFeatures의 필드값을 모두 포함하며, intersectIDField가 설정된 경우 intersectFearures의 값이 추가된다.


**Examples**
