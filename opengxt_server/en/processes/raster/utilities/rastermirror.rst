.. _rastermirror:

미러
======

래스터의 중심을 기준으로 세로 축을 따라 왼쪽에서 오른쪽으로 래스터의 방향을 바꿉니다.

**Syntax**

RasterMirror (GridCoverage2D inputCoverage) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 변환할 입력 래스터 레이어입니다.
     - GridCoverage2D
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
     - 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - Multi-Band래스터를 지원한다.


**Examples**

  .. image:: images/rastermirror.png
