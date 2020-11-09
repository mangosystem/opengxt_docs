.. _rasterdescribe:

래스터 정보 확인
===========================

래스터 레이어의 메타데이터 정보를 확인합니다.

**Syntax**

RasterDescribe (GridCoverage2D inputCoverage, Boolean detailed) : RasterDescribeResult

**Input Parameters**

.. list-table::
   :widths: 10 50 20 10 10

   * - **Identifier**
     - **Description**
     - **Type**
     - **Default**
     - **Required**

   * - inputCoverage
     - 정보를 가져올 입력 래스터 레이어입니다.
     - GridCoverage2D
     -
     - ✓

   * - detailed
     - 래스터의 셀값에 대한 요약통계정보를 계산하여 정보로 출력할 지 여부를 설정합니다. 기본값은 아니오(False)입니다.
     - Boolean
     - false
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
     - 입력 래스터 레이어에 대한 요약 정보입니다.
     - RasterDescribeResult
     -
     - ✓

**Constraints**

 - detailed가 true인 경우 각각의 밴드별 기본 통계정보를 계산하여 반환한다.
 - Output은 XML로 반환한다.


**Examples**

.. code-block:: XML

    <?xml version="1.0" encoding="UTF-8"?>
    <RasterDescription>
      <Name>seoul_dem30</Name>
      <Columns>1556</Columns>
      <Rows>1279</Rows>
      <NumberOfBands>1</NumberOfBands>
      <CellSizeX>29.998701738731725</CellSizeX>
      <CellSizeY>30.001479578692326</CellSizeY>
      <PixelType>UNSIGNED_16BITS</PixelType>
      <PixelDepth>16BITS</PixelDepth>
      <NoData>0.0</NoData>
      <Extent>
        <XMin>1.4111343323506365E7</XMin>
        <YMin>4498971.750719266</YMin>
        <XMax>1.4158021303411832E7</XMax>
        <YMax>4537343.6431004135</YMax>
      </Extent>
      <SpatialReference>PROJCS["WGS 84 / Pseudo-Mercator", &#13;
        GEOGCS["WGS 84", &#13;
          DATUM["World Geodetic System 1984", &#13;
            SPHEROID["WGS 84", 6378137.0, 298.257223563, AUTHORITY["EPSG","7030"]], &#13;
            AUTHORITY["EPSG","6326"]], &#13;
          PRIMEM["Greenwich", 0.0, AUTHORITY["EPSG","8901"]], &#13;
          UNIT["degree", 0.017453292519943295], &#13;
          AXIS["Geodetic longitude", EAST], &#13;
          AXIS["Geodetic latitude", NORTH], &#13;
          AUTHORITY["EPSG","4326"]], &#13;
        PROJECTION["Popular Visualisation Pseudo Mercator", AUTHORITY["EPSG","1024"]], &#13;
        PARAMETER["semi_minor", 6378137.0], &#13;
        PARAMETER["latitude_of_origin", 0.0], &#13;
        PARAMETER["central_meridian", 0.0], &#13;
        PARAMETER["scale_factor", 1.0], &#13;
        PARAMETER["false_easting", 0.0], &#13;
        PARAMETER["false_northing", 0.0], &#13;
        UNIT["m", 1.0], &#13;
        AXIS["Easting", EAST], &#13;
        AXIS["Northing", NORTH], &#13;
        AUTHORITY["EPSG","3857"]]
      </SpatialReference>
      <Band>
        <BandIndex>0</BandIndex>
        <Description>GRAY_INDEX</Description>
        <Count>1068918</Count>
        <Minimun>1.0</Minimun>
        <Maximin>754.0</Maximin>
        <Mean>61.70939866294702</Mean>
        <Sum>6.5962287E7</Sum>
        <Variance>6771.511633069396</Variance>
        <StandardDeviation>82.2891951173992</StandardDeviation>
        <NoData>0.0</NoData>
      </Band>
    </RasterDescription>

      .. image:: images/rasterdescribe.png
