.. _idw:

IDW 보간
==================

포인트 피처에 대해 Inverse Distance Weighted (IDW) 보간법을 적용한 래스터를 생성합니다.

**Syntax**

IDW (SimpleFeatureCollection inputFeatures, String inputField, Double power, RadiusType radiusType, Integer numberOfPoints, Double distance, Double cellSize, ReferencedEnvelope extent) : GridCoverage2D

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 보간할 입력 포인트 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - inputField
     - 각각의 샘플 포인트에 대한 높이 또는 크기 등 값을 포함한 필드입니다.
     - String
     -
     - ✓

   * - power
     - 거리에 대한 지수값(기본값은 2.0)입니다.
     - Double
     - 2.0
     -

   * - radiusType
     - 이웃한 샘플 포인트를 탐색하는데 사용되는 탐색 반경 유형입니다. Variable(기본값), Fixed.
     - RadiusType
     - Variable
     -

   * - numberOfPoints
     - 보간에 사용되는 이웃한 샘플 포인트의 수를 정수값으로 설정합니다.
     - Integer
     - 12
     -

   * - distance
     - 이웃한 입력 샘플 포인트를 탐색할 지도 단위의 최대 탐색 반경입니다.
     - Double
     - 0.0
     -

   * - cellSize
     - 출력 래스터 레이어의 셀 크기입니다.
     - Double
     - 0.0
     -

   * - extent
     - 출력 래스터 레이어의 공간 범위입니다.
     - ReferencedEnvelope
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
     - 보간한 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - radiusType: Variable(기본값), Fixed
 - extent 파라미터를 설정하지 않으면 inputFeatures 레이어의 범위를 사용한다.
 - cellSize 파라미터를 설정하지 않으면 Extent의 Width와 Height 중 작은 값을 250으로 나눈 값을 사용한다.


**Examples**
