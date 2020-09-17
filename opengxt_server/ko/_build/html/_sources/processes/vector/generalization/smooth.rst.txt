.. _smooth:

곡선화
==================

라인 또는 폴리곤 레이어의 도형을 부드럽게 합니다. 곡선화 알고리즘은 베이지어 스플라인을 사용하여 라인 상에서 버텍스를 삽입합니다.

**Syntax**

Smooth (SimpleFeatureCollection features, Double fit): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - features
     - 곡선화를 적용할 입력 라인 또는 폴리곤 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - fit
     - 스무딩된 경계(0은 느슨)의 적합성을 지정하는 0과 1(포함) 사이의 값입니다.
     - Double
     - 0.3
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

 - fit 파라미터는 0과 1 사이의 Double값을 사용한다.


**Examples**

빨간선은 원본, 파란선은 Smooth 결과 입니다.

  .. image:: images/smooth.png
