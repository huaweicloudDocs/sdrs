# 查询资源的RPO超标趋势记录列表<a name="sdrs_05_1001"></a>

## 功能介绍<a name="zh-cn_topic_0079693002_section34649765"></a>

查询当前租户大屏显示中，资源的RPO超标趋势记录列表。

## 约束与限制<a name="section15178131662310"></a>

无

## URI<a name="zh-cn_topic_0079693002_section39390935"></a>

-   URI格式

    GET /v1/\{project\_id\}/resource/rpo-statistics

-   参数说明

    <a name="zh-cn_topic_0079693002_table63321005"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0079693002_row37593218"><th class="cellrowborder" valign="top" width="21.782178217821784%" id="mcps1.1.5.1.1"><p id="p161751519115617"><a name="p161751519115617"></a><a name="p161751519115617"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.1.5.1.2"><p id="p19175131913564"><a name="p19175131913564"></a><a name="p19175131913564"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.841584158415841%" id="mcps1.1.5.1.3"><p id="p17175151916562"><a name="p17175151916562"></a><a name="p17175151916562"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="49.504950495049506%" id="mcps1.1.5.1.4"><p id="p817511935618"><a name="p817511935618"></a><a name="p817511935618"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0079693002_row29123463"><td class="cellrowborder" valign="top" width="21.782178217821784%" headers="mcps1.1.5.1.1 "><p id="p15175121945618"><a name="p15175121945618"></a><a name="p15175121945618"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.1.5.1.2 "><p id="p917561965616"><a name="p917561965616"></a><a name="p917561965616"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p917531975612"><a name="p917531975612"></a><a name="p917531975612"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.504950495049506%" headers="mcps1.1.5.1.4 "><p id="p11176619125614"><a name="p11176619125614"></a><a name="p11176619125614"></a>项目ID。</p>
    <p id="p1011411112497"><a name="p1011411112497"></a><a name="p1011411112497"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   Request filter参数说明

    <a name="zh-cn_topic_0079693002_table54932709"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0079693002_row41882373"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.1"><p id="p2363104375614"><a name="p2363104375614"></a><a name="p2363104375614"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.1.5.1.2"><p id="p7363843115616"><a name="p7363843115616"></a><a name="p7363843115616"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="15%" id="mcps1.1.5.1.3"><p id="p636311434569"><a name="p636311434569"></a><a name="p636311434569"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="46%" id="mcps1.1.5.1.4"><p id="p736314315560"><a name="p736314315560"></a><a name="p736314315560"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0079693002_row27990155"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p636364345612"><a name="p636364345612"></a><a name="p636364345612"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.1.5.1.2 "><p id="p15363174385611"><a name="p15363174385611"></a><a name="p15363174385611"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p183631643115620"><a name="p183631643115620"></a><a name="p183631643115620"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="46%" headers="mcps1.1.5.1.4 "><p id="p3363194365615"><a name="p3363194365615"></a><a name="p3363194365615"></a>每次请求返回结果个数限制，取值范围为[0,1000]的正整数，默认值为1000。</p>
    </td>
    </tr>
    <tr id="row49112572514"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p736344317569"><a name="p736344317569"></a><a name="p736344317569"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.1.5.1.2 "><p id="p2363543145612"><a name="p2363543145612"></a><a name="p2363543145612"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p836316436564"><a name="p836316436564"></a><a name="p836316436564"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="46%" headers="mcps1.1.5.1.4 "><p id="p1752104119595"><a name="p1752104119595"></a><a name="p1752104119595"></a>每次请求开始的下标，即偏移量，默认值为0。offset必须为数字，不能为负数。</p>
    </td>
    </tr>
    <tr id="row14277596517"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p33631043105615"><a name="p33631043105615"></a><a name="p33631043105615"></a>start_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.1.5.1.2 "><p id="p193637436561"><a name="p193637436561"></a><a name="p193637436561"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p2363174355610"><a name="p2363174355610"></a><a name="p2363174355610"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46%" headers="mcps1.1.5.1.4 "><p id="p6363134316569"><a name="p6363134316569"></a><a name="p6363134316569"></a>开始时间。</p>
    <p id="p9590163611256"><a name="p9590163611256"></a><a name="p9590163611256"></a>默认格式为："yyyy-MM-dd HH:mm:ss.SSS"，例："2019-04-01 12:00:00.000"。</p>
    </td>
    </tr>
    <tr id="row971182745318"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p851015142419"><a name="p851015142419"></a><a name="p851015142419"></a>end_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.1.5.1.2 "><p id="p1951385152415"><a name="p1951385152415"></a><a name="p1951385152415"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p115154512243"><a name="p115154512243"></a><a name="p115154512243"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46%" headers="mcps1.1.5.1.4 "><p id="p15171251182415"><a name="p15171251182415"></a><a name="p15171251182415"></a>结束时间。</p>
    <p id="p789065614284"><a name="p789065614284"></a><a name="p789065614284"></a>默认格式为："yyyy-MM-dd HH:mm:ss.SSS"，例："2019-04-01 12:00:00.000"。</p>
    </td>
    </tr>
    <tr id="row129428252252"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p894414251256"><a name="p894414251256"></a><a name="p894414251256"></a>resource_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.1.5.1.2 "><p id="p31853375252"><a name="p31853375252"></a><a name="p31853375252"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p12944625112511"><a name="p12944625112511"></a><a name="p12944625112511"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46%" headers="mcps1.1.5.1.4 "><p id="p1994482542516"><a name="p1994482542516"></a><a name="p1994482542516"></a>资源类型。</p>
    <a name="ul7844153212592"></a><a name="ul7844153212592"></a><ul id="ul7844153212592"><li>replication：表示查询复制对的RPO超标趋势记录。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section13320326141616"></a>

