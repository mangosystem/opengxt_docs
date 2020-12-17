.. _splitlineatpoint:

포인트로 라인 분할
==============================

포인트와 교차 또는 일정 거리 이상 근접한 포인트를 기준으로 라인을 분할합니다.

**Syntax**

SplitLineAtPoint (SimpleFeatureCollection lineFeatures, SimpleFeatureCollection pointFeatures, Double tolerance) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - lineFeatures
     - 분할할 라인 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - pointFeatures
     - 라인 레이어를 분할하는 데 사용되는 포인트 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - tolerance
     - 탐색 반경입니다. 거리가 0인 경우, 선과 가장 가까운 포인트가 라인을 분할하는데 사용됩니다.
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
     - 분할한 출력 라인 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures 파라미터는 라인 레이어 이어야 한다.
 - toleralce 파라미터가 0인 경우 각 라인 피처와 교차되는 모든 포인트가 사용되며, 만약 교차되는 포인트 피처가 없는 경우 가장 가까운 한개의 포인트 피처가 라인 분할에 사용된다.
 - toleralce 파라미터가 0 이상인 경우에 탐색 반경 내의 모든 포인트 피처가 분할에 사용된다.

**Examples**

라인 레이어를 포인트 레이어로 분할한 결과입니다.

  .. image:: images/splitlineatpoint.png
