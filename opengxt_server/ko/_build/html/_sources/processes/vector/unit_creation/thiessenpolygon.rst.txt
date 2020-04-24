.. _thiessenpolygon:

티센(Thiessen) 폴리곤
================================================

포인트 레이어를 이용하여 티센(Thiessen) 폴리곤을 생성합니다.

**Syntax**

ThiessenPolygon (SimpleFeatureCollection inputFeatures, ThiessenAttributeMode attributes, Geometry clipArea) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 티센 폴리곤을 생성할 입력 포인트 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - attributes
     - 속성 모드 : ONLY_FID(기본값), ALL(입력 레이어의 모든 속성값을 유지합니다).
     - ThiessenAttributeMode
     - OnlyFID
     -

   * - clipArea
     - 잘라낼 영역 폴리곤입니다.
     - Geometry
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
     - 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - attributes: OnlyFID(기본값), All
 - inputFeatures는 포인트, 라인, 폴리곤 모두 가능하지만, 무게중심점을 추출하여 Thiessen Polygon을 생성한다.
 - Attributes 파라미터가 ALL 인 경우 inputFeatures의 모든 속성값을 유지한다.
 - clipArea 파라미터가 주어지면 해당 영역으로 클립한 폴리곤을 반환한다.


**Examples**
