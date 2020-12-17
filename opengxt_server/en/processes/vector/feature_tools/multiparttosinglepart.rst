.. _multiparttosinglepart:

멀티파트를 싱글파트로 변환
==========================================

멀티파트 피처를 분할하여 싱글파트 피처로 변환합니다.

**Syntax**

MultipartToSinglepart (SimpleFeatureCollection inputFeatures) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 멀티파트 피처를 포함한 입력 레이어입니다.
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
     - 싱글파트로 변환된 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - inputFeatures 파라미터는 반드시 Multipart(MultiPoint, MultiLineString, MultiPolygon) 피처 타입이어야 한다.

**Examples**

2개 이상의 Polygon으로 구성된 MultiPolygon을 Single Polygon으로 변환한 결과입니다.

  .. image:: images/multiparttosinglepart.png
