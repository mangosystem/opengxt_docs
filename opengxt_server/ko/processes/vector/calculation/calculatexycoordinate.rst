.. _calculatexycoordinate:

X, Y 좌표값 계산
=================================

X, Y 필드를 추가한 후 좌표값을 계산합니다. 변환 좌표체계가 설정되면 좌표체계 변환값을 계산합니다.

**Syntax**

CalculateXYCoordinate (SimpleFeatureCollection inputFeatures, String xField, String yField, Boolean inside, CoordinateReferenceSystem targetCRS) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 입력 레이어.
     - SimpleFeatureCollection
     -
     - ✓

   * - xField
     - X 좌표값이 계산될 필드입니다.
     - String
     - x_coord
     -

   * - yField
     - Y 좌표값이 계산될 필드입니다.
     - String
     - y_coord
     -

   * - inside
     - 입력 레이어가 폴리곤일 경우 계산될 좌표값이 폴리곤에 반드시 포함(True)하거나 무게중심점(False)을 사용합니다.
     - Boolean
     - false
     -

   * - targetCRS
     - 입력 레이어의 원본 좌표체계를 이 좌표체계로 변환한 좌표값을 계산합니다.
     - CoordinateReferenceSystem
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
     - 출력 레이어.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures는 포인트, 라인, 폴리곤 모두 가능하다.
 - inputFeatures가 폴리곤이고 inside 가 Ture이면 중심점은 반드시 폴리곤 내에 포함된다.
 - targetCRS가 Null이면 원본 데이터의 좌표값을, 그렇지 않으면 좌표 변환한 값을 반환한다.


**Examples**

폴리곤 레이어의 중심값을 기준으로 xcoord, ycoord 필드에 targetCRS를 EPSG:4326(WGS84 경위도 좌표계)으로 계산한 예입니다.

  .. image:: images/calculatexycoordinate.png
