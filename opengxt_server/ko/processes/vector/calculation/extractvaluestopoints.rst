.. _extractvaluestopoints:

포인트에 래스터 셀값 계산
==========================================

각 포인트 피처에 셀 원본값, 경사도 등의 셀값 계산 유형별 래스터의 셀값을 계산합니다.

**Syntax**

ExtractValuesToPoints (SimpleFeatureCollection pointFeatures, String valueField, GridCoverage2D valueCoverage, ExtractionType valueType) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - pointFeatures
     - 값이 계산될 포인트 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - valueField
     - 래스터의 셀값이 계산될 필드입니다.
     - String
     - rasterval
     -

   * - valueCoverage
     - 값을 가져올 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - valueType
     - 셀값 유형: Default(기본값), SlopeAsDegree(도 단위의 경사값), SlopeAsPercentrise(퍼센트단위의 경사값), Aspect.(사면 향)
     - ExtractionType
     - Default
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
     - 결과
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - valueType: Default(기본값), SlopeAsDegree, SlopeAsPercentrise, Aspect
 - valueField가 Null인 경우 evaluated 필드 이름을 사용한다.
 - valueType 파라미터가 Null인 경우 GridCoverage의 원본 셀 값을 반환한다.
 - valueCoverage가 DEM인 경우 valueType 은 SlopeAsDegree, SlopeAsPercentrise, Aspect 옵션을 사용할 수 있다.


**Examples**

시군구청 포인트 데이터에 DEM의 표고값을 계산한 결과입니다.

  .. image:: images/extractvaluestopoints.png
