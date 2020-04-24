.. _nearestneighbor:

최근린 이웃 지수
===========================

각각의 피처를 기준으로 최근린 이웃 피처와의 평균 거리에 기반한 최근린 이웃 지수를 계산합니다.

**Syntax**

NearestNeighborIndex (SimpleFeatureCollection inputFeatures, DistanceMethod distanceMethod, Double area) : NearestNeighborResult

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputFeatures
     - 최근린 이웃 지수를 계산할 입력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - distanceMethod
     - 각각의 피처와 이웃 피처의 거리를 계산하는데 사용되는 알고리즘 입니다: Euclidean(기본값) 또는 Manhattan.
     - DistanceMethod
     - Euclidean
     -

   * - area
     - 분석 영역을 정의할 숫자 값입니다.
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
     - 최근린 이웃 지수 결과입니다.
     - NearestNeighborResult
     -
     - ✓

**Constraints**

 - distanceMethod: Euclidean(기본값), Manhattan
 - inputFeatures의 Centroid를 이용하여 계산한다.
 - area 파라미터를 설정하지 않으면 inputFeatures의 Centroid에 대한 Convex Hull Polygon 면적을 이용한다.
 - Output은 XML로 반환하며, 반환된 Nearest Neighbor Ratio의 값이 1이면 Random, 1보다 크면 분산, 1보다 작으면 집중되어 있다고 볼 수 있다.


**Examples**

  .. code-block::

    <?xml version="1.0" encoding="utf-8"?>
    <NearestNeighborIndex>
      <TypeName>apartment</TypeName>
      <Observed_Point_Count>4052</Observed_Point_Count>
      <Study_Area>1.047557075141607E9</Study_Area>
      <Observed_Mean_Distance>200.00446</Observed_Mean_Distance>
      <Expected_Mean_Distance>254.22844</Expected_Mean_Distance>
      <Nearest_Neighbor_Ratio>0.786712</Nearest_Neighbor_Ratio>
      <Z_Score>-25.973484</Z_Score>
      <P_Value>0.0</P_Value>
      <Standard_Error>2.087667</Standard_Error>
    </NearestNeighborIndex>
