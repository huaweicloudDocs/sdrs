# 查询job状态<a name="sdrs_05_0101"></a>

## 功能介绍<a name="zh-cn_topic_0079693002_section34649765"></a>

查询job的执行状态。

>![](public_sys-resources/icon-note.gif) **说明：** 
>对于创建保护组、删除保护组、创建保护实例、删除保护实例、创建复制对、删除复制对等异步API，命令下发后，会返回job\_id，通过job\_id可以查询任务的执行状态。

## URI<a name="zh-cn_topic_0079693002_section39390935"></a>

-   URI格式

    GET /v1/\{project\_id\}/jobs/\{job\_id\}

-   参数说明

    <a name="zh-cn_topic_0079693002_table63321005"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0079693002_row37593218"><th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0079693002_p25151854"><a name="zh-cn_topic_0079693002_p25151854"></a><a name="zh-cn_topic_0079693002_p25151854"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0079693002_p1556805116115"><a name="zh-cn_topic_0079693002_p1556805116115"></a><a name="zh-cn_topic_0079693002_p1556805116115"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="17%" id="mcps1.1.5.1.3"><p id="p553795612375"><a name="p553795612375"></a><a name="p553795612375"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="43%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0079693002_p2565159161120"><a name="zh-cn_topic_0079693002_p2565159161120"></a><a name="zh-cn_topic_0079693002_p2565159161120"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0079693002_row29123463"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0079693002_p10190321"><a name="zh-cn_topic_0079693002_p10190321"></a><a name="zh-cn_topic_0079693002_p10190321"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0079693002_p60774950161114"><a name="zh-cn_topic_0079693002_p60774950161114"></a><a name="zh-cn_topic_0079693002_p60774950161114"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.3 "><p id="p721813347387"><a name="p721813347387"></a><a name="p721813347387"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43%" headers="mcps1.1.5.1.4 "><p id="p15928101713314"><a name="p15928101713314"></a><a name="p15928101713314"></a>项目ID。</p>
    <p id="p1011411112497"><a name="p1011411112497"></a><a name="p1011411112497"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row91209154712"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.1 "><p id="p1212115134718"><a name="p1212115134718"></a><a name="p1212115134718"></a>job_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p191216112478"><a name="p191216112478"></a><a name="p191216112478"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.3 "><p id="p1921893473817"><a name="p1921893473817"></a><a name="p1921893473817"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43%" headers="mcps1.1.5.1.4 "><p id="p560514594492"><a name="p560514594492"></a><a name="p560514594492"></a>job ID。</p>
    <p id="p265974419244"><a name="p265974419244"></a><a name="p265974419244"></a>执行异步API命令下发后的返回参数，详见<a href="#zh-cn_topic_0079693002_section34649765">功能介绍</a>说明部分。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="zh-cn_topic_0079693002_section18974100"></a>

-   请求参数

    无

-   请求样例

    GET https://\{endpoint\}/v1/\{project\_id\}/jobs/0000000062db92d70162db9d200f000a


## 响应消息<a name="zh-cn_topic_0079693002_section36549175"></a>

