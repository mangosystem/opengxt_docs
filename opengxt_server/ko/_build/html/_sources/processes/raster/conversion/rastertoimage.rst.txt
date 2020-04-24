.. _rastertoimage:

래스터를 이미지로 변환
====================================

OGC WMS 인터페이스처럼 래스터 레이어와 지도 이미지 생성에 필요한 파라미터를 입력하여 지도 이미지를 생성합니다.

**Syntax**

RasterToImage (GridCoverage2D coverage, String bbox, CoordinateReferenceSystem crs, Style style, Integer width, Integer height, String format, Boolean transparent, String bgColor) : MapToImageParam

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - coverage
     - 이미지로 변환할 입력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - bbox
     - 이미지를 생성할 좌하단과 우상단의 좌표값 영역입니다. minx,miny,maxx,maxy.
     - String
     -
     -

   * - crs
     - 이미지 영역 설정에 대한 좌표체계입니다.
     - CoordinateReferenceSystem
     -
     -

   * - style
     - 래스터 심볼라이저를 포함한 Styled Layer Descriptor (SLD)입니다. 스타일을 설정하지 않으면 내부에서 지정된 스타일을 사용하여 이미지를 생성합니다.
     - Style
     -
     -

   * - width
     - 이미지의 너비를 설정합니다.
     - Integer
     -
     - ✓

   * - height
     - 이미지의 높이를 설정합니다.
     - Integer
     -
     - ✓

   * - format
     - 이미지 포맷입니다.  image/jpeg, image/png, image/gif 를 사용할 수 있습니다.
     - String
     - image/png
     -

   * - transparent
     - 지도 배경색을 투명하게 처리할 지 여부를 설정합니다. 기본값은 예(True)이며 투명 배경을 지원하는 이미지 포맷이어야 합니다.
     - Boolean
     - true
     -

   * - bgColor
     - 생성할 이미지의 배경 색상을 설정합니다. 기본값은 0xFFFFFF (흰색).
     - String
     - 0xFFFFFF
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
     - 출력 이미지입니다.
     - MapToImageParam
     -
     - ✓

**Constraints**

 - bbox와 crs 파라미터가 Null인 경우 coverage의 Extent와 좌표체계를 사용한다.
 - style 파라미터가 Null인 경우 최소/최대값을 이용한 Equal Interval Style을 적용한다.


**Examples**
