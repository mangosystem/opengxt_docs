.. _rasterclipbyextent:

영역으로 래스터 추출
=================================

설정한 직사각형 영역으로 래스터를 추출합니다.

**Syntax**

RasterClipByExtent (GridCoverage2D inputCoverage, ReferencedEnvelope cropShape) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 잘라낼 입력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - cropShape
     - 래스터를 잘라낼 공간 범위입니다. 설정한 범위의 좌표체계가 잘라낼 래스터 레이어의 좌표체계와 다를 경우 래스터 레이어의 좌표체계로 변환합니다.
     - ReferencedEnvelope
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
     - 잘라낸 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - Extent 파라미터는 BoundingBoxData 타입으로 다음과 같이 crs, dimensions, LowerCorner, UpperCorner로 구성된다.

  .. code-block::

    <wps:Data>
      <wps:BoundingBoxData crs="EPSG:3857" dimensions="2">
        <ows:LowerCorner>0.0 0.0</ows:LowerCorner>
        <ows:UpperCorner>1.0 1.0</ows:UpperCorner>
      </wps:BoundingBoxData>
    </wps:Data>

**Examples**

  .. image:: images/rasterclipbyextent.png