-   要素说明

    <a name="table155991608555"></a>
    <table><thead align="left"><tr id="row460510055518"><th class="cellrowborder" valign="top" width="22.62%" id="mcps1.1.4.1.1"><p id="p56078010555"><a name="p56078010555"></a><a name="p56078010555"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.05%" id="mcps1.1.4.1.2"><p id="p961219016552"><a name="p961219016552"></a><a name="p961219016552"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="58.330000000000005%" id="mcps1.1.4.1.3"><p id="p186139012557"><a name="p186139012557"></a><a name="p186139012557"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row86164025512"><td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.1 "><p id="p261990195515"><a name="p261990195515"></a><a name="p261990195515"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.2 "><p id="p5556811164115"><a name="p5556811164115"></a><a name="p5556811164115"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="p12625170165512"><a name="p12625170165512"></a><a name="p12625170165512"></a>Job的状态。</p>
    <a name="ul1762511012556"></a><a name="ul1762511012556"></a><ul id="ul1762511012556"><li>SUCCESS：成功。</li><li>RUNNING：运行中。</li><li>FAIL：失败。</li><li>INIT：正在初始化。</li></ul>
    </td>
    </tr>
    <tr id="row166368013553"><td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.1 "><p id="p1663817020550"><a name="p1663817020550"></a><a name="p1663817020550"></a>entities</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.2 "><p id="p35586114418"><a name="p35586114418"></a><a name="p35586114418"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="p15224935105313"><a name="p15224935105313"></a><a name="p15224935105313"></a>Job操作的对象。</p>
    <p id="p1164518018558"><a name="p1164518018558"></a><a name="p1164518018558"></a>根据不同Job类型，显示不同的内容，保护组相关操作显示server_group_id，有子Job时为子job的详情。</p>
    <p id="p107581428152713"><a name="p107581428152713"></a><a name="p107581428152713"></a>详情请参见<a href="#table503353570">表1</a>。</p>
    </td>
    </tr>
    <tr id="row11646110135510"><td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.1 "><p id="p06481100551"><a name="p06481100551"></a><a name="p06481100551"></a>job_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.2 "><p id="p16558171194112"><a name="p16558171194112"></a><a name="p16558171194112"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="p1665417018555"><a name="p1665417018555"></a><a name="p1665417018555"></a>Job ID。</p>
    <p id="p040832117517"><a name="p040832117517"></a><a name="p040832117517"></a>详见<a href="#zh-cn_topic_0079693002_section34649765">功能介绍</a>说明部分。</p>
    </td>
    </tr>
    <tr id="row6655401556"><td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.1 "><p id="p18657190125511"><a name="p18657190125511"></a><a name="p18657190125511"></a>job_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.2 "><p id="p1755816116411"><a name="p1755816116411"></a><a name="p1755816116411"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="p36630014558"><a name="p36630014558"></a><a name="p36630014558"></a>Job的类型。</p>
    <a name="ul127879407557"></a><a name="ul127879407557"></a><ul id="ul127879407557"><li>createProtectionGroupNoCG：创建保护组。</li><li>deleteProtectionGroupNoCG：删除保护组。</li><li>startProtectionGroupNoCG ：保护组开始保护。</li><li>reprotectProtectionGroupNoCG ：保护组重保护。</li><li>stopProtectionGroupNoCG ：保护组停止保护。</li><li>failoverProtectionGroupNoCG  ：保护组故障切换。</li><li>reverseProtectionGroupNoCG：保护组切换。</li><li>createProtectedInstanceNoCG：创建保护实例。</li><li>deleteProtectedInstanceNoCG：删除保护实例。</li><li>attachReplicationPairNew：保护实例挂载复制对。</li><li>detachReplicationPairNew：保护实例卸载复制对。</li><li>addNicNew：保护实例添加网卡。</li><li>deleteNicNew：保护实例删除网卡。</li><li>resizeProtectedInstanceNew：保护实例变更规格。</li><li>createReplicationPairNoCG：创建复制对。</li><li>deleteReplicationPairNoCG：删除复制对。</li><li>expandReplicationPairNew：复制对扩容。</li><li>createDisasterRecoveryDrill：创建容灾演练。</li><li>deleteDisasterRecoveryDrill：删除容灾演练。</li></ul>
    </td>
    </tr>
    <tr id="row156647095510"><td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.1 "><p id="p156667025512"><a name="p156667025512"></a><a name="p156667025512"></a>begin_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.2 "><p id="p3558311194119"><a name="p3558311194119"></a><a name="p3558311194119"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="p178851320123117"><a name="p178851320123117"></a><a name="p178851320123117"></a>开始时间。</p>
    <p id="p1867150115511"><a name="p1867150115511"></a><a name="p1867150115511"></a>默认格式为："yyyy-MM-dd'T'HH:mm:ss.SSSZ"，例："2019-04-01T12:00:00.000Z"。</p>
    </td>
    </tr>
    <tr id="row7672100175511"><td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.1 "><p id="p166749095519"><a name="p166749095519"></a><a name="p166749095519"></a>end_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.2 "><p id="p1955819111411"><a name="p1955819111411"></a><a name="p1955819111411"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="p075417312316"><a name="p075417312316"></a><a name="p075417312316"></a>结束时间。</p>
    <p id="p20679150115516"><a name="p20679150115516"></a><a name="p20679150115516"></a>默认格式为："yyyy-MM-dd'T'HH:mm:ss.SSSZ"，例："2019-04-01T12:00:00.000Z"。</p>
    </td>
    </tr>
    <tr id="row19681100205515"><td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.1 "><p id="p1368312010554"><a name="p1368312010554"></a><a name="p1368312010554"></a>error_code</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.2 "><p id="p135587111415"><a name="p135587111415"></a><a name="p135587111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="p18690103557"><a name="p18690103557"></a><a name="p18690103557"></a>Job执行失败时的错误码。</p>
    <p id="p43101514454"><a name="p43101514454"></a><a name="p43101514454"></a>详见<a href="错误码.md">错误码</a>。</p>
    </td>
    </tr>
    <tr id="row156911205555"><td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.1 "><p id="p1269312045516"><a name="p1269312045516"></a><a name="p1269312045516"></a>fail_reason</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.2 "><p id="p155801114116"><a name="p155801114116"></a><a name="p155801114116"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="p76991106554"><a name="p76991106554"></a><a name="p76991106554"></a>Job执行失败时的错误原因。</p>
    <p id="p529416112003"><a name="p529416112003"></a><a name="p529416112003"></a>详见<a href="错误码.md">错误码</a>。</p>
    </td>
    </tr>
    <tr id="row6699110115516"><td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.1 "><p id="p19701002556"><a name="p19701002556"></a><a name="p19701002556"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.2 "><p id="p055891174110"><a name="p055891174110"></a><a name="p055891174110"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="p77073010553"><a name="p77073010553"></a><a name="p77073010553"></a>出现错误时，返回的错误信息。</p>
    <p id="p20141415287"><a name="p20141415287"></a><a name="p20141415287"></a>详见<a href="#zh-cn_topic_0079693002_section60507121">返回值</a>异常码。</p>
    </td>
    </tr>
    <tr id="row37089012553"><td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.1 "><p id="p171060155514"><a name="p171060155514"></a><a name="p171060155514"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.2 "><p id="p65582011144113"><a name="p65582011144113"></a><a name="p65582011144113"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="p1771615045517"><a name="p1771615045517"></a><a name="p1771615045517"></a>出现错误时，返回的错误码。</p>
    <p id="p143705412551"><a name="p143705412551"></a><a name="p143705412551"></a>详见<a href="#zh-cn_topic_0079693002_section60507121">返回值</a>异常码。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 1**  entities字段说明

    <a name="table503353570"></a>
    <table><thead align="left"><tr id="row131163505710"><th class="cellrowborder" valign="top" width="23.810000000000002%" id="mcps1.2.4.1.1"><p id="p8131435155711"><a name="p8131435155711"></a><a name="p8131435155711"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.86%" id="mcps1.2.4.1.2"><p id="p6251035195718"><a name="p6251035195718"></a><a name="p6251035195718"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="58.330000000000005%" id="mcps1.2.4.1.3"><p id="p1727173517574"><a name="p1727173517574"></a><a name="p1727173517574"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1829133585715"><td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.1 "><p id="p13393545711"><a name="p13393545711"></a><a name="p13393545711"></a>server_group_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.86%" headers="mcps1.2.4.1.2 "><p id="p113643525715"><a name="p113643525715"></a><a name="p113643525715"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.2.4.1.3 "><p id="p13896133075915"><a name="p13896133075915"></a><a name="p13896133075915"></a>保护组相关操作显示保护组ID。</p>
    </td>
    </tr>
    <tr id="row951117394485"><td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.2.4.1.1 "><p id="p239893649137"><a name="p239893649137"></a><a name="p239893649137"></a>sub_jobs</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.86%" headers="mcps1.2.4.1.2 "><p id="p640903559137"><a name="p640903559137"></a><a name="p640903559137"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.2.4.1.3 "><p id="p597890789137"><a name="p597890789137"></a><a name="p597890789137"></a>每个子job的执行信息。没有子job时为空列表。每个子job的结构与父job类似。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {  
          "status": "SUCCESS",  
          "entities": {  
              "server_group_id": "a59d008e-4bad-4bf3-9b17-6cc25e7da483"  
          },  
          "job_id": "0000000062db92d70162db9d200f000a",  
          "job_type": "createProtectionGroupNoCG",  
          "begin_time": "2018-04-19T01:55:30.443Z",  
          "end_time": "2018-04-19T01:55:45.493Z",  
          "error_code": null,  
          "fail_reason": null  
      }
    ```

    或

    ```
    {
        "job_id": "ff8080826b45d4a5016b5036242c0025",
        "job_type": "stopProtectionGroupNoCG",
        "begin_time": "2019-06-13T09:40:53.930Z",
        "end_time": "2019-06-13T09:41:01.946Z",
        "status": "SUCCESS",
        "error_code": null,
        "fail_reason": null,
        "entities": {
            "sub_jobs": [
                {
                    "job_id": "ff8080826b45d4a5016b50362868002a",
                    "job_type": "stopProtectionGroupRepNoCG",
                    "begin_time": "2019-06-13T09:40:55.015Z",
                    "end_time": "2019-06-13T09:40:58.951Z",
                    "status": "SUCCESS",
                    "error_code": null,
                    "fail_reason": null,
                    "entities": {
                        "server_group_id": "1fd6903c-48f9-4772-8974-112dfbd74427"
                    }
                },
                {
                    "job_id": "ff8080826b45d4a5016b50362870002b",
                    "job_type": "stopProtectionGroupRepNoCG",
                    "begin_time": "2019-06-13T09:40:55.022Z",
                    "end_time": "2019-06-13T09:40:58.952Z",
                    "status": "SUCCESS",
                    "error_code": null,
                    "fail_reason": null,
                    "entities": {
                        "server_group_id": "1fd6903c-48f9-4772-8974-112dfbd74427"
                    }
                }
            ]
        }
    }
    { 
         "error": { 
             "message": "XXXX",  
             "code": "XXX" 
         } 
     }
    ```


## 返回值<a name="zh-cn_topic_0079693002_section60507121"></a>

-   正常

    <a name="table4315991194956"></a>
    <table><thead align="left"><tr id="row2336641294956"><th class="cellrowborder" valign="top" width="42.59%" id="mcps1.1.3.1.1"><p id="p1363125894956"><a name="p1363125894956"></a><a name="p1363125894956"></a>返回值</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.410000000000004%" id="mcps1.1.3.1.2"><p id="p3039012494956"><a name="p3039012494956"></a><a name="p3039012494956"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row507566794956"><td class="cellrowborder" valign="top" width="42.59%" headers="mcps1.1.3.1.1 "><p id="p847584694956"><a name="p847584694956"></a><a name="p847584694956"></a>200</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.410000000000004%" headers="mcps1.1.3.1.2 "><p id="p1545496394956"><a name="p1545496394956"></a><a name="p1545496394956"></a>服务器已接受请求。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   异常

    <a name="table22458872203835"></a>
    <table><thead align="left"><tr id="row35704554203835"><th class="cellrowborder" valign="top" width="43.419999999999995%" id="mcps1.1.3.1.1"><p id="p6387753203835"><a name="p6387753203835"></a><a name="p6387753203835"></a>返回值</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.58%" id="mcps1.1.3.1.2"><p id="p47646009203835"><a name="p47646009203835"></a><a name="p47646009203835"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row34121538203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p12381163203835"><a name="p12381163203835"></a><a name="p12381163203835"></a>400 Bad Request</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p63350108203835"><a name="p63350108203835"></a><a name="p63350108203835"></a>服务器未能处理请求。</p>
    </td>
    </tr>
    <tr id="row33280063203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p11330608203835"><a name="p11330608203835"></a><a name="p11330608203835"></a>401 Unauthorized</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p45364094203835"><a name="p45364094203835"></a><a name="p45364094203835"></a>被请求的页面需要用户名和密码。</p>
    </td>
    </tr>
    <tr id="row5623667203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p52863895203835"><a name="p52863895203835"></a><a name="p52863895203835"></a>403 Forbidden</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p54117066203835"><a name="p54117066203835"></a><a name="p54117066203835"></a>对被请求页面的访问被禁止。</p>
    </td>
    </tr>
    <tr id="row17291554203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p58438642203835"><a name="p58438642203835"></a><a name="p58438642203835"></a>404 Not Found</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p35909542203835"><a name="p35909542203835"></a><a name="p35909542203835"></a>服务器无法找到被请求的页面。</p>
    </td>
    </tr>
    <tr id="row54750425203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p5599455203835"><a name="p5599455203835"></a><a name="p5599455203835"></a>405 Method Not Allowed</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p50902717203835"><a name="p50902717203835"></a><a name="p50902717203835"></a>请求中指定的方法不被允许。</p>
    </td>
    </tr>
    <tr id="row55471277203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p63988484203835"><a name="p63988484203835"></a><a name="p63988484203835"></a>406 Not Acceptable</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p15684678203835"><a name="p15684678203835"></a><a name="p15684678203835"></a>服务器生成的响应无法被客户端所接受。</p>
    </td>
    </tr>
    <tr id="row6944380203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p25623884203835"><a name="p25623884203835"></a><a name="p25623884203835"></a>407 Proxy Authentication Required</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p62268733203835"><a name="p62268733203835"></a><a name="p62268733203835"></a>用户必须首先使用代理服务器进行验证，这样请求才会被处理。</p>
    </td>
    </tr>
    <tr id="row23547689203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p28314670203835"><a name="p28314670203835"></a><a name="p28314670203835"></a>408 Request Timeout</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p11786919203835"><a name="p11786919203835"></a><a name="p11786919203835"></a>请求超出了服务器的等待时间。</p>
    </td>
    </tr>
    <tr id="row38973411203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p2729702203835"><a name="p2729702203835"></a><a name="p2729702203835"></a>409 Conflict</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p19779281203835"><a name="p19779281203835"></a><a name="p19779281203835"></a>由于冲突，请求无法被完成。</p>
    </td>
    </tr>
    <tr id="row43795805203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p57799353203835"><a name="p57799353203835"></a><a name="p57799353203835"></a>500 Internal Server Error</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p51235984203835"><a name="p51235984203835"></a><a name="p51235984203835"></a>请求未完成。服务异常。</p>
    </td>
    </tr>
    <tr id="row58470678203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p38504500203835"><a name="p38504500203835"></a><a name="p38504500203835"></a>501 Not Implemented</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p31856770203835"><a name="p31856770203835"></a><a name="p31856770203835"></a>请求未完成。服务器不支持所请求的功能。</p>
    </td>
    </tr>
    <tr id="row18275474203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p3918444203835"><a name="p3918444203835"></a><a name="p3918444203835"></a>502 Bad Gateway</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p48958538203835"><a name="p48958538203835"></a><a name="p48958538203835"></a>请求未完成。服务器从上游服务器收到一个无效的响应。</p>
    </td>
    </tr>
    <tr id="row37973662203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p55967806203835"><a name="p55967806203835"></a><a name="p55967806203835"></a>503 Service Unavailable</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p37098455203835"><a name="p37098455203835"></a><a name="p37098455203835"></a>请求未完成。系统暂时异常。</p>
    </td>
    </tr>
    <tr id="row65450640203835"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p67010448203835"><a name="p67010448203835"></a><a name="p67010448203835"></a>504 Gateway Timeout</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p59137180203835"><a name="p59137180203835"></a><a name="p59137180203835"></a>网关超时。</p>
    </td>
    </tr>
    </tbody>
    </table>


