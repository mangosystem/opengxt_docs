.. _calculatefield:

필드 계산하기
=====================

계산식에 기반하여 새로운 필드값을 계산합니다. 미리 정의된 함수를 사용하여 문자, 숫자, 지오메트리 연산을 수행할 수 있습니다.

**Syntax**

CalculateField (SimpleFeatureCollection inputFeatures, Expression expression, String fieldName) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 계산할 벡터 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - expression
     - 다음 예와 같은 간단한 계산식입니다. 예) [population] / ([geom_area] / 1000000)
     - Expression
     -
     - ✓

   * - fieldName
     - 계산식이 저장될 필드 이름입니다.
     - String
     - evaluated
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
     - 출력 레이어.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - Expression 에 의해 반환되는 값이 Geometry인 경우 fieldName은 무시되고 반환되는 데이터의 Geometry값이 적용된다.

**Examples**

다음은 mincircle( [geom] ) 을 처리한 예입니다. 이와 같이 필드의 연산을 이용한 속성값 계산뿐만 아니라 Geometry 변환까지 처리가 가능합니다. 

  .. image:: images/calculatefield.png

**Advanced Expression**

Expression 파라미터의 다양한 활용 예제이며, [geom] 은 PostGIS, Shapefile 등의 Geometry 필드 이름입니다.


.. list-table::
   :widths: 45 45 10

   * - **구분**
     - **표현식**
     - **반환값**

   * - 일반 수식
     - round([pop2008] / (area( [geom] ) / 1000000)).
     - Numeric

   * - 면적
     - area( [geom] )
     - Numeric

   * - 둘레/길이
     - geomLength( [geom] )
     - Numeric

   * - 중심점의 X 좌표
     - getX( centroid( [geom]))
     - Numeric

   * - 폴리곤을 라인으로
     - boundary( [geom] )
     - Geometry

   * - 버퍼
     - bufferWithSegments( [geom], 250, 16)
     - Polygon

   * - 무게중심점
     - centroid( [geom])
     - Point

   * - 폴리곤에 포함되는 내부 점
     - interiorPoint( [geom] )
     - Point

   * - 폴리곤 또는 라인의 시작점
     - startPoint( [geom] )
     - Point

   * - 폴리곤 또는 라인의 끝점
     - endPoint( [geom])
     - Point

   * - 폴리곤, 라인, 멀티포인트의Convex Hull
     - convexHull( [geom] )
     - Polygon

   * - 폴리곤, 라인, 멀티포인트를 둘러싸는 최소 원
     - mincircle( [geom] )
     - Polygon

   * - 폴리곤, 라인, 멀티포인트를 포함하는 영역의 최소 반경 라인
     - minimumdiameter( [geom] )
     - Line

   * - 폴리곤, 라인, 멀티포인트를 포함하는 영역의 최소 반경 영역
     - minrectangle( [geom] )
     - Polygon

   * - 폴리곤, 라인, 멀티포인트를 포함하는 최소 8각형 영역
     - octagonalenvelope( [geom] )
     - Polygon

   * - x offset, y offset 만큼 이동
     - offset( [geom], 4000, 3000)
     - Geometry
