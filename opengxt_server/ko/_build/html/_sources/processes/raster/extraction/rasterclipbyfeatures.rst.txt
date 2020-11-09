.. _rasterclipbyfeatures:

폴리곤 피처레이어로 래스터 추출
===================================================

폴리곤 피처레이어로 래스터를 추출합니다.

**Syntax**

RasterClipByFeatures (GridCoverage2D inputCoverage, SimpleFeatureCollection cropFeatures) : GridCoverage2D

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

   * - cropFeatures
     - 래스터를 잘라낼 폴리곤 또는 멀티폴리곤 유형의 레이어입니다.
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
     - 잘라낸 출력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

**Constraints**

 - inside 파라미터가 False인 경우 원을 제외한 지역을 반환한다.

**Examples**

  .. image:: images/rasterclipbyfeatures.png
