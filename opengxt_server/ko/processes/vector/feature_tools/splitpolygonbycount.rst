.. _splitpolygonbycount:

개수 또는 표현식으로 폴리곤을 분할
=========================================================

설정한 개수(값, 필드, 표현식)에 따라 분할한 폴리곤 피처를 생성합니다.

**Syntax**

SplitPolygonByCount (SimpleFeatureCollection polygonFeatures, Expression count) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - polygonFeatures
     - 분할할 폴리곤 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - count
     - 개수를 표현하는 숫자, 필드 또는 계산식을 설정합니다. 예) 10 또는 필드 또는 area2( [geom] ) / 10.
     - Expression
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
     - 분할한 출력 폴리곤 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - polygonFeatures 파라미터는 폴리곤 레이어 이어야 한다.
 - count 파라미터는 숫자, 필드 또는 숫자값을 결과로 반환하는 Function Expression 수식을 사용할 수 있다.

**Examples**

폴리곤 피처의 boundary를 100미터 간격의 라인으로 분할한 결과입니다.

  .. image:: images/splitpolygonbycount.png

