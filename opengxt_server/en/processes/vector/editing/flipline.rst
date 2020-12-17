.. _flipline:

라인 방향 변경
========================

라인의 시점-종점 방향을 변경합니다.

**Syntax**

FlipLine (SimpleFeatureCollection lineFeatures) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - lineFeatures
     - 라인의 시작/종점을 변경할 입력 라인 레이어입니다.
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
     - 라인의 방향을 변경한 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - lineFeatures 파라미터는 라인 레이어 이어야 한다. 

**Examples**

라인의 시작/종점 방향을 변경한 결과입니다.

  .. image:: images/flipline.png
