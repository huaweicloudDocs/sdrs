# 查询API版本信息<a name="ZH-CN_TOPIC_0133405736"></a>

## 功能介绍<a name="section15202175015916"></a>

查询存储容灾当前所有可用的版本信息列表。

## 接口限制<a name="section2218250892"></a>

无

## URI<a name="section102186501492"></a>

-   URI格式

    GET  /


## 请求消息<a name="section122189507911"></a>

-   参数说明

    无

-   请求样例

    GET https://\{endpoint\}/


## 响应消息<a name="section1921820506915"></a>

-   要素说明

    <a name="table182331050591"></a>
    <table><thead align="left"><tr id="row175301150797"><th class="cellrowborder" valign="top" width="29.07%" id="mcps1.1.4.1.1"><p id="p65303501498"><a name="p65303501498"></a><a name="p65303501498"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.44%" id="mcps1.1.4.1.2"><p id="p195302503918"><a name="p195302503918"></a><a name="p195302503918"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.49%" id="mcps1.1.4.1.3"><p id="p35303501793"><a name="p35303501793"></a><a name="p35303501793"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1153012501194"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.1.4.1.1 "><p id="p19530550193"><a name="p19530550193"></a><a name="p19530550193"></a>versions</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.1.4.1.2 "><p id="p175301150093"><a name="p175301150093"></a><a name="p175301150093"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.49%" headers="mcps1.1.4.1.3 "><p id="p12530250298"><a name="p12530250298"></a><a name="p12530250298"></a>API版本信息列表。</p>
    <p id="p1292113616103"><a name="p1292113616103"></a><a name="p1292113616103"></a>详细参数请参考<a href="#table11250550892">表1</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 1**  versions字段说明

    <a name="table11250550892"></a>
    <table><thead align="left"><tr id="row195307501295"><th class="cellrowborder" valign="top" width="29.07%" id="mcps1.2.4.1.1"><p id="p65307506917"><a name="p65307506917"></a><a name="p65307506917"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.43%" id="mcps1.2.4.1.2"><p id="p653045013912"><a name="p653045013912"></a><a name="p653045013912"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.5%" id="mcps1.2.4.1.3"><p id="p253035016913"><a name="p253035016913"></a><a name="p253035016913"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row553075018919"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.2.4.1.1 "><p id="p165302507919"><a name="p165302507919"></a><a name="p165302507919"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.2.4.1.2 "><p id="p1853012503910"><a name="p1853012503910"></a><a name="p1853012503910"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.5%" headers="mcps1.2.4.1.3 "><p id="p65307507916"><a name="p65307507916"></a><a name="p65307507916"></a>版本ID（版本号），如v1。</p>
    </td>
    </tr>
    <tr id="row1953016501699"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.2.4.1.1 "><p id="p953010504914"><a name="p953010504914"></a><a name="p953010504914"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.2.4.1.2 "><p id="p9530155016912"><a name="p9530155016912"></a><a name="p9530155016912"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.5%" headers="mcps1.2.4.1.3 "><p id="p165306504911"><a name="p165306504911"></a><a name="p165306504911"></a>API的URL地址。</p>
    <p id="p79618574411"><a name="p79618574411"></a><a name="p79618574411"></a>详细参数请参考<a href="#zh-cn_topic_0060111075_table35183803523">表2</a>。</p>
    </td>
    </tr>
    <tr id="row55302504916"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.2.4.1.1 "><p id="p0530115017910"><a name="p0530115017910"></a><a name="p0530115017910"></a>version</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.2.4.1.2 "><p id="p17530115019910"><a name="p17530115019910"></a><a name="p17530115019910"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.5%" headers="mcps1.2.4.1.3 "><p id="p853015501918"><a name="p853015501918"></a><a name="p853015501918"></a>若该版本API支持微版本，则返回支持的最大微版本号，如果不支持微版本，则返回空。</p>
    </td>
    </tr>
    <tr id="row1153012501910"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.2.4.1.1 "><p id="p55301850595"><a name="p55301850595"></a><a name="p55301850595"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.2.4.1.2 "><p id="p25301501498"><a name="p25301501498"></a><a name="p25301501498"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.5%" headers="mcps1.2.4.1.3 "><p id="p85304501993"><a name="p85304501993"></a><a name="p85304501993"></a>版本状态，为如下3种：</p>
    <p id="p853015502920"><a name="p853015502920"></a><a name="p853015502920"></a>CURRENT：表示该版本为主推版本</p>
    <p id="p3530350293"><a name="p3530350293"></a><a name="p3530350293"></a>SUPPORTED：表示为老版本，但是现在还继续支持</p>
    <p id="p35306503917"><a name="p35306503917"></a><a name="p35306503917"></a>DEPRECATED：表示为废弃版本，存在后续删除的可能</p>
    </td>
    </tr>
    <tr id="row115307500919"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.2.4.1.1 "><p id="p15308501693"><a name="p15308501693"></a><a name="p15308501693"></a>updated</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.2.4.1.2 "><p id="p1530950391"><a name="p1530950391"></a><a name="p1530950391"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.5%" headers="mcps1.2.4.1.3 "><p id="p75306505917"><a name="p75306505917"></a><a name="p75306505917"></a>版本发布时间，采用UTC时间表示。如v1发布的时间2018-05-30T15:00:00Z。</p>
    </td>
    </tr>
    <tr id="row1530250795"><td class="cellrowborder" valign="top" width="29.07%" headers="mcps1.2.4.1.1 "><p id="p205307501896"><a name="p205307501896"></a><a name="p205307501896"></a>min_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.43%" headers="mcps1.2.4.1.2 "><p id="p1153014501496"><a name="p1153014501496"></a><a name="p1153014501496"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.5%" headers="mcps1.2.4.1.3 "><p id="p1653013501091"><a name="p1653013501091"></a><a name="p1653013501091"></a>若该版本API 支持微版本，则返回支持的最小微版本号，如果不支持微版本，则返回空。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 2**  links参数信息

    <a name="zh-cn_topic_0060111075_table35183803523"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0060111075_row1099838503523"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0060111075_p1845402603523"><a name="zh-cn_topic_0060111075_p1845402603523"></a><a name="zh-cn_topic_0060111075_p1845402603523"></a>参数名</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.35%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0060111075_p1838114303523"><a name="zh-cn_topic_0060111075_p1838114303523"></a><a name="zh-cn_topic_0060111075_p1838114303523"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.65%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0060111075_p405534303523"><a name="zh-cn_topic_0060111075_p405534303523"></a><a name="zh-cn_topic_0060111075_p405534303523"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0060111075_row3649809103523"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0060111075_p355541903523"><a name="zh-cn_topic_0060111075_p355541903523"></a><a name="zh-cn_topic_0060111075_p355541903523"></a>rel</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0060111075_p1955354003523"><a name="zh-cn_topic_0060111075_p1955354003523"></a><a name="zh-cn_topic_0060111075_p1955354003523"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0060111075_p4573756603523"><a name="zh-cn_topic_0060111075_p4573756603523"></a><a name="zh-cn_topic_0060111075_p4573756603523"></a>链接的描述</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0060111075_row898491303523"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0060111075_p5668937803523"><a name="zh-cn_topic_0060111075_p5668937803523"></a><a name="zh-cn_topic_0060111075_p5668937803523"></a>href</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0060111075_p2843694403523"><a name="zh-cn_topic_0060111075_p2843694403523"></a><a name="zh-cn_topic_0060111075_p2843694403523"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0060111075_p1215177703523"><a name="zh-cn_topic_0060111075_p1215177703523"></a><a name="zh-cn_topic_0060111075_p1215177703523"></a>版本号查询链接</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "versions": [
            {
                "id": "v1",
                "links": [
                    {
                        "href": "https://sdrs.localdomain.com/v1",
                        "rel": "self"
                    }
                ],
                "status": "CURRENT",
                "updated": "2018-05-30T15:00:00Z",
                "version": "",
                "min_version": ""
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


## 返回值<a name="section1280175013910"></a>

-   正常

    <a name="table1328075020914"></a>
    <table><thead align="left"><tr id="row353013501299"><th class="cellrowborder" valign="top" width="42.42%" id="mcps1.1.3.1.1"><p id="p4530350292"><a name="p4530350292"></a><a name="p4530350292"></a>返回值</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.58%" id="mcps1.1.3.1.2"><p id="p175301750497"><a name="p175301750497"></a><a name="p175301750497"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row553055014912"><td class="cellrowborder" valign="top" width="42.42%" headers="mcps1.1.3.1.1 "><p id="p553005012910"><a name="p553005012910"></a><a name="p553005012910"></a>200</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.1.3.1.2 "><p id="p95306501392"><a name="p95306501392"></a><a name="p95306501392"></a>服务器已接受请求。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   异常

    <a name="table182801579913"></a>
    <table><thead align="left"><tr id="row128011579913"><th class="cellrowborder" valign="top" width="43.43%" id="mcps1.1.3.1.1"><p id="p1328016571695"><a name="p1328016571695"></a><a name="p1328016571695"></a>返回值</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.57%" id="mcps1.1.3.1.2"><p id="p02801757990"><a name="p02801757990"></a><a name="p02801757990"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row628045712912"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p22809571991"><a name="p22809571991"></a><a name="p22809571991"></a>400 Bad Request</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p2028019571694"><a name="p2028019571694"></a><a name="p2028019571694"></a>服务器未能处理请求。</p>
    </td>
    </tr>
    <tr id="row10280105719915"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p182805576911"><a name="p182805576911"></a><a name="p182805576911"></a>401 Unauthorized</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p728019575910"><a name="p728019575910"></a><a name="p728019575910"></a>被请求的页面需要用户名和密码。</p>
    </td>
    </tr>
    <tr id="row152801571496"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p428013579918"><a name="p428013579918"></a><a name="p428013579918"></a>403 Forbidden</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p192801157095"><a name="p192801157095"></a><a name="p192801157095"></a>对被请求页面的访问被禁止。</p>
    </td>
    </tr>
    <tr id="row14280165716912"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p32801157596"><a name="p32801157596"></a><a name="p32801157596"></a>404 Not Found</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p428012575913"><a name="p428012575913"></a><a name="p428012575913"></a>服务器无法找到被请求的页面。</p>
    </td>
    </tr>
    <tr id="row152806579910"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p12280157491"><a name="p12280157491"></a><a name="p12280157491"></a>405 Method Not Allowed</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p14280957992"><a name="p14280957992"></a><a name="p14280957992"></a>请求中指定的方法不被允许。</p>
    </td>
    </tr>
    <tr id="row828015570910"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p92803570912"><a name="p92803570912"></a><a name="p92803570912"></a>406 Not Acceptable</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p2280457991"><a name="p2280457991"></a><a name="p2280457991"></a>服务器生成的响应无法被客户端所接受。</p>
    </td>
    </tr>
    <tr id="row828014573910"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p172801357397"><a name="p172801357397"></a><a name="p172801357397"></a>407 Proxy Authentication Required</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p182804578913"><a name="p182804578913"></a><a name="p182804578913"></a>用户必须首先使用代理服务器进行验证，这样请求才会被处理。</p>
    </td>
    </tr>
    <tr id="row02801857196"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p182801757394"><a name="p182801757394"></a><a name="p182801757394"></a>408 Request Timeout</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p1228014575913"><a name="p1228014575913"></a><a name="p1228014575913"></a>请求超出了服务器的等待时间。</p>
    </td>
    </tr>
    <tr id="row228035715917"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p1928019575911"><a name="p1928019575911"></a><a name="p1928019575911"></a>409 Conflict</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p11280135715913"><a name="p11280135715913"></a><a name="p11280135715913"></a>由于冲突，请求无法被完成。</p>
    </td>
    </tr>
    <tr id="row192806571191"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p9280145719917"><a name="p9280145719917"></a><a name="p9280145719917"></a>500 Internal Server Error</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p42806574918"><a name="p42806574918"></a><a name="p42806574918"></a>请求未完成。服务异常。</p>
    </td>
    </tr>
    <tr id="row52801557997"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p1728016571298"><a name="p1728016571298"></a><a name="p1728016571298"></a>501 Not Implemented</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p4280857797"><a name="p4280857797"></a><a name="p4280857797"></a>请求未完成。服务器不支持所请求的功能。</p>
    </td>
    </tr>
    <tr id="row112801057893"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p192801571095"><a name="p192801571095"></a><a name="p192801571095"></a>502 Bad Gateway</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p328045716919"><a name="p328045716919"></a><a name="p328045716919"></a>请求未完成。服务器从上游服务器收到一个无效的响应。</p>
    </td>
    </tr>
    <tr id="row728015571697"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p42801757490"><a name="p42801757490"></a><a name="p42801757490"></a>503 Service Unavailable</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p728015720916"><a name="p728015720916"></a><a name="p728015720916"></a>请求未完成。系统暂时异常。</p>
    </td>
    </tr>
    <tr id="row928075714911"><td class="cellrowborder" valign="top" width="43.43%" headers="mcps1.1.3.1.1 "><p id="p12807571690"><a name="p12807571690"></a><a name="p12807571690"></a>504 Gateway Timeout</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.1.3.1.2 "><p id="p12804571095"><a name="p12804571095"></a><a name="p12804571095"></a>网关超时。</p>
    </td>
    </tr>
    </tbody>
    </table>


