.. _quadratanalysis:

방격(Quadrat) 분석
==========================================

방격(Quadrat) 분석 기법을 이용하여 포인트의 패턴 분석을 수행합니다.

**Syntax**

QuadratAnalysis (SimpleFeatureCollection inputFeatures, Double cellSize) : QuadratResult

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 방격 분석에 사용할 포인트 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - cellSize
     - 방격 분석에 생성될 그리드 셀의 크기입니다.
     - Double
     - 0.0
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
     - 방격 분석 결과입니다.
     - QuadratResult
     -
     - ✓

**Constraints**

 - inputFeatures의 Centroid를 이용하여 계산한다.
 - cellSize 파라미터를 설정하지 않으면 다음의 식을 이용하여 셀 크기를 계산한다. Math.sqrt((inputFeatures의 BBOX 면적 * 2) / 포인트의 갯수)


**Examples**

  .. code-block::

    <?xml version="1.0" encoding="utf-8"?>
    <QuadratAnalysis>
      <TypeName>gasstation</TypeName>
      <FeatureCount>587</FeatureCount>
      <Area>1.4406602767217913E9</Area>
      <CellSize>2215.5254234488443</CellSize>
      <Columns>19</Columns>
      <Rows>16</Rows>
      <Number_of_Quadrats>304</Number_of_Quadrats>
      <Mean>1.930921052631579</Mean>
      <Variance>5.643254414819944</Variance>
      <Variance_Mean_Ratio>2.9225712812696134</Variance_Mean_Ratio>
      <Kolmogorov_Smirnov_Test>0.32209069225598863</Kolmogorov_Smirnov_Test>
      <Critical_Value_at_5percent>0.078001349515991</Critical_Value_at_5percent>
    </QuadratAnalysis>
