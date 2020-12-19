.. _multiwindrosemap:

다중 Wind Rose Map 생성
================================================

피처의 중심으로부터 Wind Rose Map을 생성합니다.

**Syntax**

MultiWindRoseMap (SimpleFeatureCollection inputFeatures, String weightFields, SimpleFeatureCollection centerFeatures, Geometry centerPoint, Double searchRadius, Integer roseCount): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 포인트, 라인, 폴리곤 유형의 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - weightFields
     - 숫자값의 가중치 필드입니다.
     - String
     -
     -

   * - centerFeatures
     - Wind Rose의 중심점 피처 레이어입니다.
     - SimpleFeatureCollection
     -
     -

   * - centerPoint
     - Wind Rose의 중심점 지오메트리입니다.
     - Geometry
     -
     -

   * - searchRadius
     - 최대 탐색 반경입니다.
     - Double
     -
     -

   * - roseCount
     - 탐색방향의 수입니다.
     - Integer
     - 36
     - ✓

**Process Outputs**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - anchor
     - 반경을 표시하는 지시선 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - windRose
     - 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - weightFields 파라미터는 Numeric 필드이어야 하며, 설정되면 이 필드 값의 합이 결과에 반영되고 그렇지 않으면 피처의 개수가 반영된다.
 - Output은 지시선을 표시하는 anchor 라인과 windRose 폴리곤 레이어를 반환한다.

**Examples**

Multiple Wind Rose Map을 생성한 예입니다.

  .. image:: images/multiwindrosemap.png