-   请求参数

    无

-   请求样例

    GET https://\{Endpoint\}/v1/\{project\_id\}/resource/rpo-statistics


## 响应<a name="zh-cn_topic_0079693002_section36549175"></a>

-   要素说明

    <a name="table155991608555"></a>
    <table><thead align="left"><tr id="row460510055518"><th class="cellrowborder" valign="top" width="29.07%" id="mcps1.1.4.1.1"><p id="p56078010555"><a name="p56078010555"></a><a name="p56078010555"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.44%" id="mcps1.1.4.1.2"><p id="p961219016552"><a name="p961219016552"></a><a name="p961219016552"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.49%" id="mcps1.1.4.1.3"><p id="p186139012557"><a name="p186139012557"></a><a name="p186139012557"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row86164025512"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.1.4.1.1 "><p id="p21991181583"><a name="p21991181583"></a><a name="p21991181583"></a>resource_rpo_statistics</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.1.4.1.2 "><p id="p91992895813"><a name="p91992895813"></a><a name="p91992895813"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.49%" headers="mcps1.1.4.1.3 "><p id="p21995845812"><a name="p21995845812"></a><a name="p21995845812"></a>资源的RPO超标趋势记录列表。</p>
    <p id="p1314220519179"><a name="p1314220519179"></a><a name="p1314220519179"></a>详情请参见<a href="#table503353570">表1</a>。</p>
    </td>
    </tr>
    <tr id="row166368013553"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.1.4.1.1 "><p id="p1919910835818"><a name="p1919910835818"></a><a name="p1919910835818"></a>count</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.1.4.1.2 "><p id="p91992084588"><a name="p91992084588"></a><a name="p91992084588"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.49%" headers="mcps1.1.4.1.3 "><p id="p1201158165818"><a name="p1201158165818"></a><a name="p1201158165818"></a>列表中包含的资源的RPO超标趋势记录个数。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 1**  resource\_rpo\_statistics字段说明

    <a name="table503353570"></a>
    <table><thead align="left"><tr id="row131163505710"><th class="cellrowborder" valign="top" width="29.07%" id="mcps1.2.4.1.1"><p id="p8131435155711"><a name="p8131435155711"></a><a name="p8131435155711"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.43%" id="mcps1.2.4.1.2"><p id="p6251035195718"><a name="p6251035195718"></a><a name="p6251035195718"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.5%" id="mcps1.2.4.1.3"><p id="p1727173517574"><a name="p1727173517574"></a><a name="p1727173517574"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row10204148131510"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.2.4.1.1 "><p id="p152051282150"><a name="p152051282150"></a><a name="p152051282150"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.2.4.1.2 "><p id="p112051181153"><a name="p112051181153"></a><a name="p112051181153"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.5%" headers="mcps1.2.4.1.3 "><p id="p10205189151"><a name="p10205189151"></a><a name="p10205189151"></a>资源的RPO超标趋势记录id。</p>
    </td>
    </tr>
    <tr id="row1472144614199"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.2.4.1.1 "><p id="p8874044105311"><a name="p8874044105311"></a><a name="p8874044105311"></a>point_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.2.4.1.2 "><p id="p132481142125812"><a name="p132481142125812"></a><a name="p132481142125812"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.5%" headers="mcps1.2.4.1.3 "><p id="p82481642175811"><a name="p82481642175811"></a><a name="p82481642175811"></a>资源的RPO超标趋势记录打点时间。</p>
    <p id="p676145013419"><a name="p676145013419"></a><a name="p676145013419"></a>默认格式为："yyyy-MM-dd HH:mm"。</p>
    </td>
    </tr>
    <tr id="row1845264811918"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.2.4.1.1 "><p id="p1587444415317"><a name="p1587444415317"></a><a name="p1587444415317"></a>resource_num</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.2.4.1.2 "><p id="p12481042145818"><a name="p12481042145818"></a><a name="p12481042145818"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.5%" headers="mcps1.2.4.1.3 "><p id="p024804218583"><a name="p024804218583"></a><a name="p024804218583"></a>RPO超标的资源个数。</p>
    </td>
    </tr>
    <tr id="row1673634113018"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.2.4.1.1 "><p id="p1173134193016"><a name="p1173134193016"></a><a name="p1173134193016"></a>resource_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.2.4.1.2 "><p id="p167333493016"><a name="p167333493016"></a><a name="p167333493016"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.5%" headers="mcps1.2.4.1.3 "><p id="p16738348308"><a name="p16738348308"></a><a name="p16738348308"></a>RPO超标的资源类型。</p>
    <a name="ul1191643384515"></a><a name="ul1191643384515"></a><ul id="ul1191643384515"><li>replication：表示查询复制对的RPO超标趋势记录。</li></ul>
    </td>
    </tr>
    <tr id="row4130183355311"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.2.4.1.1 "><p id="p188777444534"><a name="p188777444534"></a><a name="p188777444534"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.2.4.1.2 "><p id="p1024894275819"><a name="p1024894275819"></a><a name="p1024894275819"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.5%" headers="mcps1.2.4.1.3 "><p id="p1248342175814"><a name="p1248342175814"></a><a name="p1248342175814"></a>创建时间。</p>
    <p id="p4129153232"><a name="p4129153232"></a><a name="p4129153232"></a>默认格式为："yyyy-MM-dd HH:mm:ss.SSS"，例："2019-04-01 12:00:00.000"。</p>
    </td>
    </tr>
    <tr id="row838919355539"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.2.4.1.1 "><p id="p118776443530"><a name="p118776443530"></a><a name="p118776443530"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.2.4.1.2 "><p id="p11248204217584"><a name="p11248204217584"></a><a name="p11248204217584"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.5%" headers="mcps1.2.4.1.3 "><p id="p32481425582"><a name="p32481425582"></a><a name="p32481425582"></a>更新时间。</p>
    <p id="p380510139417"><a name="p380510139417"></a><a name="p380510139417"></a>默认格式为："yyyy-MM-dd HH:mm:ss.SSS"，例："2019-04-01 12:00:00.000"。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    { 
       "count": 2, 
       "resource_rpo_statistics": [
            {
                "id": "c5f38ca9-a2e0-4c4c-aea3-35cb5caccc00",
                "point_time": "2019-01-21 01:15",
                "resource_num": 1,
                "resource_type": "replication",
                "created_at": "2019-01-21 01:15:00.916",
                "updated_at": "2019-01-21 01:15:00.916"
            },
            {
                "id": "1ef74edc-9311-47c8-b092-231e64e11bee",
                "point_time": "2019-01-21 01:10",
                "resource_num": 2,
                "resource_type": "replication",
                "created_at": "2019-01-21 01:14:56.427",
                "updated_at": "2019-01-21 01:14:56.427"
            }
        ]
     }
    ```

    或

    ```
    { 
         "error": { 
             "message": "XXXX",  
             "code": "XXX" 
         } 
     }
    ```

    其中error是泛指的错误，有badrequest、itemNotFound等，如报错为：

    ```
    { 
         "badrequest": { 
             "message": "XXXX",  
             "code": "XXX" 
         } 
     }
    ```


## 返回值<a name="zh-cn_topic_0079693002_section60507121"></a>

-   正常

    <a name="sdrs_05_0101_table4315991194956"></a>
    <table><thead align="left"><tr id="sdrs_05_0101_row2336641294956"><th class="cellrowborder" valign="top" width="42.59%" id="mcps1.1.3.1.1"><p id="sdrs_05_0101_p1363125894956"><a name="sdrs_05_0101_p1363125894956"></a><a name="sdrs_05_0101_p1363125894956"></a>返回值</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.410000000000004%" id="mcps1.1.3.1.2"><p id="sdrs_05_0101_p3039012494956"><a name="sdrs_05_0101_p3039012494956"></a><a name="sdrs_05_0101_p3039012494956"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="sdrs_05_0101_row507566794956"><td class="cellrowborder" valign="top" width="42.59%" headers="mcps1.1.3.1.1 "><p id="sdrs_05_0101_p847584694956"><a name="sdrs_05_0101_p847584694956"></a><a name="sdrs_05_0101_p847584694956"></a>200</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.410000000000004%" headers="mcps1.1.3.1.2 "><p id="sdrs_05_0101_p1545496394956"><a name="sdrs_05_0101_p1545496394956"></a><a name="sdrs_05_0101_p1545496394956"></a>服务器已接受请求。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   异常

    <a name="sdrs_05_0101_table22458872203835"></a>
    <table><thead align="left"><tr id="sdrs_05_0101_row35704554203835"><th class="cellrowborder" valign="top" width="43.419999999999995%" id="mcps1.1.3.1.1"><p id="sdrs_05_0101_p6387753203835"><a name="sdrs_05_0101_p6387753203835"></a><a name="sdrs_05_0101_p6387753203835"></a>返回值</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.58%" id="mcps1.1.3.1.2"><p id="sdrs_05_0101_p47646009203835"><a name="sdrs_05_0101_p47646009203835"></a><a name="sdrs_05_0101_p47646009203835"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="sdrs_05_0101_row34121538203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="sdrs_05_0101_p12381163203835"><a name="sdrs_05_0101_p12381163203835"></a><a name="sdrs_05_0101_p12381163203835"></a>400 Bad Request</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="sdrs_05_0101_p63350108203835"><a name="sdrs_05_0101_p63350108203835"></a><a name="sdrs_05_0101_p63350108203835"></a>服务器未能处理请求。</p>
    </td>
    </tr>
    <tr id="sdrs_05_0101_row33280063203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="sdrs_05_0101_p11330608203835"><a name="sdrs_05_0101_p11330608203835"></a><a name="sdrs_05_0101_p11330608203835"></a>401 Unauthorized</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="sdrs_05_0101_p45364094203835"><a name="sdrs_05_0101_p45364094203835"></a><a name="sdrs_05_0101_p45364094203835"></a>被请求的页面需要用户名和密码。</p>
    </td>
    </tr>
    <tr id="sdrs_05_0101_row5623667203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="sdrs_05_0101_p52863895203835"><a name="sdrs_05_0101_p52863895203835"></a><a name="sdrs_05_0101_p52863895203835"></a>403 Forbidden</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="sdrs_05_0101_p54117066203835"><a name="sdrs_05_0101_p54117066203835"></a><a name="sdrs_05_0101_p54117066203835"></a>对被请求页面的访问被禁止。</p>
    </td>
    </tr>
    <tr id="sdrs_05_0101_row17291554203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="sdrs_05_0101_p58438642203835"><a name="sdrs_05_0101_p58438642203835"></a><a name="sdrs_05_0101_p58438642203835"></a>404 Not Found</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="sdrs_05_0101_p35909542203835"><a name="sdrs_05_0101_p35909542203835"></a><a name="sdrs_05_0101_p35909542203835"></a>服务器无法找到被请求的页面。</p>
    </td>
    </tr>
    <tr id="sdrs_05_0101_row54750425203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="sdrs_05_0101_p5599455203835"><a name="sdrs_05_0101_p5599455203835"></a><a name="sdrs_05_0101_p5599455203835"></a>405 Method Not Allowed</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="sdrs_05_0101_p50902717203835"><a name="sdrs_05_0101_p50902717203835"></a><a name="sdrs_05_0101_p50902717203835"></a>请求中指定的方法不被允许。</p>
    </td>
    </tr>
    <tr id="sdrs_05_0101_row55471277203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="sdrs_05_0101_p63988484203835"><a name="sdrs_05_0101_p63988484203835"></a><a name="sdrs_05_0101_p63988484203835"></a>406 Not Acceptable</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="sdrs_05_0101_p15684678203835"><a name="sdrs_05_0101_p15684678203835"></a><a name="sdrs_05_0101_p15684678203835"></a>服务器生成的响应无法被客户端所接受。</p>
    </td>
    </tr>
    <tr id="sdrs_05_0101_row6944380203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="sdrs_05_0101_p25623884203835"><a name="sdrs_05_0101_p25623884203835"></a><a name="sdrs_05_0101_p25623884203835"></a>407 Proxy Authentication Required</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="sdrs_05_0101_p62268733203835"><a name="sdrs_05_0101_p62268733203835"></a><a name="sdrs_05_0101_p62268733203835"></a>用户必须首先使用代理服务器进行验证，这样请求才会被处理。</p>
    </td>
    </tr>
    <tr id="sdrs_05_0101_row23547689203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="sdrs_05_0101_p28314670203835"><a name="sdrs_05_0101_p28314670203835"></a><a name="sdrs_05_0101_p28314670203835"></a>408 Request Timeout</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="sdrs_05_0101_p11786919203835"><a name="sdrs_05_0101_p11786919203835"></a><a name="sdrs_05_0101_p11786919203835"></a>请求超出了服务器的等待时间。</p>
    </td>
    </tr>
    <tr id="sdrs_05_0101_row38973411203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="sdrs_05_0101_p2729702203835"><a name="sdrs_05_0101_p2729702203835"></a><a name="sdrs_05_0101_p2729702203835"></a>409 Conflict</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="sdrs_05_0101_p19779281203835"><a name="sdrs_05_0101_p19779281203835"></a><a name="sdrs_05_0101_p19779281203835"></a>由于冲突，请求无法被完成。</p>
    </td>
    </tr>
    <tr id="sdrs_05_0101_row43795805203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="sdrs_05_0101_p57799353203835"><a name="sdrs_05_0101_p57799353203835"></a><a name="sdrs_05_0101_p57799353203835"></a>500 Internal Server Error</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="sdrs_05_0101_p51235984203835"><a name="sdrs_05_0101_p51235984203835"></a><a name="sdrs_05_0101_p51235984203835"></a>请求未完成。服务异常。</p>
    </td>
    </tr>
    <tr id="sdrs_05_0101_row58470678203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="sdrs_05_0101_p38504500203835"><a name="sdrs_05_0101_p38504500203835"></a><a name="sdrs_05_0101_p38504500203835"></a>501 Not Implemented</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="sdrs_05_0101_p31856770203835"><a name="sdrs_05_0101_p31856770203835"></a><a name="sdrs_05_0101_p31856770203835"></a>请求未完成。服务器不支持所请求的功能。</p>
    </td>
    </tr>
    <tr id="sdrs_05_0101_row18275474203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="sdrs_05_0101_p3918444203835"><a name="sdrs_05_0101_p3918444203835"></a><a name="sdrs_05_0101_p3918444203835"></a>502 Bad Gateway</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="sdrs_05_0101_p48958538203835"><a name="sdrs_05_0101_p48958538203835"></a><a name="sdrs_05_0101_p48958538203835"></a>请求未完成。服务器从上游服务器收到一个无效的响应。</p>
    </td>
    </tr>
    <tr id="sdrs_05_0101_row37973662203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="sdrs_05_0101_p55967806203835"><a name="sdrs_05_0101_p55967806203835"></a><a name="sdrs_05_0101_p55967806203835"></a>503 Service Unavailable</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="sdrs_05_0101_p37098455203835"><a name="sdrs_05_0101_p37098455203835"></a><a name="sdrs_05_0101_p37098455203835"></a>请求未完成。系统暂时异常。</p>
    </td>
    </tr>
    <tr id="sdrs_05_0101_row65450640203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="sdrs_05_0101_p67010448203835"><a name="sdrs_05_0101_p67010448203835"></a><a name="sdrs_05_0101_p67010448203835"></a>504 Gateway Timeout</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="sdrs_05_0101_p59137180203835"><a name="sdrs_05_0101_p59137180203835"></a><a name="sdrs_05_0101_p59137180203835"></a>网关超时。</p>
    </td>
    </tr>
    </tbody>
    </table>


