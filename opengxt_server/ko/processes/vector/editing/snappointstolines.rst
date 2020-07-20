.. _snappointstolines:

포인트를 라인에 스냅
=================================

사용자가 설정한 스냅 거리와 가장 가까운 라인 피처에 포인트 피처를 스냅합니다.

**Syntax**

SnapPointsToLines (SimpleFeatureCollection pointFeatures, SimpleFeatureCollection lineFeatures, Double tolerance) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - pointFeatures
     - 스냅할 포인트 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - lineFeatures
     - 스냅 대상 라인 또는 폴리곤(경계 라인만 사용) 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - tolerance
     - 스냅 허용 거리입니다. 만약 허용 거리가 0이면, 가장 가까운 라인이 스냅에 사용됩니다.
     - Double
     - 0.0
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
     - 스냅한 출력 포인트 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - lineFeatures 레이어는 라인 또는 폴리곤 타입 이어야 한다.
 - tolerance 파라미터가 0인 경우 가장 가까운 라인 피처로 이동하며, pointFeatures의 거리 단위를 사용한다.

**Examples**

도로 주변의 포인트를 가장 가까운 도로(라인)에 스냅한 결과입니다.

  .. image:: images/snappointstolines.png
