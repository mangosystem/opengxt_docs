.. _sumlinelength:

라인 길이합 계산
===========================

각각의 폴리곤 피처에 포함되는 라인을 잘라낸 후 길이합을 계산합니다.

**Syntax**

SumLineLength (SimpleFeatureCollection polygons, String lengthField, String countField, SimpleFeatureCollection lines) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - polygons
     - 폴리곤 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - lengthField
     - 값이 계산될 길이 필드입니다.
     - String
     - sum_len
     - ✓

   * - countField
     - 값이 계산될 개수 필드입니다.
     - String
     - line_cnt
     -

   * - lines
     - 라인 레이어입니다.
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

 - lengthField 는 폴리곤 피처와 중첩되는 라인들을 잘라낸 길이의 합이 저장되며, 기본값은 sum_len 이다.
 - countField 는 폴리곤 내에 포함되는 라인의 개수가 저장되며, 기본값은 line_cnt 이다.


**Examples**

시군구청에서 2000미터 내에 포함된 아파트의 수를 계산하여 지도화한 결과입니다.

  .. image:: images/sumlinelength.png
