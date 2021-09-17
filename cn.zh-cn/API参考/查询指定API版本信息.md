# 查询指定API版本信息<a name="sdrs_05_0202"></a>

## 功能介绍<a name="section1593161881114"></a>

查询存储容灾指定API版本信息。

## 约束与限制<a name="section165931918141120"></a>

无

## URI<a name="section13593518191116"></a>

-   URI格式

    GET /\{api\_version\}

-   参数说明

    <a name="table186092189116"></a>
    <table><thead align="left"><tr id="row4202191910113"><th class="cellrowborder" valign="top" width="29.59%" id="mcps1.1.4.1.1"><p id="p1020271916119"><a name="p1020271916119"></a><a name="p1020271916119"></a>参数名</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.33%" id="mcps1.1.4.1.2"><p id="p1620211981114"><a name="p1620211981114"></a><a name="p1620211981114"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="54.08%" id="mcps1.1.4.1.3"><p id="p5202151951112"><a name="p5202151951112"></a><a name="p5202151951112"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row10202719151120"><td class="cellrowborder" valign="top" width="29.59%" headers="mcps1.1.4.1.1 "><p id="p620241931117"><a name="p620241931117"></a><a name="p620241931117"></a>api_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.33%" headers="mcps1.1.4.1.2 "><p id="p1920261913115"><a name="p1920261913115"></a><a name="p1920261913115"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="54.08%" headers="mcps1.1.4.1.3 "><p id="p22026196116"><a name="p22026196116"></a><a name="p22026196116"></a>API版本号。例如：v1。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section11625111891113"></a>

-   请求参数

    无

-   请求样例

    GET https://\{endpoint\}/v1


## 响应<a name="section196251718101117"></a>

