.. _hublinesbyid:

ID값으로 허브 라인 생성
==========================================

두 레이어의 조인 필드를 이용하여 속성값이 일치하는 허브와 스포크 피처 사이의 최단 거리를 잇는 라인 피처를 생성합니다.

**Syntax**

HubLinesByID (SimpleFeatureCollection hubFeatures, String hubIdField, SimpleFeatureCollection spokeFeatures, String spokeIdField, Boolean preserveAttributes, Boolean useCentroid, Boolean useBezierCurve, Double maximumDistance) : SimpleFeatureCollection

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - hubFeatures
     - 중심이 되는 허브 레이어을 설정합니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - hubIdField
     - 스포크 레이어와 조인키가 되는 스포크 ID 필드를 설정합니다.
     - String
     -
     - ✓

   * - spokeFeatures
     - 허브 레이어에 연결할 스포크 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

   * - spokeIdField
     - 허브 레이어와 조인키가 되는 스포크 ID 필드를 설정합니다.
     - String
     -
     - ✓

   * - preserveAttributes
     - 스포크 레이어의 속성정보 유지 여뷰를 설정합니다.
     - Boolean
     - true
     -

   * - useCentroid
     - 포인트 레이어가 아닌 경우 두 피처간의 최단거리 라인 생성시 중심점을 사용할지 여부를 설정합니다.
     - Boolean
     - true
     -

   * - useBezierCurve
     - 두 지점간의 최단거리 라인 생성시 베이지어 커브를 사용할지 여부를 설정합니다.
     - Boolean
     - false
     -

   * - maximumDistance
     - 연결할 라인의 최대 거리를 설정합니다.
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
     - 생성된 허브라인 출력 레이어입니다.
     - SimpleFeatureCollection
     -
     - ✓

**Constraints**

 - useCentroid 파라미터가 True이고 hubFeatures, spokeFeatures의 Geometry 피처 타입이 라인 또는 폴리곤인 경우 Geometry의 Centroid를 이용하여 Hub Line을 생성한다.
 - useBezierCurve 파라미터가 True이면 두 피처간의 최단 라인을 Bezier curve로 생성한다.
 - maximumDistance 파라미터가 0보다 큰 경우 이 거리 내에 있는 피처만을 대상으로 Hub Line을 생성한다.

**Examples**

시군구청을 Hub로 설정하여 읍면동 폴리곤을 Spoke 레이어로 설정하고 시군구 코드를 기준으로Hub Line을 생성한 결과입니다.

  .. image:: images/hublinesbyid.png
