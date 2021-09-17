# API概览<a name="sdrs_02_0000"></a>

存储容灾服务所提供的接口均为扩展接口。

通过使用SDRS接口，您可以完整的使用存储容灾服务的所有功能。

**表 1**  接口说明

<a name="zh-cn_topic_0121588224_table5876102613294"></a>
<table><thead align="left"><tr id="zh-cn_topic_0121588224_row3878122616298"><th class="cellrowborder" valign="top" width="22.900000000000002%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0121588224_p68781126182914"><a name="zh-cn_topic_0121588224_p68781126182914"></a><a name="zh-cn_topic_0121588224_p68781126182914"></a><strong id="zh-cn_topic_0121588224_b125201844173712"><a name="zh-cn_topic_0121588224_b125201844173712"></a><a name="zh-cn_topic_0121588224_b125201844173712"></a>接口类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="77.10000000000001%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0121588224_p158781726112914"><a name="zh-cn_topic_0121588224_p158781726112914"></a><a name="zh-cn_topic_0121588224_p158781726112914"></a><strong id="zh-cn_topic_0121588224_b15203449370"><a name="zh-cn_topic_0121588224_b15203449370"></a><a name="zh-cn_topic_0121588224_b15203449370"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0121588224_row148781026122919"><td class="cellrowborder" valign="top" width="22.900000000000002%" headers="mcps1.2.3.1.1 "><p id="p73459108266"><a name="p73459108266"></a><a name="p73459108266"></a><a href="Job管理.md">Job管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="77.10000000000001%" headers="mcps1.2.3.1.2 "><p id="p73450100260"><a name="p73450100260"></a><a name="p73450100260"></a>对于创建保护组、删除保护组、创建保护实例、删除保护实例、创建复制对、删除复制对等异步API，命令下发后，会返回job_id，通过job_id可以查询任务的执行状态。</p>
</td>
</tr>
<tr id="row14820164122810"><td class="cellrowborder" valign="top" width="22.900000000000002%" headers="mcps1.2.3.1.1 "><p id="p14822641112817"><a name="p14822641112817"></a><a name="p14822641112817"></a><a href="API版本信息.md">API版本信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="77.10000000000001%" headers="mcps1.2.3.1.2 "><p id="p5822174132816"><a name="p5822174132816"></a><a name="p5822174132816"></a>查询SDRS API版本信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0121588224_row1987820263297"><td class="cellrowborder" valign="top" width="22.900000000000002%" headers="mcps1.2.3.1.1 "><p id="p7481141134815"><a name="p7481141134815"></a><a name="p7481141134815"></a><a href="查询双活域.md">查询双活域</a></p>
</td>
<td class="cellrowborder" valign="top" width="77.10000000000001%" headers="mcps1.2.3.1.2 "><p id="p14753711352"><a name="p14753711352"></a><a name="p14753711352"></a>双活域由本端存储设备、远端存储设备组成，通过双活域，应用服务器可以实现跨站点的数据访问。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121588224_row87746166614"><td class="cellrowborder" valign="top" width="22.900000000000002%" headers="mcps1.2.3.1.1 "><p id="p234531013261"><a name="p234531013261"></a><a name="p234531013261"></a><a href="保护组.md">保护组</a></p>
</td>
<td class="cellrowborder" valign="top" width="77.10000000000001%" headers="mcps1.2.3.1.2 "><p id="p12201619124211"><a name="p12201619124211"></a><a name="p12201619124211"></a>用于管理一组需要复制的弹性云服务器。一个保护组可以管理一个虚拟私有云下的弹性云服务器，租户拥有多个虚拟私有云时则需要创建多个保护组。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121588224_row816313459617"><td class="cellrowborder" valign="top" width="22.900000000000002%" headers="mcps1.2.3.1.1 "><p id="p17318315135112"><a name="p17318315135112"></a><a name="p17318315135112"></a><a href="保护实例.md">保护实例</a></p>
</td>
<td class="cellrowborder" valign="top" width="77.10000000000001%" headers="mcps1.2.3.1.2 "><p id="p12709141823514"><a name="p12709141823514"></a><a name="p12709141823514"></a>保护实例是一对拥有复制关系的弹性云服务器。保护实例仅属于一个特定的保护组，因此这对弹性云服务器所在位置与保护组的生产站点或容灾站点相同。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121588224_row132213492619"><td class="cellrowborder" valign="top" width="22.900000000000002%" headers="mcps1.2.3.1.1 "><p id="p7345510142613"><a name="p7345510142613"></a><a name="p7345510142613"></a><a href="复制对.md">复制对</a></p>
</td>
<td class="cellrowborder" valign="top" width="77.10000000000001%" headers="mcps1.2.3.1.2 "><p id="p83991449114215"><a name="p83991449114215"></a><a name="p83991449114215"></a>复制对是一对拥有复制关系的云硬盘。复制对仅属于一个特定的保护组，且可以挂载给同一个保护组下的保护实例。</p>
</td>
</tr>
<tr id="row4363211307"><td class="cellrowborder" valign="top" width="22.900000000000002%" headers="mcps1.2.3.1.1 "><p id="p82313481302"><a name="p82313481302"></a><a name="p82313481302"></a><a href="容灾演练.md">容灾演练</a></p>
</td>
<td class="cellrowborder" valign="top" width="77.10000000000001%" headers="mcps1.2.3.1.2 "><p id="p223194863011"><a name="p223194863011"></a><a name="p223194863011"></a>容灾演练是为了确保一旦发生故障切换后，容灾机能够正常接管业务而进行的操作。</p>
</td>
</tr>
<tr id="row7254203311302"><td class="cellrowborder" valign="top" width="22.900000000000002%" headers="mcps1.2.3.1.1 "><p id="p22541433183020"><a name="p22541433183020"></a><a name="p22541433183020"></a><a href="标签管理.md">标签管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="77.10000000000001%" headers="mcps1.2.3.1.2 "><p id="p1025463319307"><a name="p1025463319307"></a><a name="p1025463319307"></a>标签是保护实例层面的标识，可以使用标签对保护实例进行分组等。</p>
</td>
</tr>
<tr id="row13844203715309"><td class="cellrowborder" valign="top" width="22.900000000000002%" headers="mcps1.2.3.1.1 "><p id="p58441437143014"><a name="p58441437143014"></a><a name="p58441437143014"></a><a href="任务中心.md">任务中心</a></p>
</td>
<td class="cellrowborder" valign="top" width="77.10000000000001%" headers="mcps1.2.3.1.2 "><p id="p2844337193010"><a name="p2844337193010"></a><a name="p2844337193010"></a>任务中心用于管理所有保护组失败任务或者指定保护组下的所有失败任务。</p>
</td>
</tr>
<tr id="row055219322487"><td class="cellrowborder" valign="top" width="22.900000000000002%" headers="mcps1.2.3.1.1 "><p id="p15541532184818"><a name="p15541532184818"></a><a name="p15541532184818"></a><a href="大屏管理.md">大屏管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="77.10000000000001%" headers="mcps1.2.3.1.2 "><p id="p5554163214818"><a name="p5554163214818"></a><a name="p5554163214818"></a>查询当前租户大屏显示中，资源的RPO超标趋势记录列表。</p>
</td>
</tr>
<tr id="row13156184812615"><td class="cellrowborder" valign="top" width="22.900000000000002%" headers="mcps1.2.3.1.1 "><p id="p1256119534920"><a name="p1256119534920"></a><a name="p1256119534920"></a><a href="租户配额管理.md">租户配额管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="77.10000000000001%" headers="mcps1.2.3.1.2 "><p id="p715619482260"><a name="p715619482260"></a><a name="p715619482260"></a>查询租户配额信息。</p>
</td>
</tr>
</tbody>
</table>