-   要素说明

    <a name="table1265715185111"></a>
    <table><thead align="left"><tr id="row16202121991119"><th class="cellrowborder" valign="top" width="29.07%" id="mcps1.1.4.1.1"><p id="p1220211191119"><a name="p1220211191119"></a><a name="p1220211191119"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.44%" id="mcps1.1.4.1.2"><p id="p13202919161115"><a name="p13202919161115"></a><a name="p13202919161115"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.49%" id="mcps1.1.4.1.3"><p id="p1720241911117"><a name="p1720241911117"></a><a name="p1720241911117"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row20202171919110"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.1.4.1.1 "><p id="p1320281917114"><a name="p1320281917114"></a><a name="p1320281917114"></a>version</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.1.4.1.2 "><p id="p162021819121111"><a name="p162021819121111"></a><a name="p162021819121111"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.49%" headers="mcps1.1.4.1.3 "><p id="p10202121911111"><a name="p10202121911111"></a><a name="p10202121911111"></a>API版本信息。</p>
    <p id="p19242375287"><a name="p19242375287"></a><a name="p19242375287"></a>详情请参见<a href="#table14672161881114">表1</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 1**  version字段说明

    <a name="table14672161881114"></a>
    <table><thead align="left"><tr id="row020212196111"><th class="cellrowborder" valign="top" width="29.07%" id="mcps1.2.4.1.1"><p id="p720210196118"><a name="p720210196118"></a><a name="p720210196118"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.44%" id="mcps1.2.4.1.2"><p id="p1920271915118"><a name="p1920271915118"></a><a name="p1920271915118"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.49%" id="mcps1.2.4.1.3"><p id="p8202219121112"><a name="p8202219121112"></a><a name="p8202219121112"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row22021319181119"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.2.4.1.1 "><p id="p9202161913115"><a name="p9202161913115"></a><a name="p9202161913115"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.2.4.1.2 "><p id="p52021199111"><a name="p52021199111"></a><a name="p52021199111"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.49%" headers="mcps1.2.4.1.3 "><p id="p0202161941117"><a name="p0202161941117"></a><a name="p0202161941117"></a>版本ID（版本号），如v1。</p>
    </td>
    </tr>
    <tr id="row152021419121113"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.2.4.1.1 "><p id="p42021819141117"><a name="p42021819141117"></a><a name="p42021819141117"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.2.4.1.2 "><p id="p320213193119"><a name="p320213193119"></a><a name="p320213193119"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.49%" headers="mcps1.2.4.1.3 "><p id="p520218195117"><a name="p520218195117"></a><a name="p520218195117"></a>API的URL地址。</p>
    <p id="p14541184611292"><a name="p14541184611292"></a><a name="p14541184611292"></a>详情请参见<a href="#table122284216266">表2</a>。</p>
    </td>
    </tr>
    <tr id="row420214194116"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.2.4.1.1 "><p id="p2202191914110"><a name="p2202191914110"></a><a name="p2202191914110"></a>version</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.2.4.1.2 "><p id="p16202171919111"><a name="p16202171919111"></a><a name="p16202171919111"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.49%" headers="mcps1.2.4.1.3 "><p id="p5202919181115"><a name="p5202919181115"></a><a name="p5202919181115"></a>若该版本API支持微版本，则返回支持的最大微版本号，如果不支持微版本，则返回空。</p>
    </td>
    </tr>
    <tr id="row1720261915113"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.2.4.1.1 "><p id="p12021619151117"><a name="p12021619151117"></a><a name="p12021619151117"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.2.4.1.2 "><p id="p1218111991115"><a name="p1218111991115"></a><a name="p1218111991115"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.49%" headers="mcps1.2.4.1.3 "><p id="p1421871991115"><a name="p1421871991115"></a><a name="p1421871991115"></a>版本状态，为如下3种：</p>
    <p id="p13218101961111"><a name="p13218101961111"></a><a name="p13218101961111"></a>CURRENT：表示该版本为主推版本</p>
    <p id="p8218619201113"><a name="p8218619201113"></a><a name="p8218619201113"></a>SUPPORTED：表示为老版本，但是现在还继续支持</p>
    <p id="p821891911116"><a name="p821891911116"></a><a name="p821891911116"></a>DEPRECATED：表示为废弃版本，存在后续删除的可能</p>
    </td>
    </tr>
    <tr id="row1621811911114"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.2.4.1.1 "><p id="p7218171951115"><a name="p7218171951115"></a><a name="p7218171951115"></a>updated</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.2.4.1.2 "><p id="p721841914112"><a name="p721841914112"></a><a name="p721841914112"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.49%" headers="mcps1.2.4.1.3 "><p id="p192181619151111"><a name="p192181619151111"></a><a name="p192181619151111"></a>版本发布时间，采用UTC时间表示。如v1发布的时间2018-05-30T15:00:00Z。</p>
    </td>
    </tr>
    <tr id="row1221831916112"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.2.4.1.1 "><p id="p172181619101116"><a name="p172181619101116"></a><a name="p172181619101116"></a>min_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.2.4.1.2 "><p id="p4218919111111"><a name="p4218919111111"></a><a name="p4218919111111"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.49%" headers="mcps1.2.4.1.3 "><p id="p10218619131113"><a name="p10218619131113"></a><a name="p10218619131113"></a>若该版本API支持微版本，则返回支持的最小微版本号，如果不支持微版本，则返回空。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 2**  links参数信息

    <a name="table122284216266"></a>
    <table><thead align="left"><tr id="row0222174292613"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1522204215262"><a name="p1522204215262"></a><a name="p1522204215262"></a>参数名</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.35%" id="mcps1.2.4.1.2"><p id="p1822294232612"><a name="p1822294232612"></a><a name="p1822294232612"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.65%" id="mcps1.2.4.1.3"><p id="p15222164218261"><a name="p15222164218261"></a><a name="p15222164218261"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row20222144212611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p5222242202619"><a name="p5222242202619"></a><a name="p5222242202619"></a>rel</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.2.4.1.2 "><p id="p10222114212268"><a name="p10222114212268"></a><a name="p10222114212268"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.2.4.1.3 "><p id="p142221942192619"><a name="p142221942192619"></a><a name="p142221942192619"></a>链接的描述</p>
    </td>
    </tr>
    <tr id="row722294217261"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p622254262619"><a name="p622254262619"></a><a name="p622254262619"></a>href</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.2.4.1.2 "><p id="p022224232615"><a name="p022224232615"></a><a name="p022224232615"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.2.4.1.3 "><p id="p19222124210263"><a name="p19222124210263"></a><a name="p19222124210263"></a>版本号查询链接</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "version": {
            "id": "v1",
            "links": [
                {
                    "href": "https://sdrs.localdomain.com/v1",
                    "rel": "self"
                }
            ],
            "status": "CURRENT",
            "updated": "2018-05-30T00:00:00Z",
            "version": "",
            "min_version": ""
        }
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


## 返回值<a name="section137651118151119"></a>

