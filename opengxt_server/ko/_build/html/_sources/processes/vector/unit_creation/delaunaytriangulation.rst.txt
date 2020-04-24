.. _delaunaytriangulation:

델라니 삼각망(Delaunay Triangulation)
=============================================================================================

포인트 레이어로부터 델라니 삼각망(Delaunay Triangulation)을 생성합니다.

**Syntax**

DelaunayTriangulation (SimpleFeatureCollection inputFeatures, Geometry clipArea) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 델라니 삼각망을 구성할 입력 포인트 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - clipArea
     - 델라니 삼각망을 구성 후 잘라낼 폴리곤 영역을 설정합니다.
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
     - 델라니 삼각망을 포함한 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - clipArea 파라미터가 주어지면 해당 영역으로 클립한 폴리곤을 반환한다.

**Examples**
