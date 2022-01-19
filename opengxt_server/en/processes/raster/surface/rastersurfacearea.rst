.. _rastersurfacearea:

Surface Area
====================================

Calculates the surface area in polygons using DEM.

**Syntax**

RasterSurfaceArea(GridCoverage2D inputCoverage, Geometry cropShape): SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - The input surface raster to be processed.
     - GridCoverage2D
     -
     - ✓

   * - cropShape
     - The Polygon or MultiPolygon to calculate surface area.
     - Geometry
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
     - Output features.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - cropShape의 Geometry 타입은 Polygon 또는 MultiPolygon이어야 한다.
 - 출력 레이어는 area(평면 면적), surface(표면적) 필드를 포함한다.