-   正常

    <a name="table47815180118"></a>
    <table><thead align="left"><tr id="row2021871915114"><th class="cellrowborder" valign="top" width="42.42%" id="mcps1.1.3.1.1"><p id="p4218171912116"><a name="p4218171912116"></a><a name="p4218171912116"></a>返回值</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.58%" id="mcps1.1.3.1.2"><p id="p17218171901115"><a name="p17218171901115"></a><a name="p17218171901115"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row22187190113"><td class="cellrowborder" valign="top" width="42.42%" headers="mcps1.1.3.1.1 "><p id="p921861921119"><a name="p921861921119"></a><a name="p921861921119"></a>200</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.1.3.1.2 "><p id="p72184190118"><a name="p72184190118"></a><a name="p72184190118"></a>服务器已接受请求。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   异常

    <a name="table2781151816113"></a>
    <table><thead align="left"><tr id="row32181419141115"><th class="cellrowborder" valign="top" width="43.43%" id="mcps1.1.3.1.1"><p id="p2218191916115"><a name="p2218191916115"></a><a name="p2218191916115"></a>返回值</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.57%" id="mcps1.1.3.1.2"><p id="p42181719201113"><a name="p42181719201113"></a><a name="p42181719201113"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row182185197119"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p321831961112"><a name="p321831961112"></a><a name="p321831961112"></a>400 Bad Request</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p1321821981115"><a name="p1321821981115"></a><a name="p1321821981115"></a>服务器未能处理请求。</p>
    </td>
    </tr>
    <tr id="row19218161918116"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p7218151921111"><a name="p7218151921111"></a><a name="p7218151921111"></a>401 Unauthorized</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p112182191113"><a name="p112182191113"></a><a name="p112182191113"></a>被请求的页面需要用户名和密码。</p>
    </td>
    </tr>
    <tr id="row18218121921120"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p17218171918111"><a name="p17218171918111"></a><a name="p17218171918111"></a>403 Forbidden</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p15218131981117"><a name="p15218131981117"></a><a name="p15218131981117"></a>对被请求页面的访问被禁止。</p>
    </td>
    </tr>
    <tr id="row521811913111"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p20218181913113"><a name="p20218181913113"></a><a name="p20218181913113"></a>404 Not Found</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p18218101971117"><a name="p18218101971117"></a><a name="p18218101971117"></a>服务器无法找到被请求的页面。</p>
    </td>
    </tr>
    <tr id="row1821816197114"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p921817196119"><a name="p921817196119"></a><a name="p921817196119"></a>405 Method Not Allowed</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p4218171991118"><a name="p4218171991118"></a><a name="p4218171991118"></a>请求中指定的方法不被允许。</p>
    </td>
    </tr>
    <tr id="row20218151921115"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p5218519181114"><a name="p5218519181114"></a><a name="p5218519181114"></a>406 Not Acceptable</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p182189191114"><a name="p182189191114"></a><a name="p182189191114"></a>服务器生成的响应无法被客户端所接受。</p>
    </td>
    </tr>
    <tr id="row172182198112"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p22184191112"><a name="p22184191112"></a><a name="p22184191112"></a>407 Proxy Authentication Required</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p192181419141118"><a name="p192181419141118"></a><a name="p192181419141118"></a>用户必须首先使用代理服务器进行验证，这样请求才会被处理。</p>
    </td>
    </tr>
    <tr id="row32185197110"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p1721891911120"><a name="p1721891911120"></a><a name="p1721891911120"></a>408 Request Timeout</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p17218131971114"><a name="p17218131971114"></a><a name="p17218131971114"></a>请求超出了服务器的等待时间。</p>
    </td>
    </tr>
    <tr id="row62181319191115"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p921831911118"><a name="p921831911118"></a><a name="p921831911118"></a>409 Conflict</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p162181619201111"><a name="p162181619201111"></a><a name="p162181619201111"></a>由于冲突，请求无法被完成。</p>
    </td>
    </tr>
    <tr id="row1021820196115"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p18218141920118"><a name="p18218141920118"></a><a name="p18218141920118"></a>500 Internal Server Error</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p52181219191119"><a name="p52181219191119"></a><a name="p52181219191119"></a>请求未完成。服务异常。</p>
    </td>
    </tr>
    <tr id="row1421811911112"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p2021819197116"><a name="p2021819197116"></a><a name="p2021819197116"></a>501 Not Implemented</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p1821851941119"><a name="p1821851941119"></a><a name="p1821851941119"></a>请求未完成。服务器不支持所请求的功能。</p>
    </td>
    </tr>
    <tr id="row13218219151119"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p22183198114"><a name="p22183198114"></a><a name="p22183198114"></a>502 Bad Gateway</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p2021811913118"><a name="p2021811913118"></a><a name="p2021811913118"></a>请求未完成。服务器从上游服务器收到一个无效的响应。</p>
    </td>
    </tr>
    <tr id="row192180191118"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p921831991110"><a name="p921831991110"></a><a name="p921831991110"></a>503 Service Unavailable</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p22181196111"><a name="p22181196111"></a><a name="p22181196111"></a>请求未完成。系统暂时异常。</p>
    </td>
    </tr>
    <tr id="row8218119181114"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p1321814199113"><a name="p1321814199113"></a><a name="p1321814199113"></a>504 Gateway Timeout</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p02181319141114"><a name="p02181319141114"></a><a name="p02181319141114"></a>网关超时。</p>
    </td>
    </tr>
    </tbody>
    </table>


