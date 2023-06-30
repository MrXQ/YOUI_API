# YOUICompass API


**简介**:YOUICompass API


**HOST**:192.168.1.214:8080


**联系人**:YOUIBOT


**Version**:4.8.3 RELEASE


**接口路径**:/v2/api-docs


[TOC]






# AGV


## 详情


**接口地址**:`/api/v3/agvs`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:详情


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AGV|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|deviceModel|设备型号|string||
|deviceNumber|设备编号|string||
|description|描述|string||
|defaultControlMode|开机默认控制模式 自动模式:1, 手动模式:2|integer(int32)|integer(int32)|
|navigationType|导航类型 LASER:激光导航 QR_CODE:二维码导航 BLEND:混合导航|string||
|agvMapId|当前使用的地图ID|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"deviceModel": "",
	"deviceNumber": "",
	"description": "",
	"defaultControlMode": 0,
	"navigationType": "",
	"agvMapId": "",
	"createTime": "",
	"updateTime": ""
}
```


## 回调测试


**接口地址**:`/api/v3/agvs/callback`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:回调测试


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|jsonObject|回调参数|body|true|JSONObject|JSONObject|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 更新


**接口地址**:`/api/v3/agvs/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:更新


**请求示例**:


```javascript
{
	"id": "",
	"name": "",
	"deviceModel": "",
	"deviceNumber": "",
	"description": "",
	"defaultControlMode": 0,
	"navigationType": "",
	"agvMapId": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|AGV|AGV||true|AGV|AGV|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;deviceModel|设备型号||false|string||
|&emsp;&emsp;deviceNumber|设备编号||false|string||
|&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;defaultControlMode|开机默认控制模式 自动模式:1, 手动模式:2||false|integer(int32)||
|&emsp;&emsp;navigationType|导航类型 LASER:激光导航 QR_CODE:二维码导航 BLEND:混合导航||false|string||
|&emsp;&emsp;agvMapId|当前使用的地图ID||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|agv|AGV|body|true|AGV|AGV|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;deviceModel|设备型号||false|string||
|&emsp;&emsp;deviceNumber|设备编号||false|string||
|&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;defaultControlMode|开机默认控制模式 自动模式:1, 手动模式:2||false|integer(int32)||
|&emsp;&emsp;navigationType|导航类型 LASER:激光导航 QR_CODE:二维码导航 BLEND:混合导航||false|string||
|&emsp;&emsp;agvMapId|当前使用的地图ID||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|id|机器人的ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AGV|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|deviceModel|设备型号|string||
|deviceNumber|设备编号|string||
|description|描述|string||
|defaultControlMode|开机默认控制模式 自动模式:1, 手动模式:2|integer(int32)|integer(int32)|
|navigationType|导航类型 LASER:激光导航 QR_CODE:二维码导航 BLEND:混合导航|string||
|agvMapId|当前使用的地图ID|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"deviceModel": "",
	"deviceNumber": "",
	"description": "",
	"defaultControlMode": 0,
	"navigationType": "",
	"agvMapId": "",
	"createTime": "",
	"updateTime": ""
}
```


# AGV路径导航参数


## 详情


**接口地址**:`/api/v3/AGVPathParams`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AGVPathParam|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|safety|避障 1、打开避障  2、关闭避障|integer(int32)|integer(int32)|
|max_translation_speed|最大平移速度 >0 m/s|number(double)|number(double)|
|max_rotate_speed|最大旋转速度 rad/s >0|number(double)|number(double)|
|P|平移加速比例控制系数 >0|number(double)|number(double)|
|D|平移加速微分控制系数 >0|number(double)|number(double)|
|translation_acc|平移加（减）速度 m/s2 >0|number(double)|number(double)|
|rotate_acc|旋转加（减）速度 rad/s2 >0|number(double)|number(double)|
|obstacle_avoidance|绕障 1、打开绕障  2、关闭绕障|integer(int32)|integer(int32)|
|obstacle_avoidance_timeout|避障超时时间（超时后AGV会自动绕障） 单位：秒|integer(int32)|integer(int32)|
|obstacle_avoidance_count|绕障总次数（超过总次数后路径导航报错）|integer(int32)|integer(int32)|
|accurate_stop|是否启用末端精定位: 0不启用 1启用，默认是不启用|integer(int32)|integer(int32)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|修改时间|string(date-time)|string(date-time)|
|extend_bit|拓展布尔|string||
|extend_string|拓展字符串|string||
|features_requested|融合特征 1、开启 0、关闭|integer(int32)|integer(int32)|
|safety_scanner_region|雷达避障区域 0、默认区域  1、避障区域1   2、避障区域2  .....  15、避障区域15|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"id": "",
	"safety": 0,
	"max_translation_speed": 0,
	"max_rotate_speed": 0,
	"P": 0,
	"D": 0,
	"translation_acc": 0,
	"rotate_acc": 0,
	"obstacle_avoidance": 0,
	"obstacle_avoidance_timeout": 0,
	"obstacle_avoidance_count": 0,
	"accurate_stop": 0,
	"createTime": "",
	"updateTime": "",
	"extend_bit": "",
	"extend_string": "",
	"features_requested": 0,
	"safety_scanner_region": 0
}
```


## 更新


**接口地址**:`/api/v3/AGVPathParams/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"safety": 0,
	"max_translation_speed": 0,
	"max_rotate_speed": 0,
	"P": 0,
	"D": 0,
	"translation_acc": 0,
	"rotate_acc": 0,
	"obstacle_avoidance": 0,
	"obstacle_avoidance_timeout": 0,
	"obstacle_avoidance_count": 0,
	"accurate_stop": 0,
	"createTime": "",
	"updateTime": "",
	"extend_bit": "",
	"extend_string": "",
	"features_requested": 0,
	"safety_scanner_region": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|agvPathParam|AGV路径导航参数|body|true|AGVPathParam|AGVPathParam|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;safety|避障 1、打开避障  2、关闭避障||false|integer(int32)||
|&emsp;&emsp;max_translation_speed|最大平移速度 >0 m/s||false|number(double)||
|&emsp;&emsp;max_rotate_speed|最大旋转速度 rad/s >0||false|number(double)||
|&emsp;&emsp;P|平移加速比例控制系数 >0||false|number(double)||
|&emsp;&emsp;D|平移加速微分控制系数 >0||false|number(double)||
|&emsp;&emsp;translation_acc|平移加（减）速度 m/s2 >0||false|number(double)||
|&emsp;&emsp;rotate_acc|旋转加（减）速度 rad/s2 >0||false|number(double)||
|&emsp;&emsp;obstacle_avoidance|绕障 1、打开绕障  2、关闭绕障||false|integer(int32)||
|&emsp;&emsp;obstacle_avoidance_timeout|避障超时时间（超时后AGV会自动绕障） 单位：秒||false|integer(int32)||
|&emsp;&emsp;obstacle_avoidance_count|绕障总次数（超过总次数后路径导航报错）||false|integer(int32)||
|&emsp;&emsp;accurate_stop|是否启用末端精定位: 0不启用 1启用，默认是不启用||false|integer(int32)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|修改时间||false|string(date-time)||
|&emsp;&emsp;extend_bit|拓展布尔||false|string||
|&emsp;&emsp;extend_string|拓展字符串||false|string||
|&emsp;&emsp;features_requested|融合特征 1、开启 0、关闭||false|integer(int32)||
|&emsp;&emsp;safety_scanner_region|雷达避障区域 0、默认区域  1、避障区域1   2、避障区域2  .....  15、避障区域15||false|integer(int32)||
|id|AGV路径导航参数ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AGVPathParam|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|safety|避障 1、打开避障  2、关闭避障|integer(int32)|integer(int32)|
|max_translation_speed|最大平移速度 >0 m/s|number(double)|number(double)|
|max_rotate_speed|最大旋转速度 rad/s >0|number(double)|number(double)|
|P|平移加速比例控制系数 >0|number(double)|number(double)|
|D|平移加速微分控制系数 >0|number(double)|number(double)|
|translation_acc|平移加（减）速度 m/s2 >0|number(double)|number(double)|
|rotate_acc|旋转加（减）速度 rad/s2 >0|number(double)|number(double)|
|obstacle_avoidance|绕障 1、打开绕障  2、关闭绕障|integer(int32)|integer(int32)|
|obstacle_avoidance_timeout|避障超时时间（超时后AGV会自动绕障） 单位：秒|integer(int32)|integer(int32)|
|obstacle_avoidance_count|绕障总次数（超过总次数后路径导航报错）|integer(int32)|integer(int32)|
|accurate_stop|是否启用末端精定位: 0不启用 1启用，默认是不启用|integer(int32)|integer(int32)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|修改时间|string(date-time)|string(date-time)|
|extend_bit|拓展布尔|string||
|extend_string|拓展字符串|string||
|features_requested|融合特征 1、开启 0、关闭|integer(int32)|integer(int32)|
|safety_scanner_region|雷达避障区域 0、默认区域  1、避障区域1   2、避障区域2  .....  15、避障区域15|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"id": "",
	"safety": 0,
	"max_translation_speed": 0,
	"max_rotate_speed": 0,
	"P": 0,
	"D": 0,
	"translation_acc": 0,
	"rotate_acc": 0,
	"obstacle_avoidance": 0,
	"obstacle_avoidance_timeout": 0,
	"obstacle_avoidance_count": 0,
	"accurate_stop": 0,
	"createTime": "",
	"updateTime": "",
	"extend_bit": "",
	"extend_string": "",
	"features_requested": 0,
	"safety_scanner_region": 0
}
```


# DataMatrix二维码


## 列表


**接口地址**:`/api/v3/dataCodeMatrix`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|agvMapName|地图名称||true|String|String|
|isDraft|是否查询草稿数据|query|true|boolean||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|DataCodeMatrix|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|Id|string||
|reference_id|查询Id Compass创建二维码地图默认给origin|string||
|x|x坐标|number(double)|number(double)|
|y|y坐标|number(double)|number(double)|
|theta|角度|number(double)|number(double)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"reference_id": "",
		"x": 0,
		"y": 0,
		"theta": 0
	}
]
```


## 创建


**接口地址**:`/api/v3/dataCodeMatrix`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"reference_id": "",
	"x": 0,
	"y": 0,
	"theta": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|dataCodeMatrix|DataMatrix二维码|body|true|DataCodeMatrix|DataCodeMatrix|
|&emsp;&emsp;id|Id||false|string||
|&emsp;&emsp;reference_id|查询Id Compass创建二维码地图默认给origin||false|string||
|&emsp;&emsp;x|x坐标||false|number(double)||
|&emsp;&emsp;y|y坐标||false|number(double)||
|&emsp;&emsp;theta|角度||false|number(double)||
|mapName|mapName|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|DataCodeMatrix|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|Id|string||
|reference_id|查询Id Compass创建二维码地图默认给origin|string||
|x|x坐标|number(double)|number(double)|
|y|y坐标|number(double)|number(double)|
|theta|角度|number(double)|number(double)|


**响应示例**:
```javascript
{
	"id": "",
	"reference_id": "",
	"x": 0,
	"y": 0,
	"theta": 0
}
```


## 分页查询


**接口地址**:`/api/v3/dataCodeMatrix/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||
|isDraft|isDraft|query|false|boolean||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«DataCodeMatrix»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|list||array|DataCodeMatrix|
|&emsp;&emsp;id|Id|string||
|&emsp;&emsp;reference_id|查询Id Compass创建二维码地图默认给origin|string||
|&emsp;&emsp;x|x坐标|number(double)||
|&emsp;&emsp;y|y坐标|number(double)||
|&emsp;&emsp;theta|角度|number(double)||
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pagerCount||integer(int32)|integer(int32)|
|total||integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"list": [
		{
			"id": "",
			"reference_id": "",
			"x": 0,
			"y": 0,
			"theta": 0
		}
	],
	"pageNum": 0,
	"pageSize": 0,
	"pagerCount": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/dataCodeMatrix/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:根据ID获取DataMatrix二维码详情


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|DataMatrix二维码ID|path|true|string||
|isDraft|是否查询草稿数据|query|true|boolean||
|mapName|地图名称|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|DataCodeMatrix|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|Id|string||
|reference_id|查询Id Compass创建二维码地图默认给origin|string||
|x|x坐标|number(double)|number(double)|
|y|y坐标|number(double)|number(double)|
|theta|角度|number(double)|number(double)|


**响应示例**:
```javascript
{
	"id": "",
	"reference_id": "",
	"x": 0,
	"y": 0,
	"theta": 0
}
```


## 更新


**接口地址**:`/api/v3/dataCodeMatrix/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:根据ID更新DataMatrix二维码信息


**请求示例**:


```javascript
{
	"id": "",
	"reference_id": "",
	"x": 0,
	"y": 0,
	"theta": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|dataCodeMatrix|DataMatrix二维码|body|true|DataCodeMatrix|DataCodeMatrix|
|&emsp;&emsp;id|Id||false|string||
|&emsp;&emsp;reference_id|查询Id Compass创建二维码地图默认给origin||false|string||
|&emsp;&emsp;x|x坐标||false|number(double)||
|&emsp;&emsp;y|y坐标||false|number(double)||
|&emsp;&emsp;theta|角度||false|number(double)||
|id|DataMatrix二维码ID|path|true|string||
|mapName|mapName|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|DataCodeMatrix|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|Id|string||
|reference_id|查询Id Compass创建二维码地图默认给origin|string||
|x|x坐标|number(double)|number(double)|
|y|y坐标|number(double)|number(double)|
|theta|角度|number(double)|number(double)|


**响应示例**:
```javascript
{
	"id": "",
	"reference_id": "",
	"x": 0,
	"y": 0,
	"theta": 0
}
```


## 删除


**接口地址**:`/api/v3/dataCodeMatrix/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:根据ID删除DataMatrix二维码信息


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|DataMatrix二维码ID|path|true|string||
|mapName|地图名称|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# logo处理


## 查询Logo信息


**接口地址**:`/api/v3/logo`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|LogoInfo|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|companyName|公司名称|string||
|enterpriseUrl|公司网址|string||
|loginTitle|网页标题|string||
|loginTitleFontSize|登录页标题字体大小|string||
|version|系统版本|string||
|agvVersion|机器人版本|string||
|versionOwner|版权所有|string||
|logoImage|logo图片|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"companyName": "",
	"enterpriseUrl": "",
	"loginTitle": "",
	"loginTitleFontSize": "",
	"version": "",
	"agvVersion": "",
	"versionOwner": "",
	"logoImage": "",
	"createTime": "",
	"updateTime": ""
}
```


## 创建Logo


**接口地址**:`/api/v3/logo`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"companyName": "",
	"enterpriseUrl": "",
	"loginTitle": "",
	"loginTitleFontSize": "",
	"version": "",
	"agvVersion": "",
	"versionOwner": "",
	"logoImage": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|logoInfo|logo信息|body|true|LogoInfo|LogoInfo|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;companyName|公司名称||false|string||
|&emsp;&emsp;enterpriseUrl|公司网址||false|string||
|&emsp;&emsp;loginTitle|网页标题||false|string||
|&emsp;&emsp;loginTitleFontSize|登录页标题字体大小||false|string||
|&emsp;&emsp;version|系统版本||false|string||
|&emsp;&emsp;agvVersion|机器人版本||false|string||
|&emsp;&emsp;versionOwner|版权所有||false|string||
|&emsp;&emsp;logoImage|logo图片||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 修改Logo


**接口地址**:`/api/v3/logo`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"companyName": "",
	"enterpriseUrl": "",
	"loginTitle": "",
	"loginTitleFontSize": "",
	"version": "",
	"agvVersion": "",
	"versionOwner": "",
	"logoImage": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|logoInfo|logo信息|body|true|LogoInfo|LogoInfo|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;companyName|公司名称||false|string||
|&emsp;&emsp;enterpriseUrl|公司网址||false|string||
|&emsp;&emsp;loginTitle|网页标题||false|string||
|&emsp;&emsp;loginTitleFontSize|登录页标题字体大小||false|string||
|&emsp;&emsp;version|系统版本||false|string||
|&emsp;&emsp;agvVersion|机器人版本||false|string||
|&emsp;&emsp;versionOwner|版权所有||false|string||
|&emsp;&emsp;logoImage|logo图片||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# sensor-controller


## 查询所有


**接口地址**:`/api/v3/sensors`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|searchMap|searchMap|query|true||object|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|传感器|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|编号|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|functionCode|功能码|string||
|id||string||
|ip|IP地址|string||
|isDisabled|是否被禁用,0:未禁用,1:已禁用|integer(int32)|integer(int32)|
|name|名称|string||
|port|端口号|integer(int32)|integer(int32)|
|slaveId|从站ID|string||
|startAddress|起始地址|string||
|status|状态,0未触发、1已触发|integer(int32)|integer(int32)|
|triggerSelectors|关联触发器|array|TriggerSelector|
|&emsp;&emsp;buttonAddress|按钮地址|integer(int32)||
|&emsp;&emsp;code|编码|string||
|&emsp;&emsp;completedTimes|已经完成次数|integer(int32)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;deviceAddress|设备地址|integer(int32)||
|&emsp;&emsp;executeTimes|执行次数|integer(int32)||
|&emsp;&emsp;id|主键ID|string||
|&emsp;&emsp;isDisabled|是否禁用,0:启用、1:禁用|integer(int32)||
|&emsp;&emsp;missionCode|触发器关联的任务编码|string||
|&emsp;&emsp;missionId|任务ID|string||
|&emsp;&emsp;missionName|触发器关联的任务名称|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;pagerId|呼叫器ID|string||
|&emsp;&emsp;period|触发间隔|integer(int64)||
|&emsp;&emsp;sensorJson|传感器JSON [{"sensorId":"xxxx","value":1}]|string||
|&emsp;&emsp;startTime|开始时间|string(date-time)||
|&emsp;&emsp;startType|开始类型;1:即时、2:定时|integer(int32)||
|&emsp;&emsp;type|触发类型;1:定时触发、2呼叫器触发、3传感器触发|integer(int32)||
|&emsp;&emsp;unit|触发间隔的时间单位;SECOND、DAY、WEEK、MONTH|string||
|&emsp;&emsp;updateTime|修改时间|string(date-time)||
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"code": "",
		"createTime": "",
		"functionCode": "",
		"id": "",
		"ip": "",
		"isDisabled": 0,
		"name": "",
		"port": 0,
		"slaveId": "",
		"startAddress": "",
		"status": 0,
		"triggerSelectors": [
			{
				"buttonAddress": 0,
				"code": "",
				"completedTimes": 0,
				"createTime": "",
				"deviceAddress": 0,
				"executeTimes": 0,
				"id": "",
				"isDisabled": 0,
				"missionCode": "",
				"missionId": "",
				"missionName": "",
				"name": "",
				"pagerId": "",
				"period": 0,
				"sensorJson": "",
				"startTime": "",
				"startType": 0,
				"type": 0,
				"unit": "",
				"updateTime": ""
			}
		],
		"updateTime": ""
	}
]
```


## 创建


**接口地址**:`/api/v3/sensors`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sensor|传感器|body|true|Sensor|Sensor|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 分页查询


**接口地址**:`/api/v3/sensors/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||
|searchMap|searchMap|query|false||object|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«传感器»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|传感器|
|&emsp;&emsp;code|编号|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;functionCode|功能码|string||
|&emsp;&emsp;id||string||
|&emsp;&emsp;ip|IP地址|string||
|&emsp;&emsp;isDisabled|是否被禁用,0:未禁用,1:已禁用|integer(int32)||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;port|端口号|integer(int32)||
|&emsp;&emsp;slaveId|从站ID|string||
|&emsp;&emsp;startAddress|起始地址|string||
|&emsp;&emsp;status|状态,0未触发、1已触发|integer(int32)||
|&emsp;&emsp;triggerSelectors|关联触发器|array|TriggerSelector|
|&emsp;&emsp;&emsp;&emsp;buttonAddress|按钮地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;code|编码||false|string||
|&emsp;&emsp;&emsp;&emsp;completedTimes|已经完成次数||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;deviceAddress|设备地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;executeTimes|执行次数||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;id|主键ID||false|string||
|&emsp;&emsp;&emsp;&emsp;isDisabled|是否禁用,0:启用、1:禁用||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;missionCode|触发器关联的任务编码||false|string||
|&emsp;&emsp;&emsp;&emsp;missionId|任务ID||false|string||
|&emsp;&emsp;&emsp;&emsp;missionName|触发器关联的任务名称||false|string||
|&emsp;&emsp;&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;&emsp;&emsp;pagerId|呼叫器ID||false|string||
|&emsp;&emsp;&emsp;&emsp;period|触发间隔||false|integer(int64)||
|&emsp;&emsp;&emsp;&emsp;sensorJson|传感器JSON [{"sensorId":"xxxx","value":1}]||false|string||
|&emsp;&emsp;&emsp;&emsp;startTime|开始时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;startType|开始类型;1:即时、2:定时||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;type|触发类型;1:定时触发、2呼叫器触发、3传感器触发||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;unit|触发间隔的时间单位;SECOND、DAY、WEEK、MONTH||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|修改时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"code": "",
			"createTime": "",
			"functionCode": "",
			"id": "",
			"ip": "",
			"isDisabled": 0,
			"name": "",
			"port": 0,
			"slaveId": "",
			"startAddress": "",
			"status": 0,
			"triggerSelectors": [
				{
					"buttonAddress": 0,
					"code": "",
					"completedTimes": 0,
					"createTime": "",
					"deviceAddress": 0,
					"executeTimes": 0,
					"id": "",
					"isDisabled": 0,
					"missionCode": "",
					"missionId": "",
					"missionName": "",
					"name": "",
					"pagerId": "",
					"period": 0,
					"sensorJson": "",
					"startTime": "",
					"startType": 0,
					"type": 0,
					"unit": "",
					"updateTime": ""
				}
			],
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/sensors/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|传感器ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|传感器|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|编号|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|functionCode|功能码|string||
|id||string||
|ip|IP地址|string||
|isDisabled|是否被禁用,0:未禁用,1:已禁用|integer(int32)|integer(int32)|
|name|名称|string||
|port|端口号|integer(int32)|integer(int32)|
|slaveId|从站ID|string||
|startAddress|起始地址|string||
|status|状态,0未触发、1已触发|integer(int32)|integer(int32)|
|triggerSelectors|关联触发器|array|TriggerSelector|
|&emsp;&emsp;buttonAddress|按钮地址|integer(int32)||
|&emsp;&emsp;code|编码|string||
|&emsp;&emsp;completedTimes|已经完成次数|integer(int32)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;deviceAddress|设备地址|integer(int32)||
|&emsp;&emsp;executeTimes|执行次数|integer(int32)||
|&emsp;&emsp;id|主键ID|string||
|&emsp;&emsp;isDisabled|是否禁用,0:启用、1:禁用|integer(int32)||
|&emsp;&emsp;missionCode|触发器关联的任务编码|string||
|&emsp;&emsp;missionId|任务ID|string||
|&emsp;&emsp;missionName|触发器关联的任务名称|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;pagerId|呼叫器ID|string||
|&emsp;&emsp;period|触发间隔|integer(int64)||
|&emsp;&emsp;sensorJson|传感器JSON [{"sensorId":"xxxx","value":1}]|string||
|&emsp;&emsp;startTime|开始时间|string(date-time)||
|&emsp;&emsp;startType|开始类型;1:即时、2:定时|integer(int32)||
|&emsp;&emsp;type|触发类型;1:定时触发、2呼叫器触发、3传感器触发|integer(int32)||
|&emsp;&emsp;unit|触发间隔的时间单位;SECOND、DAY、WEEK、MONTH|string||
|&emsp;&emsp;updateTime|修改时间|string(date-time)||
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"code": "",
	"createTime": "",
	"functionCode": "",
	"id": "",
	"ip": "",
	"isDisabled": 0,
	"name": "",
	"port": 0,
	"slaveId": "",
	"startAddress": "",
	"status": 0,
	"triggerSelectors": [
		{
			"buttonAddress": 0,
			"code": "",
			"completedTimes": 0,
			"createTime": "",
			"deviceAddress": 0,
			"executeTimes": 0,
			"id": "",
			"isDisabled": 0,
			"missionCode": "",
			"missionId": "",
			"missionName": "",
			"name": "",
			"pagerId": "",
			"period": 0,
			"sensorJson": "",
			"startTime": "",
			"startType": 0,
			"type": 0,
			"unit": "",
			"updateTime": ""
		}
	],
	"updateTime": ""
}
```


## 修改


**接口地址**:`/api/v3/sensors/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|传感器ID|path|true|string||
|sensor|Sensor|body|true|Sensor|Sensor|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 删除


**接口地址**:`/api/v3/sensors/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 任务


## 列表


**接口地址**:`/api/v3/missionWorks`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWork|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|currentActionName|指令名称|string||
|currentActionSequence|指令序号|integer(int32)|integer(int32)|
|id|ID|string||
|releaseButtonAddress||integer(int32)|integer(int32)|
|releaseDeviceAddress||integer(int32)|integer(int32)|
|releaseSuccess||boolean||
|code|任务编码|string||
|missionCallId|预设任务ID|string||
|missionId|预设任务ID|string||
|name|名称|string||
|schedulePlanId|调度计划的ID|string||
|callbackUrl|回调接口|string||
|sequence|优先级: 1、低  2、普通  3、高  4、最高  默认是2|integer(int32)|integer(int32)|
|description|描述|string||
|status|状态 CREATE:创建(未执行) START:开始执行 WAIT:等待(继续)执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 PAUSE:暂停 BEING_PAUSE:暂停中 BEING_RESUME:恢复中 SHUTDOWN:已停止 BEING_SHUTDOWN:停止中 WAITINPUT:等待输入|string||
|message|异常信息|string||
|interrupt|是否可中断|boolean||
|runtimeParam|运行时参数(json格式) 如：{"marker1":"1001"}|string||
|missionWorkChainId|任务链ID|string||
|allocationStatus|分配状态 已分配：ASSIGNED  未分配：UNASSIGNED|string||
|totalMileage|任务总里程 单位 米|number(double)|number(double)|
|errorCode|异常错误代码|integer(int32)|integer(int32)|
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|agvCode|机器人编码|string||
|triggerSelectorId|触发器ID|string||
|updateTime|更新时间|string(date-time)|string(date-time)|
|createdBy|创建者 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||


**响应示例**:
```javascript
[
	{
		"currentActionName": "",
		"currentActionSequence": 0,
		"id": "",
		"releaseButtonAddress": 0,
		"releaseDeviceAddress": 0,
		"releaseSuccess": true,
		"code": "",
		"missionCallId": "",
		"missionId": "",
		"name": "",
		"schedulePlanId": "",
		"callbackUrl": "",
		"sequence": 0,
		"description": "",
		"status": "",
		"message": "",
		"interrupt": true,
		"runtimeParam": "",
		"missionWorkChainId": "",
		"allocationStatus": "",
		"totalMileage": 0,
		"errorCode": 0,
		"startTime": "",
		"endTime": "",
		"createTime": "",
		"agvCode": "",
		"triggerSelectorId": "",
		"updateTime": "",
		"createdBy": ""
	}
]
```


## 根据预设任务创建任务


**接口地址**:`/api/v3/missionWorks`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"missionId": "",
	"missionCode": "",
	"callbackUrl": "",
	"runtimeParam": {
		"marker1": "1001"
	}
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|missionWorkParam|任务创建参数|body|true|MissionWorkParam|MissionWorkParam|
|&emsp;&emsp;missionId|任务的ID||false|string||
|&emsp;&emsp;missionCode|任务编号||false|string||
|&emsp;&emsp;callbackUrl|回调接口||false|string||
|&emsp;&emsp;runtimeParam|运行时参数(json格式) 如：{"marker1":"1001"}||false|object||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|MissionWork|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|currentActionName|指令名称|string||
|currentActionSequence|指令序号|integer(int32)|integer(int32)|
|id|ID|string||
|releaseButtonAddress||integer(int32)|integer(int32)|
|releaseDeviceAddress||integer(int32)|integer(int32)|
|releaseSuccess||boolean||
|code|任务编码|string||
|missionCallId|预设任务ID|string||
|missionId|预设任务ID|string||
|name|名称|string||
|schedulePlanId|调度计划的ID|string||
|callbackUrl|回调接口|string||
|sequence|优先级: 1、低  2、普通  3、高  4、最高  默认是2|integer(int32)|integer(int32)|
|description|描述|string||
|status|状态 CREATE:创建(未执行) START:开始执行 WAIT:等待(继续)执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 PAUSE:暂停 BEING_PAUSE:暂停中 BEING_RESUME:恢复中 SHUTDOWN:已停止 BEING_SHUTDOWN:停止中 WAITINPUT:等待输入|string||
|message|异常信息|string||
|interrupt|是否可中断|boolean||
|runtimeParam|运行时参数(json格式) 如：{"marker1":"1001"}|string||
|missionWorkChainId|任务链ID|string||
|allocationStatus|分配状态 已分配：ASSIGNED  未分配：UNASSIGNED|string||
|totalMileage|任务总里程 单位 米|number(double)|number(double)|
|errorCode|异常错误代码|integer(int32)|integer(int32)|
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|agvCode|机器人编码|string||
|triggerSelectorId|触发器ID|string||
|updateTime|更新时间|string(date-time)|string(date-time)|
|createdBy|创建者 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||


**响应示例**:
```javascript
{
	"currentActionName": "",
	"currentActionSequence": 0,
	"id": "",
	"releaseButtonAddress": 0,
	"releaseDeviceAddress": 0,
	"releaseSuccess": true,
	"code": "",
	"missionCallId": "",
	"missionId": "",
	"name": "",
	"schedulePlanId": "",
	"callbackUrl": "",
	"sequence": 0,
	"description": "",
	"status": "",
	"message": "",
	"interrupt": true,
	"runtimeParam": "",
	"missionWorkChainId": "",
	"allocationStatus": "",
	"totalMileage": 0,
	"errorCode": 0,
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"agvCode": "",
	"triggerSelectorId": "",
	"updateTime": "",
	"createdBy": ""
}
```


## 停止所有任务


**接口地址**:`/api/v3/missionWorks/all/controls/stop`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 导出任务记录


**接口地址**:`/api/v3/missionWorks/exportRecord`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 任务名称列表


**接口地址**:`/api/v3/missionWorks/getNames`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 根据状态列表查询任务列表


**接口地址**:`/api/v3/missionWorks/listByStatus`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|statusList|状态列表|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 根据预设任务编号创建任务


**接口地址**:`/api/v3/missionWorks/missionCode`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"missionId": "",
	"missionCode": "",
	"callbackUrl": "",
	"runtimeParam": {
		"marker1": "1001"
	}
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|missionWorkParam|任务创建参数|body|true|MissionWorkParam|MissionWorkParam|
|&emsp;&emsp;missionId|任务的ID||false|string||
|&emsp;&emsp;missionCode|任务编号||false|string||
|&emsp;&emsp;callbackUrl|回调接口||false|string||
|&emsp;&emsp;runtimeParam|运行时参数(json格式) 如：{"marker1":"1001"}||false|object||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|MissionWork|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|currentActionName|指令名称|string||
|currentActionSequence|指令序号|integer(int32)|integer(int32)|
|id|ID|string||
|releaseButtonAddress||integer(int32)|integer(int32)|
|releaseDeviceAddress||integer(int32)|integer(int32)|
|releaseSuccess||boolean||
|code|任务编码|string||
|missionCallId|预设任务ID|string||
|missionId|预设任务ID|string||
|name|名称|string||
|schedulePlanId|调度计划的ID|string||
|callbackUrl|回调接口|string||
|sequence|优先级: 1、低  2、普通  3、高  4、最高  默认是2|integer(int32)|integer(int32)|
|description|描述|string||
|status|状态 CREATE:创建(未执行) START:开始执行 WAIT:等待(继续)执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 PAUSE:暂停 BEING_PAUSE:暂停中 BEING_RESUME:恢复中 SHUTDOWN:已停止 BEING_SHUTDOWN:停止中 WAITINPUT:等待输入|string||
|message|异常信息|string||
|interrupt|是否可中断|boolean||
|runtimeParam|运行时参数(json格式) 如：{"marker1":"1001"}|string||
|missionWorkChainId|任务链ID|string||
|allocationStatus|分配状态 已分配：ASSIGNED  未分配：UNASSIGNED|string||
|totalMileage|任务总里程 单位 米|number(double)|number(double)|
|errorCode|异常错误代码|integer(int32)|integer(int32)|
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|agvCode|机器人编码|string||
|triggerSelectorId|触发器ID|string||
|updateTime|更新时间|string(date-time)|string(date-time)|
|createdBy|创建者 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||


**响应示例**:
```javascript
{
	"currentActionName": "",
	"currentActionSequence": 0,
	"id": "",
	"releaseButtonAddress": 0,
	"releaseDeviceAddress": 0,
	"releaseSuccess": true,
	"code": "",
	"missionCallId": "",
	"missionId": "",
	"name": "",
	"schedulePlanId": "",
	"callbackUrl": "",
	"sequence": 0,
	"description": "",
	"status": "",
	"message": "",
	"interrupt": true,
	"runtimeParam": "",
	"missionWorkChainId": "",
	"allocationStatus": "",
	"totalMileage": 0,
	"errorCode": 0,
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"agvCode": "",
	"triggerSelectorId": "",
	"updateTime": "",
	"createdBy": ""
}
```


## 分页查询


**接口地址**:`/api/v3/missionWorks/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«MissionWork»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|MissionWork|
|&emsp;&emsp;currentActionName|指令名称|string||
|&emsp;&emsp;currentActionSequence|指令序号|integer(int32)||
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;releaseButtonAddress||integer(int32)||
|&emsp;&emsp;releaseDeviceAddress||integer(int32)||
|&emsp;&emsp;releaseSuccess||boolean||
|&emsp;&emsp;code|任务编码|string||
|&emsp;&emsp;missionCallId|预设任务ID|string||
|&emsp;&emsp;missionId|预设任务ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;schedulePlanId|调度计划的ID|string||
|&emsp;&emsp;callbackUrl|回调接口|string||
|&emsp;&emsp;sequence|优先级: 1、低  2、普通  3、高  4、最高  默认是2|integer(int32)||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;status|状态 CREATE:创建(未执行) START:开始执行 WAIT:等待(继续)执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 PAUSE:暂停 BEING_PAUSE:暂停中 BEING_RESUME:恢复中 SHUTDOWN:已停止 BEING_SHUTDOWN:停止中 WAITINPUT:等待输入|string||
|&emsp;&emsp;message|异常信息|string||
|&emsp;&emsp;interrupt|是否可中断|boolean||
|&emsp;&emsp;runtimeParam|运行时参数(json格式) 如：{"marker1":"1001"}|string||
|&emsp;&emsp;missionWorkChainId|任务链ID|string||
|&emsp;&emsp;allocationStatus|分配状态 已分配：ASSIGNED  未分配：UNASSIGNED|string||
|&emsp;&emsp;totalMileage|任务总里程 单位 米|number(double)||
|&emsp;&emsp;errorCode|异常错误代码|integer(int32)||
|&emsp;&emsp;startTime|开始时间|string(date-time)||
|&emsp;&emsp;endTime|结束时间|string(date-time)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;agvCode|机器人编码|string||
|&emsp;&emsp;triggerSelectorId|触发器ID|string||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|&emsp;&emsp;createdBy|创建者 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"currentActionName": "",
			"currentActionSequence": 0,
			"id": "",
			"releaseButtonAddress": 0,
			"releaseDeviceAddress": 0,
			"releaseSuccess": true,
			"code": "",
			"missionCallId": "",
			"missionId": "",
			"name": "",
			"schedulePlanId": "",
			"callbackUrl": "",
			"sequence": 0,
			"description": "",
			"status": "",
			"message": "",
			"interrupt": true,
			"runtimeParam": "",
			"missionWorkChainId": "",
			"allocationStatus": "",
			"totalMileage": 0,
			"errorCode": 0,
			"startTime": "",
			"endTime": "",
			"createTime": "",
			"agvCode": "",
			"triggerSelectorId": "",
			"updateTime": "",
			"createdBy": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/missionWorks/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|任务ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWork|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|currentActionName|指令名称|string||
|currentActionSequence|指令序号|integer(int32)|integer(int32)|
|id|ID|string||
|releaseButtonAddress||integer(int32)|integer(int32)|
|releaseDeviceAddress||integer(int32)|integer(int32)|
|releaseSuccess||boolean||
|code|任务编码|string||
|missionCallId|预设任务ID|string||
|missionId|预设任务ID|string||
|name|名称|string||
|schedulePlanId|调度计划的ID|string||
|callbackUrl|回调接口|string||
|sequence|优先级: 1、低  2、普通  3、高  4、最高  默认是2|integer(int32)|integer(int32)|
|description|描述|string||
|status|状态 CREATE:创建(未执行) START:开始执行 WAIT:等待(继续)执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 PAUSE:暂停 BEING_PAUSE:暂停中 BEING_RESUME:恢复中 SHUTDOWN:已停止 BEING_SHUTDOWN:停止中 WAITINPUT:等待输入|string||
|message|异常信息|string||
|interrupt|是否可中断|boolean||
|runtimeParam|运行时参数(json格式) 如：{"marker1":"1001"}|string||
|missionWorkChainId|任务链ID|string||
|allocationStatus|分配状态 已分配：ASSIGNED  未分配：UNASSIGNED|string||
|totalMileage|任务总里程 单位 米|number(double)|number(double)|
|errorCode|异常错误代码|integer(int32)|integer(int32)|
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|agvCode|机器人编码|string||
|triggerSelectorId|触发器ID|string||
|updateTime|更新时间|string(date-time)|string(date-time)|
|createdBy|创建者 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||


**响应示例**:
```javascript
{
	"currentActionName": "",
	"currentActionSequence": 0,
	"id": "",
	"releaseButtonAddress": 0,
	"releaseDeviceAddress": 0,
	"releaseSuccess": true,
	"code": "",
	"missionCallId": "",
	"missionId": "",
	"name": "",
	"schedulePlanId": "",
	"callbackUrl": "",
	"sequence": 0,
	"description": "",
	"status": "",
	"message": "",
	"interrupt": true,
	"runtimeParam": "",
	"missionWorkChainId": "",
	"allocationStatus": "",
	"totalMileage": 0,
	"errorCode": 0,
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"agvCode": "",
	"triggerSelectorId": "",
	"updateTime": "",
	"createdBy": ""
}
```


## 更新


**接口地址**:`/api/v3/missionWorks/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"currentActionName": "",
	"currentActionSequence": 0,
	"id": "",
	"releaseButtonAddress": 0,
	"releaseDeviceAddress": 0,
	"releaseSuccess": true,
	"code": "",
	"missionCallId": "",
	"missionId": "",
	"name": "",
	"schedulePlanId": "",
	"callbackUrl": "",
	"sequence": 0,
	"description": "",
	"status": "",
	"message": "",
	"interrupt": true,
	"runtimeParam": "",
	"missionWorkChainId": "",
	"allocationStatus": "",
	"totalMileage": 0,
	"errorCode": 0,
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"agvCode": "",
	"triggerSelectorId": "",
	"updateTime": "",
	"createdBy": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|任务ID|path|true|string||
|missionWork|任务|body|true|MissionWork|MissionWork|
|&emsp;&emsp;currentActionName|指令名称||false|string||
|&emsp;&emsp;currentActionSequence|指令序号||false|integer(int32)||
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;releaseButtonAddress|||false|integer(int32)||
|&emsp;&emsp;releaseDeviceAddress|||false|integer(int32)||
|&emsp;&emsp;releaseSuccess|||false|boolean||
|&emsp;&emsp;code|任务编码||false|string||
|&emsp;&emsp;missionCallId|预设任务ID||false|string||
|&emsp;&emsp;missionId|预设任务ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;schedulePlanId|调度计划的ID||false|string||
|&emsp;&emsp;callbackUrl|回调接口||false|string||
|&emsp;&emsp;sequence|优先级: 1、低  2、普通  3、高  4、最高  默认是2||false|integer(int32)||
|&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;status|状态 CREATE:创建(未执行) START:开始执行 WAIT:等待(继续)执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 PAUSE:暂停 BEING_PAUSE:暂停中 BEING_RESUME:恢复中 SHUTDOWN:已停止 BEING_SHUTDOWN:停止中 WAITINPUT:等待输入||false|string||
|&emsp;&emsp;message|异常信息||false|string||
|&emsp;&emsp;interrupt|是否可中断||false|boolean||
|&emsp;&emsp;runtimeParam|运行时参数(json格式) 如：{"marker1":"1001"}||false|string||
|&emsp;&emsp;missionWorkChainId|任务链ID||false|string||
|&emsp;&emsp;allocationStatus|分配状态 已分配：ASSIGNED  未分配：UNASSIGNED||false|string||
|&emsp;&emsp;totalMileage|任务总里程 单位 米||false|number(double)||
|&emsp;&emsp;errorCode|异常错误代码||false|integer(int32)||
|&emsp;&emsp;startTime|开始时间||false|string(date-time)||
|&emsp;&emsp;endTime|结束时间||false|string(date-time)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;agvCode|机器人编码||false|string||
|&emsp;&emsp;triggerSelectorId|触发器ID||false|string||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|&emsp;&emsp;createdBy|创建者 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWork|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|currentActionName|指令名称|string||
|currentActionSequence|指令序号|integer(int32)|integer(int32)|
|id|ID|string||
|releaseButtonAddress||integer(int32)|integer(int32)|
|releaseDeviceAddress||integer(int32)|integer(int32)|
|releaseSuccess||boolean||
|code|任务编码|string||
|missionCallId|预设任务ID|string||
|missionId|预设任务ID|string||
|name|名称|string||
|schedulePlanId|调度计划的ID|string||
|callbackUrl|回调接口|string||
|sequence|优先级: 1、低  2、普通  3、高  4、最高  默认是2|integer(int32)|integer(int32)|
|description|描述|string||
|status|状态 CREATE:创建(未执行) START:开始执行 WAIT:等待(继续)执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 PAUSE:暂停 BEING_PAUSE:暂停中 BEING_RESUME:恢复中 SHUTDOWN:已停止 BEING_SHUTDOWN:停止中 WAITINPUT:等待输入|string||
|message|异常信息|string||
|interrupt|是否可中断|boolean||
|runtimeParam|运行时参数(json格式) 如：{"marker1":"1001"}|string||
|missionWorkChainId|任务链ID|string||
|allocationStatus|分配状态 已分配：ASSIGNED  未分配：UNASSIGNED|string||
|totalMileage|任务总里程 单位 米|number(double)|number(double)|
|errorCode|异常错误代码|integer(int32)|integer(int32)|
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|agvCode|机器人编码|string||
|triggerSelectorId|触发器ID|string||
|updateTime|更新时间|string(date-time)|string(date-time)|
|createdBy|创建者 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||


**响应示例**:
```javascript
{
	"currentActionName": "",
	"currentActionSequence": 0,
	"id": "",
	"releaseButtonAddress": 0,
	"releaseDeviceAddress": 0,
	"releaseSuccess": true,
	"code": "",
	"missionCallId": "",
	"missionId": "",
	"name": "",
	"schedulePlanId": "",
	"callbackUrl": "",
	"sequence": 0,
	"description": "",
	"status": "",
	"message": "",
	"interrupt": true,
	"runtimeParam": "",
	"missionWorkChainId": "",
	"allocationStatus": "",
	"totalMileage": 0,
	"errorCode": 0,
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"agvCode": "",
	"triggerSelectorId": "",
	"updateTime": "",
	"createdBy": ""
}
```


## 删除


**接口地址**:`/api/v3/missionWorks/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|任务ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 继续执行任务


**接口地址**:`/api/v3/missionWorks/{id}/controls/continue`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|任务ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 暂停任务


**接口地址**:`/api/v3/missionWorks/{id}/controls/pause`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|任务ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 恢复任务


**接口地址**:`/api/v3/missionWorks/{id}/controls/resume`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|任务ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 停止任务


**接口地址**:`/api/v3/missionWorks/{id}/controls/stop`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|任务ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 停止任务并将机器人切换到手动模式


**接口地址**:`/api/v3/missionWorks/{id}/controls/stopAndManualMode`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|任务ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 根据任务ID查询动作列表


**接口地址**:`/api/v3/missionWorks/{id}/missionWorkActions`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|任务ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWorkAction|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionActionId|预设动作ID|string||
|missionWorkId|任务ID|string||
|actionType|动作类型|string||
|name|名称|string||
|sequence|顺序编号|integer(int32)|integer(int32)|
|message|执行结果描述|string||
|parentActionId|父类动作Id|string||
|parameters|参数|string||
|status|状态 START:开始执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误|string||
|childType|子动作类型 1、IF 2、ELSE 3、WHILE|string||
|resultCode|返回编码 1001:正确编码 其他为错误编码|integer(int32)|integer(int32)|
|resultMessage|返回提示信息|string||
|resultType|返回数据区数据类型|string||
|resultData|返回数据区数据|string||
|errorCode|异常错误代码|integer(int32)|integer(int32)|
|thisLoopCompletes|当该action属于循环action的子action时，记录该action所在的本次循环执行是否完成|boolean||
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"missionActionId": "",
		"missionWorkId": "",
		"actionType": "",
		"name": "",
		"sequence": 0,
		"message": "",
		"parentActionId": "",
		"parameters": "",
		"status": "",
		"childType": "",
		"resultCode": 0,
		"resultMessage": "",
		"resultType": "",
		"resultData": "",
		"errorCode": 0,
		"thisLoopCompletes": true,
		"startTime": "",
		"endTime": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


## 根据任务ID查询任务全局变量


**接口地址**:`/api/v3/missionWorks/{id}/missionWorkGlobalVariables`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|任务ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWorkGlobalVariable|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|预设任务ID|string||
|missionWorkId|任务ID|string||
|variableKey|变量键|string||
|variableValue|变量值|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"missionId": "",
		"missionWorkId": "",
		"variableKey": "",
		"variableValue": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


## 获取等待输入的变量列表


**接口地址**:`/api/v3/missionWorks/{id}/waitInputVariables`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|任务ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWorkGlobalVariable|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|预设任务ID|string||
|missionWorkId|任务ID|string||
|variableKey|变量键|string||
|variableValue|变量值|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"missionId": "",
		"missionWorkId": "",
		"variableKey": "",
		"variableValue": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


# 任务全局变量


## 列表


**接口地址**:`/api/v3/missionWorkGlobalVariables`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWorkGlobalVariable|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|预设任务ID|string||
|missionWorkId|任务ID|string||
|variableKey|变量键|string||
|variableValue|变量值|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"missionId": "",
		"missionWorkId": "",
		"variableKey": "",
		"variableValue": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


## 批量更新


**接口地址**:`/api/v3/missionWorkGlobalVariables/batch`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
[
	{
		"id": "",
		"missionId": "",
		"missionWorkId": "",
		"variableKey": "",
		"variableValue": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|missionWorkGlobalVariables|任务全局变量|body|true|array|MissionWorkGlobalVariable|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;missionId|预设任务ID||false|string||
|&emsp;&emsp;missionWorkId|任务ID||false|string||
|&emsp;&emsp;variableKey|变量键||false|string||
|&emsp;&emsp;variableValue|变量值||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 分页查询


**接口地址**:`/api/v3/missionWorkGlobalVariables/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«MissionWorkGlobalVariable»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|MissionWorkGlobalVariable|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;missionId|预设任务ID|string||
|&emsp;&emsp;missionWorkId|任务ID|string||
|&emsp;&emsp;variableKey|变量键|string||
|&emsp;&emsp;variableValue|变量值|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"missionId": "",
			"missionWorkId": "",
			"variableKey": "",
			"variableValue": "",
			"createTime": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/missionWorkGlobalVariables/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|任务全局变量ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWorkGlobalVariable|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|预设任务ID|string||
|missionWorkId|任务ID|string||
|variableKey|变量键|string||
|variableValue|变量值|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"missionId": "",
	"missionWorkId": "",
	"variableKey": "",
	"variableValue": "",
	"createTime": "",
	"updateTime": ""
}
```


## 更新


**接口地址**:`/api/v3/missionWorkGlobalVariables/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"missionId": "",
	"missionWorkId": "",
	"variableKey": "",
	"variableValue": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|任务全局变量ID|path|true|string||
|missionWorkGlobalVariable|任务全局变量|body|true|MissionWorkGlobalVariable|MissionWorkGlobalVariable|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;missionId|预设任务ID||false|string||
|&emsp;&emsp;missionWorkId|任务ID||false|string||
|&emsp;&emsp;variableKey|变量键||false|string||
|&emsp;&emsp;variableValue|变量值||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWorkGlobalVariable|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|预设任务ID|string||
|missionWorkId|任务ID|string||
|variableKey|变量键|string||
|variableValue|变量值|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"missionId": "",
	"missionWorkId": "",
	"variableKey": "",
	"variableValue": "",
	"createTime": "",
	"updateTime": ""
}
```


# 任务数据导入导出


## 导出任务数据


**接口地址**:`/api/v3/export/exportMissionData`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:导出任务数据JSON文件


**请求示例**:


```javascript
{
	"missionIds": []
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|missionExportParam|missionExportParam|body|true|MissionExportParam|MissionExportParam|
|&emsp;&emsp;missionIds|||false|array|string|
|missionIds|任务id数组||false|String|String|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created||
|204|No Content||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 导入任务数据


**接口地址**:`/api/v3/export/importMission`


**请求方式**:`POST`


**请求数据类型**:`multipart/form-data`


**响应数据类型**:`*/*`


**接口描述**:导入任务数据JSON文件


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|mutiPartFile|文件|formData|true|ref||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 任务链


## 列表


**接口地址**:`/api/v3/missionWorkChains`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWorkChain|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|missionChainId|预设任务链ID|string||
|missionIds|预设任务ID列表, 多个ID以逗号隔开|string||
|unExecutedMissionIds|未执行的预设任务ID列表, 多个ID以逗号隔开|string||
|message|错误信息|string||
|status|状态  CREATE:创建  RUNNING:执行  FAULT:错误  SUCCESS:成功  SHUTDOWN:停止|string||
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|
|missions|预设任务列表|array|Mission|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;code|预设任务编码|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;sequence|优先级,1:低，2：普通，3：高，4：最高. 默认是2|integer(int32)||
|&emsp;&emsp;interrupt|是否可中断,True:任务可以被更高优级的新任务中断，False:必须执行完成后才能执行其他的任务。|boolean||
|&emsp;&emsp;version|预设任务版本|integer(int32)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|missionWorks|任务列表|array|MissionWork|
|&emsp;&emsp;currentActionName|指令名称|string||
|&emsp;&emsp;currentActionSequence|指令序号|integer(int32)||
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;releaseButtonAddress||integer(int32)||
|&emsp;&emsp;releaseDeviceAddress||integer(int32)||
|&emsp;&emsp;releaseSuccess||boolean||
|&emsp;&emsp;code|任务编码|string||
|&emsp;&emsp;missionCallId|预设任务ID|string||
|&emsp;&emsp;missionId|预设任务ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;schedulePlanId|调度计划的ID|string||
|&emsp;&emsp;callbackUrl|回调接口|string||
|&emsp;&emsp;sequence|优先级: 1、低  2、普通  3、高  4、最高  默认是2|integer(int32)||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;status|状态 CREATE:创建(未执行) START:开始执行 WAIT:等待(继续)执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 PAUSE:暂停 BEING_PAUSE:暂停中 BEING_RESUME:恢复中 SHUTDOWN:已停止 BEING_SHUTDOWN:停止中 WAITINPUT:等待输入|string||
|&emsp;&emsp;message|异常信息|string||
|&emsp;&emsp;interrupt|是否可中断|boolean||
|&emsp;&emsp;runtimeParam|运行时参数(json格式) 如：{"marker1":"1001"}|string||
|&emsp;&emsp;missionWorkChainId|任务链ID|string||
|&emsp;&emsp;allocationStatus|分配状态 已分配：ASSIGNED  未分配：UNASSIGNED|string||
|&emsp;&emsp;totalMileage|任务总里程 单位 米|number(double)||
|&emsp;&emsp;errorCode|异常错误代码|integer(int32)||
|&emsp;&emsp;startTime|开始时间|string(date-time)||
|&emsp;&emsp;endTime|结束时间|string(date-time)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;agvCode|机器人编码|string||
|&emsp;&emsp;triggerSelectorId|触发器ID|string||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|&emsp;&emsp;createdBy|创建者 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||
|unExecutedMissions|未执行的预设任务列表|array|Mission|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;code|预设任务编码|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;sequence|优先级,1:低，2：普通，3：高，4：最高. 默认是2|integer(int32)||
|&emsp;&emsp;interrupt|是否可中断,True:任务可以被更高优级的新任务中断，False:必须执行完成后才能执行其他的任务。|boolean||
|&emsp;&emsp;version|预设任务版本|integer(int32)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||


**响应示例**:
```javascript
[
	{
		"id": "",
		"name": "",
		"missionChainId": "",
		"missionIds": "",
		"unExecutedMissionIds": "",
		"message": "",
		"status": "",
		"startTime": "",
		"endTime": "",
		"createTime": "",
		"updateTime": "",
		"missions": [
			{
				"id": "",
				"code": "",
				"name": "自动运输任务",
				"description": "自动运输任务",
				"sequence": 2,
				"interrupt": false,
				"version": 0,
				"createTime": "",
				"updateTime": ""
			}
		],
		"missionWorks": [
			{
				"currentActionName": "",
				"currentActionSequence": 0,
				"id": "",
				"releaseButtonAddress": 0,
				"releaseDeviceAddress": 0,
				"releaseSuccess": true,
				"code": "",
				"missionCallId": "",
				"missionId": "",
				"name": "",
				"schedulePlanId": "",
				"callbackUrl": "",
				"sequence": 0,
				"description": "",
				"status": "",
				"message": "",
				"interrupt": true,
				"runtimeParam": "",
				"missionWorkChainId": "",
				"allocationStatus": "",
				"totalMileage": 0,
				"errorCode": 0,
				"startTime": "",
				"endTime": "",
				"createTime": "",
				"agvCode": "",
				"triggerSelectorId": "",
				"updateTime": "",
				"createdBy": ""
			}
		],
		"unExecutedMissions": [
			{
				"id": "",
				"code": "",
				"name": "自动运输任务",
				"description": "自动运输任务",
				"sequence": 2,
				"interrupt": false,
				"version": 0,
				"createTime": "",
				"updateTime": ""
			}
		]
	}
]
```


## 创建


**接口地址**:`/api/v3/missionWorkChains`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"missionChainId": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|missionWorkChainParam|任务链创建参数|body|true|MissionWorkChainParam|MissionWorkChainParam|
|&emsp;&emsp;missionChainId|预设任务链ID||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|MissionWorkChain|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|missionChainId|预设任务链ID|string||
|missionIds|预设任务ID列表, 多个ID以逗号隔开|string||
|unExecutedMissionIds|未执行的预设任务ID列表, 多个ID以逗号隔开|string||
|message|错误信息|string||
|status|状态  CREATE:创建  RUNNING:执行  FAULT:错误  SUCCESS:成功  SHUTDOWN:停止|string||
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|
|missions|预设任务列表|array|Mission|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;code|预设任务编码|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;sequence|优先级,1:低，2：普通，3：高，4：最高. 默认是2|integer(int32)||
|&emsp;&emsp;interrupt|是否可中断,True:任务可以被更高优级的新任务中断，False:必须执行完成后才能执行其他的任务。|boolean||
|&emsp;&emsp;version|预设任务版本|integer(int32)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|missionWorks|任务列表|array|MissionWork|
|&emsp;&emsp;currentActionName|指令名称|string||
|&emsp;&emsp;currentActionSequence|指令序号|integer(int32)||
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;releaseButtonAddress||integer(int32)||
|&emsp;&emsp;releaseDeviceAddress||integer(int32)||
|&emsp;&emsp;releaseSuccess||boolean||
|&emsp;&emsp;code|任务编码|string||
|&emsp;&emsp;missionCallId|预设任务ID|string||
|&emsp;&emsp;missionId|预设任务ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;schedulePlanId|调度计划的ID|string||
|&emsp;&emsp;callbackUrl|回调接口|string||
|&emsp;&emsp;sequence|优先级: 1、低  2、普通  3、高  4、最高  默认是2|integer(int32)||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;status|状态 CREATE:创建(未执行) START:开始执行 WAIT:等待(继续)执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 PAUSE:暂停 BEING_PAUSE:暂停中 BEING_RESUME:恢复中 SHUTDOWN:已停止 BEING_SHUTDOWN:停止中 WAITINPUT:等待输入|string||
|&emsp;&emsp;message|异常信息|string||
|&emsp;&emsp;interrupt|是否可中断|boolean||
|&emsp;&emsp;runtimeParam|运行时参数(json格式) 如：{"marker1":"1001"}|string||
|&emsp;&emsp;missionWorkChainId|任务链ID|string||
|&emsp;&emsp;allocationStatus|分配状态 已分配：ASSIGNED  未分配：UNASSIGNED|string||
|&emsp;&emsp;totalMileage|任务总里程 单位 米|number(double)||
|&emsp;&emsp;errorCode|异常错误代码|integer(int32)||
|&emsp;&emsp;startTime|开始时间|string(date-time)||
|&emsp;&emsp;endTime|结束时间|string(date-time)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;agvCode|机器人编码|string||
|&emsp;&emsp;triggerSelectorId|触发器ID|string||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|&emsp;&emsp;createdBy|创建者 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||
|unExecutedMissions|未执行的预设任务列表|array|Mission|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;code|预设任务编码|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;sequence|优先级,1:低，2：普通，3：高，4：最高. 默认是2|integer(int32)||
|&emsp;&emsp;interrupt|是否可中断,True:任务可以被更高优级的新任务中断，False:必须执行完成后才能执行其他的任务。|boolean||
|&emsp;&emsp;version|预设任务版本|integer(int32)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"missionChainId": "",
	"missionIds": "",
	"unExecutedMissionIds": "",
	"message": "",
	"status": "",
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"updateTime": "",
	"missions": [
		{
			"id": "",
			"code": "",
			"name": "自动运输任务",
			"description": "自动运输任务",
			"sequence": 2,
			"interrupt": false,
			"version": 0,
			"createTime": "",
			"updateTime": ""
		}
	],
	"missionWorks": [
		{
			"currentActionName": "",
			"currentActionSequence": 0,
			"id": "",
			"releaseButtonAddress": 0,
			"releaseDeviceAddress": 0,
			"releaseSuccess": true,
			"code": "",
			"missionCallId": "",
			"missionId": "",
			"name": "",
			"schedulePlanId": "",
			"callbackUrl": "",
			"sequence": 0,
			"description": "",
			"status": "",
			"message": "",
			"interrupt": true,
			"runtimeParam": "",
			"missionWorkChainId": "",
			"allocationStatus": "",
			"totalMileage": 0,
			"errorCode": 0,
			"startTime": "",
			"endTime": "",
			"createTime": "",
			"agvCode": "",
			"triggerSelectorId": "",
			"updateTime": "",
			"createdBy": ""
		}
	],
	"unExecutedMissions": [
		{
			"id": "",
			"code": "",
			"name": "自动运输任务",
			"description": "自动运输任务",
			"sequence": 2,
			"interrupt": false,
			"version": 0,
			"createTime": "",
			"updateTime": ""
		}
	]
}
```


## 根据状态列表查询任务链列表


**接口地址**:`/api/v3/missionWorkChains/listByStatus`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|statusList|状态列表|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 分页查询


**接口地址**:`/api/v3/missionWorkChains/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«MissionWorkChain»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|MissionWorkChain|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;missionChainId|预设任务链ID|string||
|&emsp;&emsp;missionIds|预设任务ID列表, 多个ID以逗号隔开|string||
|&emsp;&emsp;unExecutedMissionIds|未执行的预设任务ID列表, 多个ID以逗号隔开|string||
|&emsp;&emsp;message|错误信息|string||
|&emsp;&emsp;status|状态  CREATE:创建  RUNNING:执行  FAULT:错误  SUCCESS:成功  SHUTDOWN:停止|string||
|&emsp;&emsp;startTime|开始时间|string(date-time)||
|&emsp;&emsp;endTime|结束时间|string(date-time)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|&emsp;&emsp;missions|预设任务列表|array|Mission|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;code|预设任务编码||false|string||
|&emsp;&emsp;&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;&emsp;&emsp;sequence|优先级,1:低，2：普通，3：高，4：最高. 默认是2||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;interrupt|是否可中断,True:任务可以被更高优级的新任务中断，False:必须执行完成后才能执行其他的任务。||false|boolean||
|&emsp;&emsp;&emsp;&emsp;version|预设任务版本||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|&emsp;&emsp;missionWorks|任务列表|array|MissionWork|
|&emsp;&emsp;&emsp;&emsp;currentActionName|指令名称||false|string||
|&emsp;&emsp;&emsp;&emsp;currentActionSequence|指令序号||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;releaseButtonAddress|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;releaseDeviceAddress|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;releaseSuccess|||false|boolean||
|&emsp;&emsp;&emsp;&emsp;code|任务编码||false|string||
|&emsp;&emsp;&emsp;&emsp;missionCallId|预设任务ID||false|string||
|&emsp;&emsp;&emsp;&emsp;missionId|预设任务ID||false|string||
|&emsp;&emsp;&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;&emsp;&emsp;schedulePlanId|调度计划的ID||false|string||
|&emsp;&emsp;&emsp;&emsp;callbackUrl|回调接口||false|string||
|&emsp;&emsp;&emsp;&emsp;sequence|优先级: 1、低  2、普通  3、高  4、最高  默认是2||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;&emsp;&emsp;status|状态 CREATE:创建(未执行) START:开始执行 WAIT:等待(继续)执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 PAUSE:暂停 BEING_PAUSE:暂停中 BEING_RESUME:恢复中 SHUTDOWN:已停止 BEING_SHUTDOWN:停止中 WAITINPUT:等待输入||false|string||
|&emsp;&emsp;&emsp;&emsp;message|异常信息||false|string||
|&emsp;&emsp;&emsp;&emsp;interrupt|是否可中断||false|boolean||
|&emsp;&emsp;&emsp;&emsp;runtimeParam|运行时参数(json格式) 如：{"marker1":"1001"}||false|string||
|&emsp;&emsp;&emsp;&emsp;missionWorkChainId|任务链ID||false|string||
|&emsp;&emsp;&emsp;&emsp;allocationStatus|分配状态 已分配：ASSIGNED  未分配：UNASSIGNED||false|string||
|&emsp;&emsp;&emsp;&emsp;totalMileage|任务总里程 单位 米||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;errorCode|异常错误代码||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;startTime|开始时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;endTime|结束时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;agvCode|机器人编码||false|string||
|&emsp;&emsp;&emsp;&emsp;triggerSelectorId|触发器ID||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;createdBy|创建者 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass||false|string||
|&emsp;&emsp;unExecutedMissions|未执行的预设任务列表|array|Mission|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;code|预设任务编码||false|string||
|&emsp;&emsp;&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;&emsp;&emsp;sequence|优先级,1:低，2：普通，3：高，4：最高. 默认是2||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;interrupt|是否可中断,True:任务可以被更高优级的新任务中断，False:必须执行完成后才能执行其他的任务。||false|boolean||
|&emsp;&emsp;&emsp;&emsp;version|预设任务版本||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"name": "",
			"missionChainId": "",
			"missionIds": "",
			"unExecutedMissionIds": "",
			"message": "",
			"status": "",
			"startTime": "",
			"endTime": "",
			"createTime": "",
			"updateTime": "",
			"missions": [
				{
					"id": "",
					"code": "",
					"name": "自动运输任务",
					"description": "自动运输任务",
					"sequence": 2,
					"interrupt": false,
					"version": 0,
					"createTime": "",
					"updateTime": ""
				}
			],
			"missionWorks": [
				{
					"currentActionName": "",
					"currentActionSequence": 0,
					"id": "",
					"releaseButtonAddress": 0,
					"releaseDeviceAddress": 0,
					"releaseSuccess": true,
					"code": "",
					"missionCallId": "",
					"missionId": "",
					"name": "",
					"schedulePlanId": "",
					"callbackUrl": "",
					"sequence": 0,
					"description": "",
					"status": "",
					"message": "",
					"interrupt": true,
					"runtimeParam": "",
					"missionWorkChainId": "",
					"allocationStatus": "",
					"totalMileage": 0,
					"errorCode": 0,
					"startTime": "",
					"endTime": "",
					"createTime": "",
					"agvCode": "",
					"triggerSelectorId": "",
					"updateTime": "",
					"createdBy": ""
				}
			],
			"unExecutedMissions": [
				{
					"id": "",
					"code": "",
					"name": "自动运输任务",
					"description": "自动运输任务",
					"sequence": 2,
					"interrupt": false,
					"version": 0,
					"createTime": "",
					"updateTime": ""
				}
			]
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/missionWorkChains/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|任务链ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWorkChain|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|missionChainId|预设任务链ID|string||
|missionIds|预设任务ID列表, 多个ID以逗号隔开|string||
|unExecutedMissionIds|未执行的预设任务ID列表, 多个ID以逗号隔开|string||
|message|错误信息|string||
|status|状态  CREATE:创建  RUNNING:执行  FAULT:错误  SUCCESS:成功  SHUTDOWN:停止|string||
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|
|missions|预设任务列表|array|Mission|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;code|预设任务编码|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;sequence|优先级,1:低，2：普通，3：高，4：最高. 默认是2|integer(int32)||
|&emsp;&emsp;interrupt|是否可中断,True:任务可以被更高优级的新任务中断，False:必须执行完成后才能执行其他的任务。|boolean||
|&emsp;&emsp;version|预设任务版本|integer(int32)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|missionWorks|任务列表|array|MissionWork|
|&emsp;&emsp;currentActionName|指令名称|string||
|&emsp;&emsp;currentActionSequence|指令序号|integer(int32)||
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;releaseButtonAddress||integer(int32)||
|&emsp;&emsp;releaseDeviceAddress||integer(int32)||
|&emsp;&emsp;releaseSuccess||boolean||
|&emsp;&emsp;code|任务编码|string||
|&emsp;&emsp;missionCallId|预设任务ID|string||
|&emsp;&emsp;missionId|预设任务ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;schedulePlanId|调度计划的ID|string||
|&emsp;&emsp;callbackUrl|回调接口|string||
|&emsp;&emsp;sequence|优先级: 1、低  2、普通  3、高  4、最高  默认是2|integer(int32)||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;status|状态 CREATE:创建(未执行) START:开始执行 WAIT:等待(继续)执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 PAUSE:暂停 BEING_PAUSE:暂停中 BEING_RESUME:恢复中 SHUTDOWN:已停止 BEING_SHUTDOWN:停止中 WAITINPUT:等待输入|string||
|&emsp;&emsp;message|异常信息|string||
|&emsp;&emsp;interrupt|是否可中断|boolean||
|&emsp;&emsp;runtimeParam|运行时参数(json格式) 如：{"marker1":"1001"}|string||
|&emsp;&emsp;missionWorkChainId|任务链ID|string||
|&emsp;&emsp;allocationStatus|分配状态 已分配：ASSIGNED  未分配：UNASSIGNED|string||
|&emsp;&emsp;totalMileage|任务总里程 单位 米|number(double)||
|&emsp;&emsp;errorCode|异常错误代码|integer(int32)||
|&emsp;&emsp;startTime|开始时间|string(date-time)||
|&emsp;&emsp;endTime|结束时间|string(date-time)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;agvCode|机器人编码|string||
|&emsp;&emsp;triggerSelectorId|触发器ID|string||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|&emsp;&emsp;createdBy|创建者 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||
|unExecutedMissions|未执行的预设任务列表|array|Mission|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;code|预设任务编码|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;sequence|优先级,1:低，2：普通，3：高，4：最高. 默认是2|integer(int32)||
|&emsp;&emsp;interrupt|是否可中断,True:任务可以被更高优级的新任务中断，False:必须执行完成后才能执行其他的任务。|boolean||
|&emsp;&emsp;version|预设任务版本|integer(int32)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"missionChainId": "",
	"missionIds": "",
	"unExecutedMissionIds": "",
	"message": "",
	"status": "",
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"updateTime": "",
	"missions": [
		{
			"id": "",
			"code": "",
			"name": "自动运输任务",
			"description": "自动运输任务",
			"sequence": 2,
			"interrupt": false,
			"version": 0,
			"createTime": "",
			"updateTime": ""
		}
	],
	"missionWorks": [
		{
			"currentActionName": "",
			"currentActionSequence": 0,
			"id": "",
			"releaseButtonAddress": 0,
			"releaseDeviceAddress": 0,
			"releaseSuccess": true,
			"code": "",
			"missionCallId": "",
			"missionId": "",
			"name": "",
			"schedulePlanId": "",
			"callbackUrl": "",
			"sequence": 0,
			"description": "",
			"status": "",
			"message": "",
			"interrupt": true,
			"runtimeParam": "",
			"missionWorkChainId": "",
			"allocationStatus": "",
			"totalMileage": 0,
			"errorCode": 0,
			"startTime": "",
			"endTime": "",
			"createTime": "",
			"agvCode": "",
			"triggerSelectorId": "",
			"updateTime": "",
			"createdBy": ""
		}
	],
	"unExecutedMissions": [
		{
			"id": "",
			"code": "",
			"name": "自动运输任务",
			"description": "自动运输任务",
			"sequence": 2,
			"interrupt": false,
			"version": 0,
			"createTime": "",
			"updateTime": ""
		}
	]
}
```


## 更新


**接口地址**:`/api/v3/missionWorkChains/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"name": "",
	"missionChainId": "",
	"missionIds": "",
	"unExecutedMissionIds": "",
	"message": "",
	"status": "",
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"updateTime": "",
	"missions": [
		{
			"id": "",
			"code": "",
			"name": "自动运输任务",
			"description": "自动运输任务",
			"sequence": 2,
			"interrupt": false,
			"version": 0,
			"createTime": "",
			"updateTime": ""
		}
	],
	"missionWorks": [
		{
			"currentActionName": "",
			"currentActionSequence": 0,
			"id": "",
			"releaseButtonAddress": 0,
			"releaseDeviceAddress": 0,
			"releaseSuccess": true,
			"code": "",
			"missionCallId": "",
			"missionId": "",
			"name": "",
			"schedulePlanId": "",
			"callbackUrl": "",
			"sequence": 0,
			"description": "",
			"status": "",
			"message": "",
			"interrupt": true,
			"runtimeParam": "",
			"missionWorkChainId": "",
			"allocationStatus": "",
			"totalMileage": 0,
			"errorCode": 0,
			"startTime": "",
			"endTime": "",
			"createTime": "",
			"agvCode": "",
			"triggerSelectorId": "",
			"updateTime": "",
			"createdBy": ""
		}
	],
	"unExecutedMissions": [
		{
			"id": "",
			"code": "",
			"name": "自动运输任务",
			"description": "自动运输任务",
			"sequence": 2,
			"interrupt": false,
			"version": 0,
			"createTime": "",
			"updateTime": ""
		}
	]
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|任务链ID|path|true|string||
|missionWorkChain|任务链|body|true|MissionWorkChain|MissionWorkChain|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;missionChainId|预设任务链ID||false|string||
|&emsp;&emsp;missionIds|预设任务ID列表, 多个ID以逗号隔开||false|string||
|&emsp;&emsp;unExecutedMissionIds|未执行的预设任务ID列表, 多个ID以逗号隔开||false|string||
|&emsp;&emsp;message|错误信息||false|string||
|&emsp;&emsp;status|状态  CREATE:创建  RUNNING:执行  FAULT:错误  SUCCESS:成功  SHUTDOWN:停止||false|string||
|&emsp;&emsp;startTime|开始时间||false|string(date-time)||
|&emsp;&emsp;endTime|结束时间||false|string(date-time)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|&emsp;&emsp;missions|预设任务列表||false|array|Mission|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;code|预设任务编码||false|string||
|&emsp;&emsp;&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;&emsp;&emsp;sequence|优先级,1:低，2：普通，3：高，4：最高. 默认是2||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;interrupt|是否可中断,True:任务可以被更高优级的新任务中断，False:必须执行完成后才能执行其他的任务。||false|boolean||
|&emsp;&emsp;&emsp;&emsp;version|预设任务版本||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|&emsp;&emsp;missionWorks|任务列表||false|array|MissionWork|
|&emsp;&emsp;&emsp;&emsp;currentActionName|指令名称||false|string||
|&emsp;&emsp;&emsp;&emsp;currentActionSequence|指令序号||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;releaseButtonAddress|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;releaseDeviceAddress|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;releaseSuccess|||false|boolean||
|&emsp;&emsp;&emsp;&emsp;code|任务编码||false|string||
|&emsp;&emsp;&emsp;&emsp;missionCallId|预设任务ID||false|string||
|&emsp;&emsp;&emsp;&emsp;missionId|预设任务ID||false|string||
|&emsp;&emsp;&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;&emsp;&emsp;schedulePlanId|调度计划的ID||false|string||
|&emsp;&emsp;&emsp;&emsp;callbackUrl|回调接口||false|string||
|&emsp;&emsp;&emsp;&emsp;sequence|优先级: 1、低  2、普通  3、高  4、最高  默认是2||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;&emsp;&emsp;status|状态 CREATE:创建(未执行) START:开始执行 WAIT:等待(继续)执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 PAUSE:暂停 BEING_PAUSE:暂停中 BEING_RESUME:恢复中 SHUTDOWN:已停止 BEING_SHUTDOWN:停止中 WAITINPUT:等待输入||false|string||
|&emsp;&emsp;&emsp;&emsp;message|异常信息||false|string||
|&emsp;&emsp;&emsp;&emsp;interrupt|是否可中断||false|boolean||
|&emsp;&emsp;&emsp;&emsp;runtimeParam|运行时参数(json格式) 如：{"marker1":"1001"}||false|string||
|&emsp;&emsp;&emsp;&emsp;missionWorkChainId|任务链ID||false|string||
|&emsp;&emsp;&emsp;&emsp;allocationStatus|分配状态 已分配：ASSIGNED  未分配：UNASSIGNED||false|string||
|&emsp;&emsp;&emsp;&emsp;totalMileage|任务总里程 单位 米||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;errorCode|异常错误代码||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;startTime|开始时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;endTime|结束时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;agvCode|机器人编码||false|string||
|&emsp;&emsp;&emsp;&emsp;triggerSelectorId|触发器ID||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;createdBy|创建者 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass||false|string||
|&emsp;&emsp;unExecutedMissions|未执行的预设任务列表||false|array|Mission|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;code|预设任务编码||false|string||
|&emsp;&emsp;&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;&emsp;&emsp;sequence|优先级,1:低，2：普通，3：高，4：最高. 默认是2||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;interrupt|是否可中断,True:任务可以被更高优级的新任务中断，False:必须执行完成后才能执行其他的任务。||false|boolean||
|&emsp;&emsp;&emsp;&emsp;version|预设任务版本||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWorkChain|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|missionChainId|预设任务链ID|string||
|missionIds|预设任务ID列表, 多个ID以逗号隔开|string||
|unExecutedMissionIds|未执行的预设任务ID列表, 多个ID以逗号隔开|string||
|message|错误信息|string||
|status|状态  CREATE:创建  RUNNING:执行  FAULT:错误  SUCCESS:成功  SHUTDOWN:停止|string||
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|
|missions|预设任务列表|array|Mission|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;code|预设任务编码|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;sequence|优先级,1:低，2：普通，3：高，4：最高. 默认是2|integer(int32)||
|&emsp;&emsp;interrupt|是否可中断,True:任务可以被更高优级的新任务中断，False:必须执行完成后才能执行其他的任务。|boolean||
|&emsp;&emsp;version|预设任务版本|integer(int32)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|missionWorks|任务列表|array|MissionWork|
|&emsp;&emsp;currentActionName|指令名称|string||
|&emsp;&emsp;currentActionSequence|指令序号|integer(int32)||
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;releaseButtonAddress||integer(int32)||
|&emsp;&emsp;releaseDeviceAddress||integer(int32)||
|&emsp;&emsp;releaseSuccess||boolean||
|&emsp;&emsp;code|任务编码|string||
|&emsp;&emsp;missionCallId|预设任务ID|string||
|&emsp;&emsp;missionId|预设任务ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;schedulePlanId|调度计划的ID|string||
|&emsp;&emsp;callbackUrl|回调接口|string||
|&emsp;&emsp;sequence|优先级: 1、低  2、普通  3、高  4、最高  默认是2|integer(int32)||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;status|状态 CREATE:创建(未执行) START:开始执行 WAIT:等待(继续)执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 PAUSE:暂停 BEING_PAUSE:暂停中 BEING_RESUME:恢复中 SHUTDOWN:已停止 BEING_SHUTDOWN:停止中 WAITINPUT:等待输入|string||
|&emsp;&emsp;message|异常信息|string||
|&emsp;&emsp;interrupt|是否可中断|boolean||
|&emsp;&emsp;runtimeParam|运行时参数(json格式) 如：{"marker1":"1001"}|string||
|&emsp;&emsp;missionWorkChainId|任务链ID|string||
|&emsp;&emsp;allocationStatus|分配状态 已分配：ASSIGNED  未分配：UNASSIGNED|string||
|&emsp;&emsp;totalMileage|任务总里程 单位 米|number(double)||
|&emsp;&emsp;errorCode|异常错误代码|integer(int32)||
|&emsp;&emsp;startTime|开始时间|string(date-time)||
|&emsp;&emsp;endTime|结束时间|string(date-time)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;agvCode|机器人编码|string||
|&emsp;&emsp;triggerSelectorId|触发器ID|string||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|&emsp;&emsp;createdBy|创建者 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||
|unExecutedMissions|未执行的预设任务列表|array|Mission|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;code|预设任务编码|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;sequence|优先级,1:低，2：普通，3：高，4：最高. 默认是2|integer(int32)||
|&emsp;&emsp;interrupt|是否可中断,True:任务可以被更高优级的新任务中断，False:必须执行完成后才能执行其他的任务。|boolean||
|&emsp;&emsp;version|预设任务版本|integer(int32)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"missionChainId": "",
	"missionIds": "",
	"unExecutedMissionIds": "",
	"message": "",
	"status": "",
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"updateTime": "",
	"missions": [
		{
			"id": "",
			"code": "",
			"name": "自动运输任务",
			"description": "自动运输任务",
			"sequence": 2,
			"interrupt": false,
			"version": 0,
			"createTime": "",
			"updateTime": ""
		}
	],
	"missionWorks": [
		{
			"currentActionName": "",
			"currentActionSequence": 0,
			"id": "",
			"releaseButtonAddress": 0,
			"releaseDeviceAddress": 0,
			"releaseSuccess": true,
			"code": "",
			"missionCallId": "",
			"missionId": "",
			"name": "",
			"schedulePlanId": "",
			"callbackUrl": "",
			"sequence": 0,
			"description": "",
			"status": "",
			"message": "",
			"interrupt": true,
			"runtimeParam": "",
			"missionWorkChainId": "",
			"allocationStatus": "",
			"totalMileage": 0,
			"errorCode": 0,
			"startTime": "",
			"endTime": "",
			"createTime": "",
			"agvCode": "",
			"triggerSelectorId": "",
			"updateTime": "",
			"createdBy": ""
		}
	],
	"unExecutedMissions": [
		{
			"id": "",
			"code": "",
			"name": "自动运输任务",
			"description": "自动运输任务",
			"sequence": 2,
			"interrupt": false,
			"version": 0,
			"createTime": "",
			"updateTime": ""
		}
	]
}
```


## 停止任务链


**接口地址**:`/api/v3/missionWorkChains/{id}/controls/stop`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|工作ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 使用语言


## 列表


**接口地址**:`/api/v3/languages`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Language|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|currentUse|当前使用语言, 中文:CHINESE  英文:ENGLISH|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"currentUse": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


## 分页查询


**接口地址**:`/api/v3/languages/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«Language»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|Language|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;currentUse|当前使用语言, 中文:CHINESE  英文:ENGLISH|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"currentUse": "",
			"createTime": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/languages/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|语言ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Language|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|currentUse|当前使用语言, 中文:CHINESE  英文:ENGLISH|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"currentUse": "",
	"createTime": "",
	"updateTime": ""
}
```


## 更新


**接口地址**:`/api/v3/languages/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"currentUse": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|语言ID|path|true|string||
|language|使用语言|body|true|Language|Language|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;currentUse|当前使用语言, 中文:CHINESE  英文:ENGLISH||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Language|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|currentUse|当前使用语言, 中文:CHINESE  英文:ENGLISH|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"currentUse": "",
	"createTime": "",
	"updateTime": ""
}
```


# 动作


## 列表


**接口地址**:`/api/v3/missionWorkActions`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWorkAction|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionActionId|预设动作ID|string||
|missionWorkId|任务ID|string||
|actionType|动作类型|string||
|name|名称|string||
|sequence|顺序编号|integer(int32)|integer(int32)|
|message|执行结果描述|string||
|parentActionId|父类动作Id|string||
|parameters|参数|string||
|status|状态 START:开始执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误|string||
|childType|子动作类型 1、IF 2、ELSE 3、WHILE|string||
|resultCode|返回编码 1001:正确编码 其他为错误编码|integer(int32)|integer(int32)|
|resultMessage|返回提示信息|string||
|resultType|返回数据区数据类型|string||
|resultData|返回数据区数据|string||
|errorCode|异常错误代码|integer(int32)|integer(int32)|
|thisLoopCompletes|当该action属于循环action的子action时，记录该action所在的本次循环执行是否完成|boolean||
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"missionActionId": "",
		"missionWorkId": "",
		"actionType": "",
		"name": "",
		"sequence": 0,
		"message": "",
		"parentActionId": "",
		"parameters": "",
		"status": "",
		"childType": "",
		"resultCode": 0,
		"resultMessage": "",
		"resultType": "",
		"resultData": "",
		"errorCode": 0,
		"thisLoopCompletes": true,
		"startTime": "",
		"endTime": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


## 分页查询


**接口地址**:`/api/v3/missionWorkActions/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«MissionWorkAction»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|MissionWorkAction|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;missionActionId|预设动作ID|string||
|&emsp;&emsp;missionWorkId|任务ID|string||
|&emsp;&emsp;actionType|动作类型|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;sequence|顺序编号|integer(int32)||
|&emsp;&emsp;message|执行结果描述|string||
|&emsp;&emsp;parentActionId|父类动作Id|string||
|&emsp;&emsp;parameters|参数|string||
|&emsp;&emsp;status|状态 START:开始执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误|string||
|&emsp;&emsp;childType|子动作类型 1、IF 2、ELSE 3、WHILE|string||
|&emsp;&emsp;resultCode|返回编码 1001:正确编码 其他为错误编码|integer(int32)||
|&emsp;&emsp;resultMessage|返回提示信息|string||
|&emsp;&emsp;resultType|返回数据区数据类型|string||
|&emsp;&emsp;resultData|返回数据区数据|string||
|&emsp;&emsp;errorCode|异常错误代码|integer(int32)||
|&emsp;&emsp;thisLoopCompletes|当该action属于循环action的子action时，记录该action所在的本次循环执行是否完成|boolean||
|&emsp;&emsp;startTime|开始时间|string(date-time)||
|&emsp;&emsp;endTime|结束时间|string(date-time)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"missionActionId": "",
			"missionWorkId": "",
			"actionType": "",
			"name": "",
			"sequence": 0,
			"message": "",
			"parentActionId": "",
			"parameters": "",
			"status": "",
			"childType": "",
			"resultCode": 0,
			"resultMessage": "",
			"resultType": "",
			"resultData": "",
			"errorCode": 0,
			"thisLoopCompletes": true,
			"startTime": "",
			"endTime": "",
			"createTime": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/missionWorkActions/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|动作ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWorkAction|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionActionId|预设动作ID|string||
|missionWorkId|任务ID|string||
|actionType|动作类型|string||
|name|名称|string||
|sequence|顺序编号|integer(int32)|integer(int32)|
|message|执行结果描述|string||
|parentActionId|父类动作Id|string||
|parameters|参数|string||
|status|状态 START:开始执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误|string||
|childType|子动作类型 1、IF 2、ELSE 3、WHILE|string||
|resultCode|返回编码 1001:正确编码 其他为错误编码|integer(int32)|integer(int32)|
|resultMessage|返回提示信息|string||
|resultType|返回数据区数据类型|string||
|resultData|返回数据区数据|string||
|errorCode|异常错误代码|integer(int32)|integer(int32)|
|thisLoopCompletes|当该action属于循环action的子action时，记录该action所在的本次循环执行是否完成|boolean||
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"missionActionId": "",
	"missionWorkId": "",
	"actionType": "",
	"name": "",
	"sequence": 0,
	"message": "",
	"parentActionId": "",
	"parameters": "",
	"status": "",
	"childType": "",
	"resultCode": 0,
	"resultMessage": "",
	"resultType": "",
	"resultData": "",
	"errorCode": 0,
	"thisLoopCompletes": true,
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"updateTime": ""
}
```


## 根据动作ID查询动作日志列表


**接口地址**:`/api/v3/missionWorkActions/{id}/missionWorkActionLogs`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|动作ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWorkActionLog|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionWorkActionId|预设动作ID|string||
|apiCode|Api编号|string||
|parameters|运行时参数|string||
|resultData|返回值|string||
|description|描述|string||
|status|状态 CREATE:创建(未执行) RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 SHUTDOWN:停止|string||
|errorMessage|错误信息|string||
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|修改时间|string(date-time)|string(date-time)|
|missionWorkId|任务ID|string||


**响应示例**:
```javascript
[
	{
		"id": "",
		"missionWorkActionId": "",
		"apiCode": "",
		"parameters": "",
		"resultData": "",
		"description": "",
		"status": "",
		"errorMessage": "",
		"startTime": "",
		"endTime": "",
		"createTime": "",
		"updateTime": "",
		"missionWorkId": ""
	}
]
```


## 根据动作ID查询参数列表


**接口地址**:`/api/v3/missionWorkActions/{id}/missionWorkActionParameters`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|动作ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWorkActionParameter|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionWorkActionId|动作ID|string||
|parameterKey|参数|string||
|parameterValue|参数值|string||
|type|数据类型|string||
|parameterType|参数类型|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"missionWorkActionId": "",
		"parameterKey": "",
		"parameterValue": "",
		"type": "",
		"parameterType": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


# 动作参数


## 列表


**接口地址**:`/api/v3/missionWorkActionParameters`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWorkActionParameter|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionWorkActionId|动作ID|string||
|parameterKey|参数|string||
|parameterValue|参数值|string||
|type|数据类型|string||
|parameterType|参数类型|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"missionWorkActionId": "",
		"parameterKey": "",
		"parameterValue": "",
		"type": "",
		"parameterType": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


## 分页查询


**接口地址**:`/api/v3/missionWorkActionParameters/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«MissionWorkActionParameter»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|MissionWorkActionParameter|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;missionWorkActionId|动作ID|string||
|&emsp;&emsp;parameterKey|参数|string||
|&emsp;&emsp;parameterValue|参数值|string||
|&emsp;&emsp;type|数据类型|string||
|&emsp;&emsp;parameterType|参数类型|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"missionWorkActionId": "",
			"parameterKey": "",
			"parameterValue": "",
			"type": "",
			"parameterType": "",
			"createTime": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/missionWorkActionParameters/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|动作参数ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWorkActionParameter|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionWorkActionId|动作ID|string||
|parameterKey|参数|string||
|parameterValue|参数值|string||
|type|数据类型|string||
|parameterType|参数类型|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"missionWorkActionId": "",
	"parameterKey": "",
	"parameterValue": "",
	"type": "",
	"parameterType": "",
	"createTime": "",
	"updateTime": ""
}
```


# 动作日志


## 列表


**接口地址**:`/api/v3/missionWorkActionLogs`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWorkActionLog|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionWorkActionId|预设动作ID|string||
|apiCode|Api编号|string||
|parameters|运行时参数|string||
|resultData|返回值|string||
|description|描述|string||
|status|状态 CREATE:创建(未执行) RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 SHUTDOWN:停止|string||
|errorMessage|错误信息|string||
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|修改时间|string(date-time)|string(date-time)|
|missionWorkId|任务ID|string||


**响应示例**:
```javascript
[
	{
		"id": "",
		"missionWorkActionId": "",
		"apiCode": "",
		"parameters": "",
		"resultData": "",
		"description": "",
		"status": "",
		"errorMessage": "",
		"startTime": "",
		"endTime": "",
		"createTime": "",
		"updateTime": "",
		"missionWorkId": ""
	}
]
```


## 创建


**接口地址**:`/api/v3/missionWorkActionLogs`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"missionWorkActionId": "",
	"apiCode": "",
	"parameters": "",
	"resultData": "",
	"description": "",
	"status": "",
	"errorMessage": "",
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"updateTime": "",
	"missionWorkId": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|missionWorkActionLog|动作指令日志|body|true|MissionWorkActionLog|MissionWorkActionLog|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;missionWorkActionId|预设动作ID||false|string||
|&emsp;&emsp;apiCode|Api编号||false|string||
|&emsp;&emsp;parameters|运行时参数||false|string||
|&emsp;&emsp;resultData|返回值||false|string||
|&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;status|状态 CREATE:创建(未执行) RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 SHUTDOWN:停止||false|string||
|&emsp;&emsp;errorMessage|错误信息||false|string||
|&emsp;&emsp;startTime|开始时间||false|string(date-time)||
|&emsp;&emsp;endTime|结束时间||false|string(date-time)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|修改时间||false|string(date-time)||
|&emsp;&emsp;missionWorkId|任务ID||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|MissionWorkActionLog|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionWorkActionId|预设动作ID|string||
|apiCode|Api编号|string||
|parameters|运行时参数|string||
|resultData|返回值|string||
|description|描述|string||
|status|状态 CREATE:创建(未执行) RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 SHUTDOWN:停止|string||
|errorMessage|错误信息|string||
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|修改时间|string(date-time)|string(date-time)|
|missionWorkId|任务ID|string||


**响应示例**:
```javascript
{
	"id": "",
	"missionWorkActionId": "",
	"apiCode": "",
	"parameters": "",
	"resultData": "",
	"description": "",
	"status": "",
	"errorMessage": "",
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"updateTime": "",
	"missionWorkId": ""
}
```


## 分页查询


**接口地址**:`/api/v3/missionWorkActionLogs/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«MissionWorkActionLog»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|MissionWorkActionLog|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;missionWorkActionId|预设动作ID|string||
|&emsp;&emsp;apiCode|Api编号|string||
|&emsp;&emsp;parameters|运行时参数|string||
|&emsp;&emsp;resultData|返回值|string||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;status|状态 CREATE:创建(未执行) RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 SHUTDOWN:停止|string||
|&emsp;&emsp;errorMessage|错误信息|string||
|&emsp;&emsp;startTime|开始时间|string(date-time)||
|&emsp;&emsp;endTime|结束时间|string(date-time)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|修改时间|string(date-time)||
|&emsp;&emsp;missionWorkId|任务ID|string||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"missionWorkActionId": "",
			"apiCode": "",
			"parameters": "",
			"resultData": "",
			"description": "",
			"status": "",
			"errorMessage": "",
			"startTime": "",
			"endTime": "",
			"createTime": "",
			"updateTime": "",
			"missionWorkId": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/missionWorkActionLogs/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|动作指令日志ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWorkActionLog|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionWorkActionId|预设动作ID|string||
|apiCode|Api编号|string||
|parameters|运行时参数|string||
|resultData|返回值|string||
|description|描述|string||
|status|状态 CREATE:创建(未执行) RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 SHUTDOWN:停止|string||
|errorMessage|错误信息|string||
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|修改时间|string(date-time)|string(date-time)|
|missionWorkId|任务ID|string||


**响应示例**:
```javascript
{
	"id": "",
	"missionWorkActionId": "",
	"apiCode": "",
	"parameters": "",
	"resultData": "",
	"description": "",
	"status": "",
	"errorMessage": "",
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"updateTime": "",
	"missionWorkId": ""
}
```


## 更新


**接口地址**:`/api/v3/missionWorkActionLogs/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"missionWorkActionId": "",
	"apiCode": "",
	"parameters": "",
	"resultData": "",
	"description": "",
	"status": "",
	"errorMessage": "",
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"updateTime": "",
	"missionWorkId": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|动作指令日志ID|path|true|string||
|missionWorkActionLog|动作指令日志|body|true|MissionWorkActionLog|MissionWorkActionLog|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;missionWorkActionId|预设动作ID||false|string||
|&emsp;&emsp;apiCode|Api编号||false|string||
|&emsp;&emsp;parameters|运行时参数||false|string||
|&emsp;&emsp;resultData|返回值||false|string||
|&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;status|状态 CREATE:创建(未执行) RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 SHUTDOWN:停止||false|string||
|&emsp;&emsp;errorMessage|错误信息||false|string||
|&emsp;&emsp;startTime|开始时间||false|string(date-time)||
|&emsp;&emsp;endTime|结束时间||false|string(date-time)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|修改时间||false|string(date-time)||
|&emsp;&emsp;missionWorkId|任务ID||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWorkActionLog|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionWorkActionId|预设动作ID|string||
|apiCode|Api编号|string||
|parameters|运行时参数|string||
|resultData|返回值|string||
|description|描述|string||
|status|状态 CREATE:创建(未执行) RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 SHUTDOWN:停止|string||
|errorMessage|错误信息|string||
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|修改时间|string(date-time)|string(date-time)|
|missionWorkId|任务ID|string||


**响应示例**:
```javascript
{
	"id": "",
	"missionWorkActionId": "",
	"apiCode": "",
	"parameters": "",
	"resultData": "",
	"description": "",
	"status": "",
	"errorMessage": "",
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"updateTime": "",
	"missionWorkId": ""
}
```


## 删除


**接口地址**:`/api/v3/missionWorkActionLogs/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|动作指令日志ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 呼叫盒


## 列表


**接口地址**:`/api/v3/missionsCall`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionCall|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|deviceAddress|设备地址|integer(int32)|integer(int32)|
|buttonAddress|按钮地址|integer(int32)|integer(int32)|
|missionId|任务ID|string||
|missionName|任务名称|string||
|missionCode|任务编号|string||
|missionWorkId|当前作业ID|string||
|status|状态 异常：ABNORMAL  已呼叫：CALLED  未呼叫：NO_CALL|string||
|message|错误信息, 状态为ABNORMAL才有值|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"name": "",
		"deviceAddress": 0,
		"buttonAddress": 0,
		"missionId": "",
		"missionName": "",
		"missionCode": "",
		"missionWorkId": "",
		"status": "",
		"message": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


## 创建


**接口地址**:`/api/v3/missionsCall`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"name": "",
	"deviceAddress": 0,
	"buttonAddress": 0,
	"missionId": "",
	"missionName": "",
	"missionCode": "",
	"missionWorkId": "",
	"status": "",
	"message": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|missionCall|呼叫盒|body|true|MissionCall|MissionCall|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;deviceAddress|设备地址||false|integer(int32)||
|&emsp;&emsp;buttonAddress|按钮地址||false|integer(int32)||
|&emsp;&emsp;missionId|任务ID||false|string||
|&emsp;&emsp;missionName|任务名称||false|string||
|&emsp;&emsp;missionCode|任务编号||false|string||
|&emsp;&emsp;missionWorkId|当前作业ID||false|string||
|&emsp;&emsp;status|状态 异常：ABNORMAL  已呼叫：CALLED  未呼叫：NO_CALL||false|string||
|&emsp;&emsp;message|错误信息, 状态为ABNORMAL才有值||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|MissionCall|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|deviceAddress|设备地址|integer(int32)|integer(int32)|
|buttonAddress|按钮地址|integer(int32)|integer(int32)|
|missionId|任务ID|string||
|missionName|任务名称|string||
|missionCode|任务编号|string||
|missionWorkId|当前作业ID|string||
|status|状态 异常：ABNORMAL  已呼叫：CALLED  未呼叫：NO_CALL|string||
|message|错误信息, 状态为ABNORMAL才有值|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"deviceAddress": 0,
	"buttonAddress": 0,
	"missionId": "",
	"missionName": "",
	"missionCode": "",
	"missionWorkId": "",
	"status": "",
	"message": "",
	"createTime": "",
	"updateTime": ""
}
```


## 分页查询


**接口地址**:`/api/v3/missionsCall/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«MissionCall»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|MissionCall|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;deviceAddress|设备地址|integer(int32)||
|&emsp;&emsp;buttonAddress|按钮地址|integer(int32)||
|&emsp;&emsp;missionId|任务ID|string||
|&emsp;&emsp;missionName|任务名称|string||
|&emsp;&emsp;missionCode|任务编号|string||
|&emsp;&emsp;missionWorkId|当前作业ID|string||
|&emsp;&emsp;status|状态 异常：ABNORMAL  已呼叫：CALLED  未呼叫：NO_CALL|string||
|&emsp;&emsp;message|错误信息, 状态为ABNORMAL才有值|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"name": "",
			"deviceAddress": 0,
			"buttonAddress": 0,
			"missionId": "",
			"missionName": "",
			"missionCode": "",
			"missionWorkId": "",
			"status": "",
			"message": "",
			"createTime": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/missionsCall/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|呼叫盒ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionCall|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|deviceAddress|设备地址|integer(int32)|integer(int32)|
|buttonAddress|按钮地址|integer(int32)|integer(int32)|
|missionId|任务ID|string||
|missionName|任务名称|string||
|missionCode|任务编号|string||
|missionWorkId|当前作业ID|string||
|status|状态 异常：ABNORMAL  已呼叫：CALLED  未呼叫：NO_CALL|string||
|message|错误信息, 状态为ABNORMAL才有值|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"deviceAddress": 0,
	"buttonAddress": 0,
	"missionId": "",
	"missionName": "",
	"missionCode": "",
	"missionWorkId": "",
	"status": "",
	"message": "",
	"createTime": "",
	"updateTime": ""
}
```


## 更新


**接口地址**:`/api/v3/missionsCall/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:根据ID更新呼叫盒信息


**请求示例**:


```javascript
{
	"id": "",
	"name": "",
	"deviceAddress": 0,
	"buttonAddress": 0,
	"missionId": "",
	"missionName": "",
	"missionCode": "",
	"missionWorkId": "",
	"status": "",
	"message": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|任务ID|path|true|string||
|missionCall|呼叫盒|body|true|MissionCall|MissionCall|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;deviceAddress|设备地址||false|integer(int32)||
|&emsp;&emsp;buttonAddress|按钮地址||false|integer(int32)||
|&emsp;&emsp;missionId|任务ID||false|string||
|&emsp;&emsp;missionName|任务名称||false|string||
|&emsp;&emsp;missionCode|任务编号||false|string||
|&emsp;&emsp;missionWorkId|当前作业ID||false|string||
|&emsp;&emsp;status|状态 异常：ABNORMAL  已呼叫：CALLED  未呼叫：NO_CALL||false|string||
|&emsp;&emsp;message|错误信息, 状态为ABNORMAL才有值||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionCall|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|deviceAddress|设备地址|integer(int32)|integer(int32)|
|buttonAddress|按钮地址|integer(int32)|integer(int32)|
|missionId|任务ID|string||
|missionName|任务名称|string||
|missionCode|任务编号|string||
|missionWorkId|当前作业ID|string||
|status|状态 异常：ABNORMAL  已呼叫：CALLED  未呼叫：NO_CALL|string||
|message|错误信息, 状态为ABNORMAL才有值|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"deviceAddress": 0,
	"buttonAddress": 0,
	"missionId": "",
	"missionName": "",
	"missionCode": "",
	"missionWorkId": "",
	"status": "",
	"message": "",
	"createTime": "",
	"updateTime": ""
}
```


## 删除


**接口地址**:`/api/v3/missionsCall/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:根据ID删除呼叫盒信息


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|呼叫盒ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 图片


## 获取图片(base64格式)


**接口地址**:`/api/v3/images/base64`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:根据图片路径获取图片


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|url|图片url|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 获取图片(文件流格式)


**接口地址**:`/api/v3/images/stream`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:根据图片路径获取图片


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|url|图片url|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 地图


## 列表


**接口地址**:`/api/v3/AGVMaps`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AGVMapResult|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|agvMap|机器人地图|AGVMap|AGVMap|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;type|类型：LASER_MAP:激光地图，VIRTUAL_MAP:虚拟地图|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;originX|中心x坐标|number(double)||
|&emsp;&emsp;originY|中心y坐标|number(double)||
|&emsp;&emsp;resolution|分辨率|number(double)||
|&emsp;&emsp;height|像素高度|number(double)||
|&emsp;&emsp;width|像素宽度|number(double)||
|&emsp;&emsp;negate|是否应该反转 白/黑   空闲/占用（阈值的解释不受影响）|number(double)||
|&emsp;&emsp;occupied_thresh|占用阀值，大于此阈值的像素被视为完全占用|number(double)||
|&emsp;&emsp;free_thresh|空闲阀值，小于此阈值的像素被认为是完全空闲的|number(double)||
|&emsp;&emsp;originYaw|角度|number(double)||
|&emsp;&emsp;image|栅格图片|string||
|lastUpdateTime|文件最后修改时间|integer(int64)|integer(int64)|


**响应示例**:
```javascript
[
	{
		"agvMap": {
			"id": "",
			"type": "",
			"name": "",
			"originX": 0,
			"originY": 0,
			"resolution": 0,
			"height": 0,
			"width": 0,
			"negate": 0,
			"occupied_thresh": 0,
			"free_thresh": 0,
			"originYaw": 0,
			"image": ""
		},
		"lastUpdateTime": 0
	}
]
```


## 创建


**接口地址**:`/api/v3/AGVMaps`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"type": "",
	"name": "",
	"originX": 0,
	"originY": 0,
	"resolution": 0,
	"height": 0,
	"width": 0,
	"negate": 0,
	"occupied_thresh": 0,
	"free_thresh": 0,
	"originYaw": 0,
	"image": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|agvMap|地图|body|true|AGVMap|AGVMap|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;type|类型：LASER_MAP:激光地图，VIRTUAL_MAP:虚拟地图||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;originX|中心x坐标||false|number(double)||
|&emsp;&emsp;originY|中心y坐标||false|number(double)||
|&emsp;&emsp;resolution|分辨率||false|number(double)||
|&emsp;&emsp;height|像素高度||false|number(double)||
|&emsp;&emsp;width|像素宽度||false|number(double)||
|&emsp;&emsp;negate|是否应该反转 白/黑   空闲/占用（阈值的解释不受影响）||false|number(double)||
|&emsp;&emsp;occupied_thresh|占用阀值，大于此阈值的像素被视为完全占用||false|number(double)||
|&emsp;&emsp;free_thresh|空闲阀值，小于此阈值的像素被认为是完全空闲的||false|number(double)||
|&emsp;&emsp;originYaw|角度||false|number(double)||
|&emsp;&emsp;image|栅格图片||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|AGVMap|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|type|类型：LASER_MAP:激光地图，VIRTUAL_MAP:虚拟地图|string||
|name|名称|string||
|originX|中心x坐标|number(double)|number(double)|
|originY|中心y坐标|number(double)|number(double)|
|resolution|分辨率|number(double)|number(double)|
|height|像素高度|number(double)|number(double)|
|width|像素宽度|number(double)|number(double)|
|negate|是否应该反转 白/黑   空闲/占用（阈值的解释不受影响）|number(double)|number(double)|
|occupied_thresh|占用阀值，大于此阈值的像素被视为完全占用|number(double)|number(double)|
|free_thresh|空闲阀值，小于此阈值的像素被认为是完全空闲的|number(double)|number(double)|
|originYaw|角度|number(double)|number(double)|
|image|栅格图片|string||


**响应示例**:
```javascript
{
	"id": "",
	"type": "",
	"name": "",
	"originX": 0,
	"originY": 0,
	"resolution": 0,
	"height": 0,
	"width": 0,
	"negate": 0,
	"occupied_thresh": 0,
	"free_thresh": 0,
	"originYaw": 0,
	"image": ""
}
```


## 地图复制


**接口地址**:`/api/v3/AGVMaps/copyMap`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:复制当前地图并生成新地图


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sourceMapName|数据源地图名称|query|true|string||
|targetMapName|目标地图名称|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 导出地图数据


**接口地址**:`/api/v3/AGVMaps/exportMapData`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:导出地图数据zip文件


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|mapName|地图id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|204|No Content||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 导入地图数据


**接口地址**:`/api/v3/AGVMaps/importMapData`


**请求方式**:`POST`


**请求数据类型**:`multipart/form-data`


**响应数据类型**:`application/json`


**接口描述**:导入地图数据zip文件


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|multiPartFile|文件|formData|true|ref||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 地图数据转换


**接口地址**:`/api/v3/AGVMaps/mapChange`


**请求方式**:`POST`


**请求数据类型**:`multipart/form-data`


**响应数据类型**:`application/json`


**接口描述**:地图数据转换


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|multipartFile|文件|formData|true|ref||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 将4.8.0的地图数据转换位4.8.2


**接口地址**:`/api/v3/AGVMaps/mapChangeV2/{agvMapName}`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json;charset=utf-8`


**接口描述**:将4.8.0的地图数据转换位4.8.2


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|agvMapName|地图名称|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 返回地图文件的压缩包


**接口地址**:`/api/v3/AGVMaps/mapSave`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:返回地图文件的压缩包


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|multipartFile|文件内容的JSON数据|body|true|JSONObject|JSONObject|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 分页查询


**接口地址**:`/api/v3/AGVMaps/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«AGVMap»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|list||array|AGVMap|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;type|类型：LASER_MAP:激光地图，VIRTUAL_MAP:虚拟地图|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;originX|中心x坐标|number(double)||
|&emsp;&emsp;originY|中心y坐标|number(double)||
|&emsp;&emsp;resolution|分辨率|number(double)||
|&emsp;&emsp;height|像素高度|number(double)||
|&emsp;&emsp;width|像素宽度|number(double)||
|&emsp;&emsp;negate|是否应该反转 白/黑   空闲/占用（阈值的解释不受影响）|number(double)||
|&emsp;&emsp;occupied_thresh|占用阀值，大于此阈值的像素被视为完全占用|number(double)||
|&emsp;&emsp;free_thresh|空闲阀值，小于此阈值的像素被认为是完全空闲的|number(double)||
|&emsp;&emsp;originYaw|角度|number(double)||
|&emsp;&emsp;image|栅格图片|string||
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pagerCount||integer(int32)|integer(int32)|
|total||integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"list": [
		{
			"id": "",
			"type": "",
			"name": "",
			"originX": 0,
			"originY": 0,
			"resolution": 0,
			"height": 0,
			"width": 0,
			"negate": 0,
			"occupied_thresh": 0,
			"free_thresh": 0,
			"originYaw": 0,
			"image": ""
		}
	],
	"pageNum": 0,
	"pageSize": 0,
	"pagerCount": 0,
	"total": 0
}
```


## 地图发布


**接口地址**:`/api/v3/AGVMaps/pushMapData/{mapName}`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:将草稿数据转为正式数据


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|mapName|地图名称|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 地图刷新


**接口地址**:`/api/v3/AGVMaps/refresh/{mapName}`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:将正式数据加载到内存


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|mapName|地图名称|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 地图保存


**接口地址**:`/api/v3/AGVMaps/saveMap/{mapName}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:将地图保存到本地数据


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|mapName|地图名称|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 删除路网


**接口地址**:`/api/v3/AGVMaps/{agvMapName}/delPaths`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"adjustActions": {
		"additionalProperties1": {
			"id": "",
			"markerId": "",
			"destMarkerId": "",
			"agvMapId": "",
			"agvRotateAngle": 0,
			"shelvesRotateAngle": 0,
			"createTime": "",
			"updateTime": ""
		}
	},
	"mapAreas": {
		"additionalProperties1": {
			"areaMarkers": [
				{
					"id": "",
					"code": "",
					"x": 0,
					"y": 0,
					"agvMapName": "",
					"angle": 0,
					"type": "",
					"covariance": "",
					"usageStatus": "",
					"dockingPoint": {
						"qrDockId": 0,
						"relativeX": 0,
						"relativeY": 0,
						"relativeAngle": 0,
						"type": "",
						"direction": 0,
						"isChargeStation": 0
					},
					"isPark": 0
				}
			],
			"id": "",
			"areaTypeId": "",
			"name": "",
			"remark": "",
			"polygon": "",
			"agvMapId": "",
			"createTime": "",
			"updateTime": ""
		}
	},
	"markers": {
		"additionalProperties1": {
			"id": "",
			"code": "",
			"x": 0,
			"y": 0,
			"agvMapName": "",
			"angle": 0,
			"type": "",
			"covariance": "",
			"usageStatus": "",
			"dockingPoint": {
				"qrDockId": 0,
				"relativeX": 0,
				"relativeY": 0,
				"relativeAngle": 0,
				"type": "",
				"direction": 0,
				"isChargeStation": 0
			},
			"isPark": 0
		}
	},
	"paths": {
		"additionalProperties1": {
			"id": "",
			"agvMapName": "",
			"startMarkerId": "",
			"endMarkerId": "",
			"startControl": "",
			"endControl": "",
			"length": 0,
			"lineType": 0,
			"direction": 0,
			"forwardAgvDirection": 0,
			"reverseAgvDirection": 0,
			"usageStatus": "",
			"autoDoorId": ""
		}
	},
	"sidePaths": {
		"additionalProperties1": {
			"id": "",
			"pathParam": {
				"safety_scanner_region": 0,
				"safety": 0,
				"max_translation_speed": 0,
				"max_rotate_speed": 0,
				"P": 0,
				"D": 0,
				"translation_acc": 0,
				"rotate_acc": 0,
				"createTime": "",
				"updateTime": "",
				"extend_bit": "",
				"extend_string": "",
				"features_requested": 0
			},
			"safetyScannerRegion": 0,
			"weightRatio": 0,
			"agvMapName": "",
			"pathId": "",
			"startMarkerId": "",
			"endMarkerId": "",
			"startControl": "",
			"endControl": "",
			"length": 0,
			"lineType": 0,
			"agvDirection": 0,
			"usageStatus": "",
			"autoDoorId": "",
			"directionAgv": 0,
			"directionAgv2": 0,
			"pathType": 0,
			"directionShelf": 0,
			"workStationCode": 0,
			"directionShelf2": 0,
			"position": 0,
			"effectivePath": 0,
			"rpmShelf": 0,
			"firstPath": 0,
			"accurateStop": 0,
			"hasAction": 0,
			"agvDirection2": 0
		}
	}
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pathResult|pathResult|body|true|PathResultData|PathResultData|
|&emsp;&emsp;adjustActions|||false|adjust_action|adjust_action|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;markerId|关联标记点id||false|string||
|&emsp;&emsp;&emsp;&emsp;destMarkerId|目标标记点id||false|string||
|&emsp;&emsp;&emsp;&emsp;agvMapId|地图id||false|string||
|&emsp;&emsp;&emsp;&emsp;agvRotateAngle|机器人旋转角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;shelvesRotateAngle|货架旋转角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|&emsp;&emsp;mapAreas|||false|MapArea|MapArea|
|&emsp;&emsp;&emsp;&emsp;areaMarkers|||false|array|Marker|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;code|编码||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;x|x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;y|y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;agvMapName|地图名称||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;angle|角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;covariance|协方差矩阵||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dockingPoint|对接点||false|DockingPoint|DockingPoint|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;qrDockId|地面二维码坐标ID||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeX|相对x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeY|相对y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeAngle|相对角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;isPark|是否可泊车, 0:不可泊车，1：可泊车||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;areaTypeId|区域类型 单机区域:SINGLE_AGV_AREA||false|string||
|&emsp;&emsp;&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;&emsp;&emsp;remark|备注||false|string||
|&emsp;&emsp;&emsp;&emsp;polygon|区域坐标列表||false|string||
|&emsp;&emsp;&emsp;&emsp;agvMapId|地图的ID||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|&emsp;&emsp;markers|||false|Marker|Marker|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;code|编码||false|string||
|&emsp;&emsp;&emsp;&emsp;x|x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;y|y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;agvMapName|地图名称||false|string||
|&emsp;&emsp;&emsp;&emsp;angle|角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点||false|string||
|&emsp;&emsp;&emsp;&emsp;covariance|协方差矩阵||false|string||
|&emsp;&emsp;&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;&emsp;&emsp;dockingPoint|对接点||false|DockingPoint|DockingPoint|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;qrDockId|地面二维码坐标ID||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeX|相对x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeY|相对y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeAngle|相对角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;isPark|是否可泊车, 0:不可泊车，1：可泊车||false|integer(int32)||
|&emsp;&emsp;paths|||false|Path|Path|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;agvMapName|地图ID||false|string||
|&emsp;&emsp;&emsp;&emsp;startMarkerId|开始标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;endMarkerId|结束标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;startControl|开始点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;endControl|结束点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;length|长度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;direction|方向 0、双向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;forwardAgvDirection|正向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;reverseAgvDirection|反向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;&emsp;&emsp;autoDoorId|自动门ID||false|string||
|&emsp;&emsp;sidePaths|||false|SidePath|SidePath|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;pathParam|路径参数||false|PathParam|PathParam|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;safety_scanner_region|雷达避障区域 0、默认区域||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;safety|避障 1、打开避障  2、关闭避障||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;max_translation_speed|最大平移速度 >0 m/s||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;max_rotate_speed|最大旋转速度 rad/s >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;P|平移加速比例控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;D|平移加速微分控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;translation_acc|平移加（减）速度 m/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rotate_acc|旋转加（减）速度 rad/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;updateTime|修改时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;extend_bit|拓展布尔||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;extend_string|拓展字符串||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;features_requested|融合特征 1、开启 0、关闭||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;safetyScannerRegion|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;weightRatio|路径权重系数||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;agvMapName|地图ID||false|string||
|&emsp;&emsp;&emsp;&emsp;pathId|路径ID||false|string||
|&emsp;&emsp;&emsp;&emsp;startMarkerId|开始标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;endMarkerId|结束标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;startControl|开始点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;endControl|结束点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;length|长度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;agvDirection|agv方向: 0、双向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;&emsp;&emsp;autoDoorId|自动门ID||false|string||
|&emsp;&emsp;&emsp;&emsp;directionAgv|AGV要朝向的角度（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;directionAgv2|AGV要朝向的角度2（地图坐标系下）（预留，暂不使用）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;pathType|路径类型: 0、普通路径 1、二维码对接路径 2、脱离对接路径||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;directionShelf|货架要朝向的角度1（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;workStationCode|工位编码||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;directionShelf2|货架要朝向的角度2（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;position|位置，1、起始点 2、结束点||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;effectivePath|生效路径 1、全部路径 2、第一段路径||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;rpmShelf|uint, 货架旋转速度，单位，转/每分钟||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;firstPath|是否是首段路径 1、是 0、否||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;accurateStop|是否启用末端精定位: 0不启用 1启用，默认是不启用||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;hasAction|是否有动作,1、有 0、没有||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;agvDirection2|agv方向2: -180 ~ 180||false|integer(int32)||
|agvMapName|地图名称|path|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 修改路网


**接口地址**:`/api/v3/AGVMaps/{agvMapName}/updatePaths`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"adjustActions": {
		"additionalProperties1": {
			"id": "",
			"markerId": "",
			"destMarkerId": "",
			"agvMapId": "",
			"agvRotateAngle": 0,
			"shelvesRotateAngle": 0,
			"createTime": "",
			"updateTime": ""
		}
	},
	"mapAreas": {
		"additionalProperties1": {
			"areaMarkers": [
				{
					"id": "",
					"code": "",
					"x": 0,
					"y": 0,
					"agvMapName": "",
					"angle": 0,
					"type": "",
					"covariance": "",
					"usageStatus": "",
					"dockingPoint": {
						"qrDockId": 0,
						"relativeX": 0,
						"relativeY": 0,
						"relativeAngle": 0,
						"type": "",
						"direction": 0,
						"isChargeStation": 0
					},
					"isPark": 0
				}
			],
			"id": "",
			"areaTypeId": "",
			"name": "",
			"remark": "",
			"polygon": "",
			"agvMapId": "",
			"createTime": "",
			"updateTime": ""
		}
	},
	"markers": {
		"additionalProperties1": {
			"id": "",
			"code": "",
			"x": 0,
			"y": 0,
			"agvMapName": "",
			"angle": 0,
			"type": "",
			"covariance": "",
			"usageStatus": "",
			"dockingPoint": {
				"qrDockId": 0,
				"relativeX": 0,
				"relativeY": 0,
				"relativeAngle": 0,
				"type": "",
				"direction": 0,
				"isChargeStation": 0
			},
			"isPark": 0
		}
	},
	"paths": {
		"additionalProperties1": {
			"id": "",
			"agvMapName": "",
			"startMarkerId": "",
			"endMarkerId": "",
			"startControl": "",
			"endControl": "",
			"length": 0,
			"lineType": 0,
			"direction": 0,
			"forwardAgvDirection": 0,
			"reverseAgvDirection": 0,
			"usageStatus": "",
			"autoDoorId": ""
		}
	},
	"sidePaths": {
		"additionalProperties1": {
			"id": "",
			"pathParam": {
				"safety_scanner_region": 0,
				"safety": 0,
				"max_translation_speed": 0,
				"max_rotate_speed": 0,
				"P": 0,
				"D": 0,
				"translation_acc": 0,
				"rotate_acc": 0,
				"createTime": "",
				"updateTime": "",
				"extend_bit": "",
				"extend_string": "",
				"features_requested": 0
			},
			"safetyScannerRegion": 0,
			"weightRatio": 0,
			"agvMapName": "",
			"pathId": "",
			"startMarkerId": "",
			"endMarkerId": "",
			"startControl": "",
			"endControl": "",
			"length": 0,
			"lineType": 0,
			"agvDirection": 0,
			"usageStatus": "",
			"autoDoorId": "",
			"directionAgv": 0,
			"directionAgv2": 0,
			"pathType": 0,
			"directionShelf": 0,
			"workStationCode": 0,
			"directionShelf2": 0,
			"position": 0,
			"effectivePath": 0,
			"rpmShelf": 0,
			"firstPath": 0,
			"accurateStop": 0,
			"hasAction": 0,
			"agvDirection2": 0
		}
	}
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pathResult|修改路网数据|body|true|PathResultData|PathResultData|
|&emsp;&emsp;adjustActions|||false|adjust_action|adjust_action|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;markerId|关联标记点id||false|string||
|&emsp;&emsp;&emsp;&emsp;destMarkerId|目标标记点id||false|string||
|&emsp;&emsp;&emsp;&emsp;agvMapId|地图id||false|string||
|&emsp;&emsp;&emsp;&emsp;agvRotateAngle|机器人旋转角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;shelvesRotateAngle|货架旋转角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|&emsp;&emsp;mapAreas|||false|MapArea|MapArea|
|&emsp;&emsp;&emsp;&emsp;areaMarkers|||false|array|Marker|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;code|编码||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;x|x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;y|y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;agvMapName|地图名称||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;angle|角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;covariance|协方差矩阵||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dockingPoint|对接点||false|DockingPoint|DockingPoint|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;qrDockId|地面二维码坐标ID||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeX|相对x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeY|相对y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeAngle|相对角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;isPark|是否可泊车, 0:不可泊车，1：可泊车||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;areaTypeId|区域类型 单机区域:SINGLE_AGV_AREA||false|string||
|&emsp;&emsp;&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;&emsp;&emsp;remark|备注||false|string||
|&emsp;&emsp;&emsp;&emsp;polygon|区域坐标列表||false|string||
|&emsp;&emsp;&emsp;&emsp;agvMapId|地图的ID||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|&emsp;&emsp;markers|||false|Marker|Marker|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;code|编码||false|string||
|&emsp;&emsp;&emsp;&emsp;x|x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;y|y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;agvMapName|地图名称||false|string||
|&emsp;&emsp;&emsp;&emsp;angle|角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点||false|string||
|&emsp;&emsp;&emsp;&emsp;covariance|协方差矩阵||false|string||
|&emsp;&emsp;&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;&emsp;&emsp;dockingPoint|对接点||false|DockingPoint|DockingPoint|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;qrDockId|地面二维码坐标ID||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeX|相对x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeY|相对y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeAngle|相对角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;isPark|是否可泊车, 0:不可泊车，1：可泊车||false|integer(int32)||
|&emsp;&emsp;paths|||false|Path|Path|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;agvMapName|地图ID||false|string||
|&emsp;&emsp;&emsp;&emsp;startMarkerId|开始标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;endMarkerId|结束标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;startControl|开始点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;endControl|结束点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;length|长度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;direction|方向 0、双向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;forwardAgvDirection|正向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;reverseAgvDirection|反向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;&emsp;&emsp;autoDoorId|自动门ID||false|string||
|&emsp;&emsp;sidePaths|||false|SidePath|SidePath|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;pathParam|路径参数||false|PathParam|PathParam|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;safety_scanner_region|雷达避障区域 0、默认区域||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;safety|避障 1、打开避障  2、关闭避障||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;max_translation_speed|最大平移速度 >0 m/s||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;max_rotate_speed|最大旋转速度 rad/s >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;P|平移加速比例控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;D|平移加速微分控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;translation_acc|平移加（减）速度 m/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rotate_acc|旋转加（减）速度 rad/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;updateTime|修改时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;extend_bit|拓展布尔||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;extend_string|拓展字符串||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;features_requested|融合特征 1、开启 0、关闭||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;safetyScannerRegion|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;weightRatio|路径权重系数||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;agvMapName|地图ID||false|string||
|&emsp;&emsp;&emsp;&emsp;pathId|路径ID||false|string||
|&emsp;&emsp;&emsp;&emsp;startMarkerId|开始标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;endMarkerId|结束标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;startControl|开始点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;endControl|结束点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;length|长度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;agvDirection|agv方向: 0、双向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;&emsp;&emsp;autoDoorId|自动门ID||false|string||
|&emsp;&emsp;&emsp;&emsp;directionAgv|AGV要朝向的角度（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;directionAgv2|AGV要朝向的角度2（地图坐标系下）（预留，暂不使用）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;pathType|路径类型: 0、普通路径 1、二维码对接路径 2、脱离对接路径||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;directionShelf|货架要朝向的角度1（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;workStationCode|工位编码||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;directionShelf2|货架要朝向的角度2（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;position|位置，1、起始点 2、结束点||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;effectivePath|生效路径 1、全部路径 2、第一段路径||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;rpmShelf|uint, 货架旋转速度，单位，转/每分钟||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;firstPath|是否是首段路径 1、是 0、否||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;accurateStop|是否启用末端精定位: 0不启用 1启用，默认是不启用||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;hasAction|是否有动作,1、有 0、没有||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;agvDirection2|agv方向2: -180 ~ 180||false|integer(int32)||
|agvMapName|地图名称|path|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 详情


**接口地址**:`/api/v3/AGVMaps/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|地图ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AGVMap|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|type|类型：LASER_MAP:激光地图，VIRTUAL_MAP:虚拟地图|string||
|name|名称|string||
|originX|中心x坐标|number(double)|number(double)|
|originY|中心y坐标|number(double)|number(double)|
|resolution|分辨率|number(double)|number(double)|
|height|像素高度|number(double)|number(double)|
|width|像素宽度|number(double)|number(double)|
|negate|是否应该反转 白/黑   空闲/占用（阈值的解释不受影响）|number(double)|number(double)|
|occupied_thresh|占用阀值，大于此阈值的像素被视为完全占用|number(double)|number(double)|
|free_thresh|空闲阀值，小于此阈值的像素被认为是完全空闲的|number(double)|number(double)|
|originYaw|角度|number(double)|number(double)|
|image|栅格图片|string||


**响应示例**:
```javascript
{
	"id": "",
	"type": "",
	"name": "",
	"originX": 0,
	"originY": 0,
	"resolution": 0,
	"height": 0,
	"width": 0,
	"negate": 0,
	"occupied_thresh": 0,
	"free_thresh": 0,
	"originYaw": 0,
	"image": ""
}
```


## 更新


**接口地址**:`/api/v3/AGVMaps/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"type": "",
	"name": "",
	"originX": 0,
	"originY": 0,
	"resolution": 0,
	"height": 0,
	"width": 0,
	"negate": 0,
	"occupied_thresh": 0,
	"free_thresh": 0,
	"originYaw": 0,
	"image": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|agvMap|地图|body|true|AGVMap|AGVMap|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;type|类型：LASER_MAP:激光地图，VIRTUAL_MAP:虚拟地图||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;originX|中心x坐标||false|number(double)||
|&emsp;&emsp;originY|中心y坐标||false|number(double)||
|&emsp;&emsp;resolution|分辨率||false|number(double)||
|&emsp;&emsp;height|像素高度||false|number(double)||
|&emsp;&emsp;width|像素宽度||false|number(double)||
|&emsp;&emsp;negate|是否应该反转 白/黑   空闲/占用（阈值的解释不受影响）||false|number(double)||
|&emsp;&emsp;occupied_thresh|占用阀值，大于此阈值的像素被视为完全占用||false|number(double)||
|&emsp;&emsp;free_thresh|空闲阀值，小于此阈值的像素被认为是完全空闲的||false|number(double)||
|&emsp;&emsp;originYaw|角度||false|number(double)||
|&emsp;&emsp;image|栅格图片||false|string||
|id|地图ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AGVMap|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|type|类型：LASER_MAP:激光地图，VIRTUAL_MAP:虚拟地图|string||
|name|名称|string||
|originX|中心x坐标|number(double)|number(double)|
|originY|中心y坐标|number(double)|number(double)|
|resolution|分辨率|number(double)|number(double)|
|height|像素高度|number(double)|number(double)|
|width|像素宽度|number(double)|number(double)|
|negate|是否应该反转 白/黑   空闲/占用（阈值的解释不受影响）|number(double)|number(double)|
|occupied_thresh|占用阀值，大于此阈值的像素被视为完全占用|number(double)|number(double)|
|free_thresh|空闲阀值，小于此阈值的像素被认为是完全空闲的|number(double)|number(double)|
|originYaw|角度|number(double)|number(double)|
|image|栅格图片|string||


**响应示例**:
```javascript
{
	"id": "",
	"type": "",
	"name": "",
	"originX": 0,
	"originY": 0,
	"resolution": 0,
	"height": 0,
	"width": 0,
	"negate": 0,
	"occupied_thresh": 0,
	"free_thresh": 0,
	"originYaw": 0,
	"image": ""
}
```


## 删除


**接口地址**:`/api/v3/AGVMaps/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|地图ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 删除草稿数据


**接口地址**:`/api/v3/AGVMaps/{id}/deleteDraftFile`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:删除当前草稿数据


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|地图ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 查询区域列表


**接口地址**:`/api/v3/AGVMaps/{id}/eventAreas`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:根据地图ID获取地图区域列表


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|地图ID|path|true|string||
|isDraft|isDraft|query|false|boolean||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MapArea|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|areaMarkers||array|Marker|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;code|编码|string||
|&emsp;&emsp;x|x坐标|number(double)||
|&emsp;&emsp;y|y坐标|number(double)||
|&emsp;&emsp;agvMapName|地图名称|string||
|&emsp;&emsp;angle|角度|number(double)||
|&emsp;&emsp;type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点|string||
|&emsp;&emsp;covariance|协方差矩阵|string||
|&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|&emsp;&emsp;dockingPoint|对接点|DockingPoint|DockingPoint|
|&emsp;&emsp;&emsp;&emsp;qrDockId|地面二维码坐标ID||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;relativeX|相对x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;relativeY|相对y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;relativeAngle|相对角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点||false|string||
|&emsp;&emsp;&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否||false|integer(int32)||
|&emsp;&emsp;isPark|是否可泊车, 0:不可泊车，1：可泊车|integer(int32)||
|id|ID|string||
|areaTypeId|区域类型 单机区域:SINGLE_AGV_AREA|string||
|name|名称|string||
|remark|备注|string||
|polygon|区域坐标列表|string||
|agvMapId|地图的ID|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"areaMarkers": [
			{
				"id": "",
				"code": "",
				"x": 0,
				"y": 0,
				"agvMapName": "",
				"angle": 0,
				"type": "",
				"covariance": "",
				"usageStatus": "",
				"dockingPoint": {
					"qrDockId": 0,
					"relativeX": 0,
					"relativeY": 0,
					"relativeAngle": 0,
					"type": "",
					"direction": 0,
					"isChargeStation": 0
				},
				"isPark": 0
			}
		],
		"id": "",
		"areaTypeId": "",
		"name": "",
		"remark": "",
		"polygon": "",
		"agvMapId": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


## 查询地图文件最后一次修改的时间


**接口地址**:`/api/v3/AGVMaps/{id}/getLastUpdateTime`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 查询标记列表


**接口地址**:`/api/v3/AGVMaps/{id}/markers`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:根据地图ID获取标记列表


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|地图ID|path|true|string||
|isDraft|isDraft|query|false|boolean||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Marker|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|code|编码|string||
|x|x坐标|number(double)|number(double)|
|y|y坐标|number(double)|number(double)|
|agvMapName|地图名称|string||
|angle|角度|number(double)|number(double)|
|type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点|string||
|covariance|协方差矩阵|string||
|usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|dockingPoint|对接点|DockingPoint|DockingPoint|
|&emsp;&emsp;qrDockId|地面二维码坐标ID|integer(int32)||
|&emsp;&emsp;relativeX|相对x坐标|number(double)||
|&emsp;&emsp;relativeY|相对y坐标|number(double)||
|&emsp;&emsp;relativeAngle|相对角度|number(double)||
|&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点|string||
|&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接|integer(int32)||
|&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否|integer(int32)||
|isPark|是否可泊车, 0:不可泊车，1：可泊车|integer(int32)|integer(int32)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"code": "",
		"x": 0,
		"y": 0,
		"agvMapName": "",
		"angle": 0,
		"type": "",
		"covariance": "",
		"usageStatus": "",
		"dockingPoint": {
			"qrDockId": 0,
			"relativeX": 0,
			"relativeY": 0,
			"relativeAngle": 0,
			"type": "",
			"direction": 0,
			"isChargeStation": 0
		},
		"isPark": 0
	}
]
```


## 查询路径列表


**接口地址**:`/api/v3/AGVMaps/{id}/paths`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:根据地图ID获取路径列表


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|地图ID|path|true|string||
|isDraft|isDraft|query|false|boolean||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Path|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|agvMapName|地图ID|string||
|startMarkerId|开始标记点|string||
|endMarkerId|结束标记点|string||
|startControl|开始点的控制点xy坐标|string||
|endControl|结束点的控制点xy坐标|string||
|length|长度|number(double)|number(double)|
|lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）|integer(int32)|integer(int32)|
|direction|方向 0、双向 1、正向 2、反向|integer(int32)|integer(int32)|
|forwardAgvDirection|正向行驶时agv方向 1、正向 2、反向|integer(int32)|integer(int32)|
|reverseAgvDirection|反向行驶时agv方向 1、正向 2、反向|integer(int32)|integer(int32)|
|usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|autoDoorId|自动门ID|string||


**响应示例**:
```javascript
[
	{
		"id": "",
		"agvMapName": "",
		"startMarkerId": "",
		"endMarkerId": "",
		"startControl": "",
		"endControl": "",
		"length": 0,
		"lineType": 0,
		"direction": 0,
		"forwardAgvDirection": 0,
		"reverseAgvDirection": 0,
		"usageStatus": "",
		"autoDoorId": ""
	}
]
```


## 查询当前地图是否有草稿数据


**接口地址**:`/api/v3/AGVMaps/{id}/selectDraftFile`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:查询当前地图是否有草稿数据


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|地图ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 地图元素配置


## 列表


**接口地址**:`/api/v3/mapElementConfig`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MapElementConfig|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|mwidthHeight||number(double)|number(double)|
|id|Id|string||
|mapName|地图名称|string||
|lineWidthHeight|路径的宽高|number(double)|number(double)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"mwidthHeight": 0,
		"id": "",
		"mapName": "",
		"lineWidthHeight": 0,
		"createTime": "",
		"updateTime": ""
	}
]
```


## 创建


**接口地址**:`/api/v3/mapElementConfig`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"mwidthHeight": 0,
	"id": "",
	"mapName": "",
	"lineWidthHeight": 0,
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|mapElementConfig|地图元素配置|body|true|MapElementConfig|MapElementConfig|
|&emsp;&emsp;mwidthHeight|||false|number(double)||
|&emsp;&emsp;id|Id||false|string||
|&emsp;&emsp;mapName|地图名称||false|string||
|&emsp;&emsp;lineWidthHeight|路径的宽高||false|number(double)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|MapElementConfig|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|mwidthHeight||number(double)|number(double)|
|id|Id|string||
|mapName|地图名称|string||
|lineWidthHeight|路径的宽高|number(double)|number(double)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"mwidthHeight": 0,
	"id": "",
	"mapName": "",
	"lineWidthHeight": 0,
	"createTime": "",
	"updateTime": ""
}
```


## 根据地图名称查询


**接口地址**:`/api/v3/mapElementConfig/getByMapName/{mapName}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|mapName|地图名称|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MapElementConfig|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|mwidthHeight||number(double)|number(double)|
|id|Id|string||
|mapName|地图名称|string||
|lineWidthHeight|路径的宽高|number(double)|number(double)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"mwidthHeight": 0,
	"id": "",
	"mapName": "",
	"lineWidthHeight": 0,
	"createTime": "",
	"updateTime": ""
}
```


## 分页查询


**接口地址**:`/api/v3/mapElementConfig/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«MapElementConfig»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|MapElementConfig|
|&emsp;&emsp;mwidthHeight||number(double)||
|&emsp;&emsp;id|Id|string||
|&emsp;&emsp;mapName|地图名称|string||
|&emsp;&emsp;lineWidthHeight|路径的宽高|number(double)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"mwidthHeight": 0,
			"id": "",
			"mapName": "",
			"lineWidthHeight": 0,
			"createTime": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/mapElementConfig/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|地图元素配置ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MapElementConfig|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|mwidthHeight||number(double)|number(double)|
|id|Id|string||
|mapName|地图名称|string||
|lineWidthHeight|路径的宽高|number(double)|number(double)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"mwidthHeight": 0,
	"id": "",
	"mapName": "",
	"lineWidthHeight": 0,
	"createTime": "",
	"updateTime": ""
}
```


## 更新


**接口地址**:`/api/v3/mapElementConfig/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"mwidthHeight": 0,
	"id": "",
	"mapName": "",
	"lineWidthHeight": 0,
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|地图元素配置ID|path|true|string||
|mapElementConfig|地图元素配置|body|true|MapElementConfig|MapElementConfig|
|&emsp;&emsp;mwidthHeight|||false|number(double)||
|&emsp;&emsp;id|Id||false|string||
|&emsp;&emsp;mapName|地图名称||false|string||
|&emsp;&emsp;lineWidthHeight|路径的宽高||false|number(double)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MapElementConfig|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|mwidthHeight||number(double)|number(double)|
|id|Id|string||
|mapName|地图名称|string||
|lineWidthHeight|路径的宽高|number(double)|number(double)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"mwidthHeight": 0,
	"id": "",
	"mapName": "",
	"lineWidthHeight": 0,
	"createTime": "",
	"updateTime": ""
}
```


## 删除


**接口地址**:`/api/v3/mapElementConfig/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|地图元素配置ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 地图区域


## 列表


**接口地址**:`/api/v3/mapAreas`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|agvMapName|地图名称||true|String|String|
|isDraft|是否查询草稿数据|query|true|boolean||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MapArea|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|areaMarkers||array|Marker|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;code|编码|string||
|&emsp;&emsp;x|x坐标|number(double)||
|&emsp;&emsp;y|y坐标|number(double)||
|&emsp;&emsp;agvMapName|地图名称|string||
|&emsp;&emsp;angle|角度|number(double)||
|&emsp;&emsp;type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点|string||
|&emsp;&emsp;covariance|协方差矩阵|string||
|&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|&emsp;&emsp;dockingPoint|对接点|DockingPoint|DockingPoint|
|&emsp;&emsp;&emsp;&emsp;qrDockId|地面二维码坐标ID||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;relativeX|相对x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;relativeY|相对y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;relativeAngle|相对角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点||false|string||
|&emsp;&emsp;&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否||false|integer(int32)||
|&emsp;&emsp;isPark|是否可泊车, 0:不可泊车，1：可泊车|integer(int32)||
|id|ID|string||
|areaTypeId|区域类型 单机区域:SINGLE_AGV_AREA|string||
|name|名称|string||
|remark|备注|string||
|polygon|区域坐标列表|string||
|agvMapId|地图的ID|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"areaMarkers": [
			{
				"id": "",
				"code": "",
				"x": 0,
				"y": 0,
				"agvMapName": "",
				"angle": 0,
				"type": "",
				"covariance": "",
				"usageStatus": "",
				"dockingPoint": {
					"qrDockId": 0,
					"relativeX": 0,
					"relativeY": 0,
					"relativeAngle": 0,
					"type": "",
					"direction": 0,
					"isChargeStation": 0
				},
				"isPark": 0
			}
		],
		"id": "",
		"areaTypeId": "",
		"name": "",
		"remark": "",
		"polygon": "",
		"agvMapId": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


## 创建


**接口地址**:`/api/v3/mapAreas`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"areaMarkers": [
		{
			"id": "",
			"code": "",
			"x": 0,
			"y": 0,
			"agvMapName": "",
			"angle": 0,
			"type": "",
			"covariance": "",
			"usageStatus": "",
			"dockingPoint": {
				"qrDockId": 0,
				"relativeX": 0,
				"relativeY": 0,
				"relativeAngle": 0,
				"type": "",
				"direction": 0,
				"isChargeStation": 0
			},
			"isPark": 0
		}
	],
	"id": "",
	"areaTypeId": "",
	"name": "",
	"remark": "",
	"polygon": "",
	"agvMapId": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|mapArea|地图区域|body|true|MapArea|MapArea|
|&emsp;&emsp;areaMarkers|||false|array|Marker|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;code|编码||false|string||
|&emsp;&emsp;&emsp;&emsp;x|x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;y|y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;agvMapName|地图名称||false|string||
|&emsp;&emsp;&emsp;&emsp;angle|角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点||false|string||
|&emsp;&emsp;&emsp;&emsp;covariance|协方差矩阵||false|string||
|&emsp;&emsp;&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;&emsp;&emsp;dockingPoint|对接点||false|DockingPoint|DockingPoint|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;qrDockId|地面二维码坐标ID||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeX|相对x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeY|相对y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeAngle|相对角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;isPark|是否可泊车, 0:不可泊车，1：可泊车||false|integer(int32)||
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;areaTypeId|区域类型 单机区域:SINGLE_AGV_AREA||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;remark|备注||false|string||
|&emsp;&emsp;polygon|区域坐标列表||false|string||
|&emsp;&emsp;agvMapId|地图的ID||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|MapArea|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|areaMarkers||array|Marker|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;code|编码|string||
|&emsp;&emsp;x|x坐标|number(double)||
|&emsp;&emsp;y|y坐标|number(double)||
|&emsp;&emsp;agvMapName|地图名称|string||
|&emsp;&emsp;angle|角度|number(double)||
|&emsp;&emsp;type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点|string||
|&emsp;&emsp;covariance|协方差矩阵|string||
|&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|&emsp;&emsp;dockingPoint|对接点|DockingPoint|DockingPoint|
|&emsp;&emsp;&emsp;&emsp;qrDockId|地面二维码坐标ID||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;relativeX|相对x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;relativeY|相对y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;relativeAngle|相对角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点||false|string||
|&emsp;&emsp;&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否||false|integer(int32)||
|&emsp;&emsp;isPark|是否可泊车, 0:不可泊车，1：可泊车|integer(int32)||
|id|ID|string||
|areaTypeId|区域类型 单机区域:SINGLE_AGV_AREA|string||
|name|名称|string||
|remark|备注|string||
|polygon|区域坐标列表|string||
|agvMapId|地图的ID|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"areaMarkers": [
		{
			"id": "",
			"code": "",
			"x": 0,
			"y": 0,
			"agvMapName": "",
			"angle": 0,
			"type": "",
			"covariance": "",
			"usageStatus": "",
			"dockingPoint": {
				"qrDockId": 0,
				"relativeX": 0,
				"relativeY": 0,
				"relativeAngle": 0,
				"type": "",
				"direction": 0,
				"isChargeStation": 0
			},
			"isPark": 0
		}
	],
	"id": "",
	"areaTypeId": "",
	"name": "",
	"remark": "",
	"polygon": "",
	"agvMapId": "",
	"createTime": "",
	"updateTime": ""
}
```


## 分页查询


**接口地址**:`/api/v3/mapAreas/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|isDraft|isDraft|query|true|boolean||
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«MapArea»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|list||array|MapArea|
|&emsp;&emsp;areaMarkers||array|Marker|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;code|编码||false|string||
|&emsp;&emsp;&emsp;&emsp;x|x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;y|y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;agvMapName|地图名称||false|string||
|&emsp;&emsp;&emsp;&emsp;angle|角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点||false|string||
|&emsp;&emsp;&emsp;&emsp;covariance|协方差矩阵||false|string||
|&emsp;&emsp;&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;&emsp;&emsp;dockingPoint|对接点||false|DockingPoint|DockingPoint|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;qrDockId|地面二维码坐标ID||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeX|相对x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeY|相对y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeAngle|相对角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;isPark|是否可泊车, 0:不可泊车，1：可泊车||false|integer(int32)||
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;areaTypeId|区域类型 单机区域:SINGLE_AGV_AREA|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;remark|备注|string||
|&emsp;&emsp;polygon|区域坐标列表|string||
|&emsp;&emsp;agvMapId|地图的ID|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pagerCount||integer(int32)|integer(int32)|
|total||integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"list": [
		{
			"areaMarkers": [
				{
					"id": "",
					"code": "",
					"x": 0,
					"y": 0,
					"agvMapName": "",
					"angle": 0,
					"type": "",
					"covariance": "",
					"usageStatus": "",
					"dockingPoint": {
						"qrDockId": 0,
						"relativeX": 0,
						"relativeY": 0,
						"relativeAngle": 0,
						"type": "",
						"direction": 0,
						"isChargeStation": 0
					},
					"isPark": 0
				}
			],
			"id": "",
			"areaTypeId": "",
			"name": "",
			"remark": "",
			"polygon": "",
			"agvMapId": "",
			"createTime": "",
			"updateTime": ""
		}
	],
	"pageNum": 0,
	"pageSize": 0,
	"pagerCount": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/mapAreas/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|地图区域ID|path|true|string||
|isDraft|是否查询草稿数据|query|true|boolean||
|mapName|地图名称|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MapArea|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|areaMarkers||array|Marker|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;code|编码|string||
|&emsp;&emsp;x|x坐标|number(double)||
|&emsp;&emsp;y|y坐标|number(double)||
|&emsp;&emsp;agvMapName|地图名称|string||
|&emsp;&emsp;angle|角度|number(double)||
|&emsp;&emsp;type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点|string||
|&emsp;&emsp;covariance|协方差矩阵|string||
|&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|&emsp;&emsp;dockingPoint|对接点|DockingPoint|DockingPoint|
|&emsp;&emsp;&emsp;&emsp;qrDockId|地面二维码坐标ID||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;relativeX|相对x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;relativeY|相对y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;relativeAngle|相对角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点||false|string||
|&emsp;&emsp;&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否||false|integer(int32)||
|&emsp;&emsp;isPark|是否可泊车, 0:不可泊车，1：可泊车|integer(int32)||
|id|ID|string||
|areaTypeId|区域类型 单机区域:SINGLE_AGV_AREA|string||
|name|名称|string||
|remark|备注|string||
|polygon|区域坐标列表|string||
|agvMapId|地图的ID|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"areaMarkers": [
		{
			"id": "",
			"code": "",
			"x": 0,
			"y": 0,
			"agvMapName": "",
			"angle": 0,
			"type": "",
			"covariance": "",
			"usageStatus": "",
			"dockingPoint": {
				"qrDockId": 0,
				"relativeX": 0,
				"relativeY": 0,
				"relativeAngle": 0,
				"type": "",
				"direction": 0,
				"isChargeStation": 0
			},
			"isPark": 0
		}
	],
	"id": "",
	"areaTypeId": "",
	"name": "",
	"remark": "",
	"polygon": "",
	"agvMapId": "",
	"createTime": "",
	"updateTime": ""
}
```


## 更新


**接口地址**:`/api/v3/mapAreas/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"areaMarkers": [
		{
			"id": "",
			"code": "",
			"x": 0,
			"y": 0,
			"agvMapName": "",
			"angle": 0,
			"type": "",
			"covariance": "",
			"usageStatus": "",
			"dockingPoint": {
				"qrDockId": 0,
				"relativeX": 0,
				"relativeY": 0,
				"relativeAngle": 0,
				"type": "",
				"direction": 0,
				"isChargeStation": 0
			},
			"isPark": 0
		}
	],
	"id": "",
	"areaTypeId": "",
	"name": "",
	"remark": "",
	"polygon": "",
	"agvMapId": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|地图区域ID|path|true|string||
|mapArea|地图区域|body|true|MapArea|MapArea|
|&emsp;&emsp;areaMarkers|||false|array|Marker|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;code|编码||false|string||
|&emsp;&emsp;&emsp;&emsp;x|x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;y|y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;agvMapName|地图名称||false|string||
|&emsp;&emsp;&emsp;&emsp;angle|角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点||false|string||
|&emsp;&emsp;&emsp;&emsp;covariance|协方差矩阵||false|string||
|&emsp;&emsp;&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;&emsp;&emsp;dockingPoint|对接点||false|DockingPoint|DockingPoint|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;qrDockId|地面二维码坐标ID||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeX|相对x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeY|相对y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;relativeAngle|相对角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;isPark|是否可泊车, 0:不可泊车，1：可泊车||false|integer(int32)||
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;areaTypeId|区域类型 单机区域:SINGLE_AGV_AREA||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;remark|备注||false|string||
|&emsp;&emsp;polygon|区域坐标列表||false|string||
|&emsp;&emsp;agvMapId|地图的ID||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MapArea|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|areaMarkers||array|Marker|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;code|编码|string||
|&emsp;&emsp;x|x坐标|number(double)||
|&emsp;&emsp;y|y坐标|number(double)||
|&emsp;&emsp;agvMapName|地图名称|string||
|&emsp;&emsp;angle|角度|number(double)||
|&emsp;&emsp;type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点|string||
|&emsp;&emsp;covariance|协方差矩阵|string||
|&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|&emsp;&emsp;dockingPoint|对接点|DockingPoint|DockingPoint|
|&emsp;&emsp;&emsp;&emsp;qrDockId|地面二维码坐标ID||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;relativeX|相对x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;relativeY|相对y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;relativeAngle|相对角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点||false|string||
|&emsp;&emsp;&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否||false|integer(int32)||
|&emsp;&emsp;isPark|是否可泊车, 0:不可泊车，1：可泊车|integer(int32)||
|id|ID|string||
|areaTypeId|区域类型 单机区域:SINGLE_AGV_AREA|string||
|name|名称|string||
|remark|备注|string||
|polygon|区域坐标列表|string||
|agvMapId|地图的ID|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"areaMarkers": [
		{
			"id": "",
			"code": "",
			"x": 0,
			"y": 0,
			"agvMapName": "",
			"angle": 0,
			"type": "",
			"covariance": "",
			"usageStatus": "",
			"dockingPoint": {
				"qrDockId": 0,
				"relativeX": 0,
				"relativeY": 0,
				"relativeAngle": 0,
				"type": "",
				"direction": 0,
				"isChargeStation": 0
			},
			"isPark": 0
		}
	],
	"id": "",
	"areaTypeId": "",
	"name": "",
	"remark": "",
	"polygon": "",
	"agvMapId": "",
	"createTime": "",
	"updateTime": ""
}
```


## 删除


**接口地址**:`/api/v3/mapAreas/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|地图区域ID|path|true|string||
|mapName|地图名称|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 声光配置信息


## 音频文件列表


**接口地址**:`/api/v3/SoundLight/configs`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:音频文件列表


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 删除音频


**接口地址**:`/api/v3/SoundLight/configs`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:删除音频文件


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|fileName|删除文件名称|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 下载音频文件


**接口地址**:`/api/v3/SoundLight/configs/download/audioFile`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:下载音频文件


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|fileName|下载文件名称|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 获取灯光列表


**接口地址**:`/api/v3/SoundLight/configs/query/lightList`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:灯光列表


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 声光配置表


**接口地址**:`/api/v3/SoundLight/configs/query/soundLightList`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:声光配置列表


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 更新声光列表


**接口地址**:`/api/v3/SoundLight/configs/update/soundLightList`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:更新声光配置列表


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|info|配置信息||true|List|List|
|reset|更新 0、更新 1、重置||true|Integer|Integer|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 上传音频文件


**接口地址**:`/api/v3/SoundLight/configs/upload/audioFile`


**请求方式**:`POST`


**请求数据类型**:`multipart/form-data`


**响应数据类型**:`application/json`


**接口描述**:上传音频文件


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|multipartFile|文件|formData|true|ref||
|uploadFileName|上传文件名称|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 外部动作调用


## 外部动作调用执行


**接口地址**:`/api/v3/foreignAction`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"actionParameter": {},
	"actionType": "",
	"agvCode": "",
	"callBackUrl": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|foreignActionRequestParam|外部动作调用请求参数|body|true|ForeignActionRequestParam|ForeignActionRequestParam|
|&emsp;&emsp;actionParameter|动作参数||false|object||
|&emsp;&emsp;actionType|动作类型||false|string||
|&emsp;&emsp;agvCode|机器人编号||false|string||
|&emsp;&emsp;callBackUrl|回传url||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|ForeignActionResponseParam|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|actionId|code为0时，异常信息说明|string||
|code|1:成功 0:失败|integer(int32)|integer(int32)|
|msg|响应信息|string||


**响应示例**:
```javascript
{
	"actionId": "",
	"code": 0,
	"msg": ""
}
```


## 外部动作状态查询


**接口地址**:`/api/v3/foreignAction/{actionId}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|actionId|外部动作调用actionId|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created|ForeignActionResponseParam|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|actionId|code为0时，异常信息说明|string||
|code|1:成功 0:失败|integer(int32)|integer(int32)|
|msg|响应信息|string||


**响应示例**:
```javascript
{
	"actionId": "",
	"code": 0,
	"msg": ""
}
```


# 心跳检测


## 心跳检测


**接口地址**:`/api/v3/alives`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:根据该接口完成心跳检测


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 摄像头预置参数


## 列表


**接口地址**:`/api/v3/cameraPresetParams`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|CameraPresetParam|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|osd_str|OSD字符叠加(图片水印)|string||
|pBrightValue|亮度指针,取值范围[1,10]|integer(int32)|integer(int32)|
|pContrastValue|对比度指针,取值范围[1,10]|integer(int32)|integer(int32)|
|pSaturationValue|饱和度指针,取值范围[1,10]|integer(int32)|integer(int32)|
|byExposureModeSet|球机的曝光模式：0-手动模式，1-自动曝光，2-光圈优先，3-快门优先，4-增益优先|integer(int32)|integer(int32)|
|byShutterSet|快门等级：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230|integer(int32)|integer(int32)|
|byMaxShutterSet|最大快门值：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230(在自动曝光模式下生效)|integer(int32)|integer(int32)|
|byMinShutterSet|最小快门值：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230(在自动曝光模式下生效)|integer(int32)|integer(int32)|
|byMaxIrisSet|最大光圈限制值(在自动曝光模式下生效)，取值范围：[0,100]|integer(int32)|integer(int32)|
|byMinIrisSet|最小光圈限制值(在自动曝光模式下生效)，取值范围：[0,100]|integer(int32)|integer(int32)|
|byFocusMode|聚焦模式：0-自动，1-手动，2-半自动|integer(int32)|integer(int32)|
|wZoomPos|Z参数（变倍参数）|integer(int32)|integer(int32)|
|iIrisSet|光圈，为实际取值*100的值，0表示关闭光圈|integer(int32)|integer(int32)|
|xmlFocus|可见光单目摄像头调整焦距|integer(int32)|integer(int32)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"name": "",
		"osd_str": "",
		"pBrightValue": 0,
		"pContrastValue": 0,
		"pSaturationValue": 0,
		"byExposureModeSet": 0,
		"byShutterSet": 0,
		"byMaxShutterSet": 0,
		"byMinShutterSet": 0,
		"byMaxIrisSet": 0,
		"byMinIrisSet": 0,
		"byFocusMode": 0,
		"wZoomPos": 0,
		"iIrisSet": 0,
		"xmlFocus": 0,
		"createTime": "",
		"updateTime": ""
	}
]
```


## 创建


**接口地址**:`/api/v3/cameraPresetParams`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"name": "",
	"osd_str": "",
	"pBrightValue": 0,
	"pContrastValue": 0,
	"pSaturationValue": 0,
	"byExposureModeSet": 0,
	"byShutterSet": 0,
	"byMaxShutterSet": 0,
	"byMinShutterSet": 0,
	"byMaxIrisSet": 0,
	"byMinIrisSet": 0,
	"byFocusMode": 0,
	"wZoomPos": 0,
	"iIrisSet": 0,
	"xmlFocus": 0,
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|cameraPresetParam|摄像头预置参数|body|true|CameraPresetParam|CameraPresetParam|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;osd_str|OSD字符叠加(图片水印)||false|string||
|&emsp;&emsp;pBrightValue|亮度指针,取值范围[1,10]||false|integer(int32)||
|&emsp;&emsp;pContrastValue|对比度指针,取值范围[1,10]||false|integer(int32)||
|&emsp;&emsp;pSaturationValue|饱和度指针,取值范围[1,10]||false|integer(int32)||
|&emsp;&emsp;byExposureModeSet|球机的曝光模式：0-手动模式，1-自动曝光，2-光圈优先，3-快门优先，4-增益优先||false|integer(int32)||
|&emsp;&emsp;byShutterSet|快门等级：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230||false|integer(int32)||
|&emsp;&emsp;byMaxShutterSet|最大快门值：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230(在自动曝光模式下生效)||false|integer(int32)||
|&emsp;&emsp;byMinShutterSet|最小快门值：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230(在自动曝光模式下生效)||false|integer(int32)||
|&emsp;&emsp;byMaxIrisSet|最大光圈限制值(在自动曝光模式下生效)，取值范围：[0,100]||false|integer(int32)||
|&emsp;&emsp;byMinIrisSet|最小光圈限制值(在自动曝光模式下生效)，取值范围：[0,100]||false|integer(int32)||
|&emsp;&emsp;byFocusMode|聚焦模式：0-自动，1-手动，2-半自动||false|integer(int32)||
|&emsp;&emsp;wZoomPos|Z参数（变倍参数）||false|integer(int32)||
|&emsp;&emsp;iIrisSet|光圈，为实际取值*100的值，0表示关闭光圈||false|integer(int32)||
|&emsp;&emsp;xmlFocus|可见光单目摄像头调整焦距||false|integer(int32)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|CameraPresetParam|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|osd_str|OSD字符叠加(图片水印)|string||
|pBrightValue|亮度指针,取值范围[1,10]|integer(int32)|integer(int32)|
|pContrastValue|对比度指针,取值范围[1,10]|integer(int32)|integer(int32)|
|pSaturationValue|饱和度指针,取值范围[1,10]|integer(int32)|integer(int32)|
|byExposureModeSet|球机的曝光模式：0-手动模式，1-自动曝光，2-光圈优先，3-快门优先，4-增益优先|integer(int32)|integer(int32)|
|byShutterSet|快门等级：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230|integer(int32)|integer(int32)|
|byMaxShutterSet|最大快门值：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230(在自动曝光模式下生效)|integer(int32)|integer(int32)|
|byMinShutterSet|最小快门值：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230(在自动曝光模式下生效)|integer(int32)|integer(int32)|
|byMaxIrisSet|最大光圈限制值(在自动曝光模式下生效)，取值范围：[0,100]|integer(int32)|integer(int32)|
|byMinIrisSet|最小光圈限制值(在自动曝光模式下生效)，取值范围：[0,100]|integer(int32)|integer(int32)|
|byFocusMode|聚焦模式：0-自动，1-手动，2-半自动|integer(int32)|integer(int32)|
|wZoomPos|Z参数（变倍参数）|integer(int32)|integer(int32)|
|iIrisSet|光圈，为实际取值*100的值，0表示关闭光圈|integer(int32)|integer(int32)|
|xmlFocus|可见光单目摄像头调整焦距|integer(int32)|integer(int32)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"osd_str": "",
	"pBrightValue": 0,
	"pContrastValue": 0,
	"pSaturationValue": 0,
	"byExposureModeSet": 0,
	"byShutterSet": 0,
	"byMaxShutterSet": 0,
	"byMinShutterSet": 0,
	"byMaxIrisSet": 0,
	"byMinIrisSet": 0,
	"byFocusMode": 0,
	"wZoomPos": 0,
	"iIrisSet": 0,
	"xmlFocus": 0,
	"createTime": "",
	"updateTime": ""
}
```


## 分页查询


**接口地址**:`/api/v3/cameraPresetParams/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«CameraPresetParam»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|CameraPresetParam|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;osd_str|OSD字符叠加(图片水印)|string||
|&emsp;&emsp;pBrightValue|亮度指针,取值范围[1,10]|integer(int32)||
|&emsp;&emsp;pContrastValue|对比度指针,取值范围[1,10]|integer(int32)||
|&emsp;&emsp;pSaturationValue|饱和度指针,取值范围[1,10]|integer(int32)||
|&emsp;&emsp;byExposureModeSet|球机的曝光模式：0-手动模式，1-自动曝光，2-光圈优先，3-快门优先，4-增益优先|integer(int32)||
|&emsp;&emsp;byShutterSet|快门等级：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230|integer(int32)||
|&emsp;&emsp;byMaxShutterSet|最大快门值：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230(在自动曝光模式下生效)|integer(int32)||
|&emsp;&emsp;byMinShutterSet|最小快门值：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230(在自动曝光模式下生效)|integer(int32)||
|&emsp;&emsp;byMaxIrisSet|最大光圈限制值(在自动曝光模式下生效)，取值范围：[0,100]|integer(int32)||
|&emsp;&emsp;byMinIrisSet|最小光圈限制值(在自动曝光模式下生效)，取值范围：[0,100]|integer(int32)||
|&emsp;&emsp;byFocusMode|聚焦模式：0-自动，1-手动，2-半自动|integer(int32)||
|&emsp;&emsp;wZoomPos|Z参数（变倍参数）|integer(int32)||
|&emsp;&emsp;iIrisSet|光圈，为实际取值*100的值，0表示关闭光圈|integer(int32)||
|&emsp;&emsp;xmlFocus|可见光单目摄像头调整焦距|integer(int32)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"name": "",
			"osd_str": "",
			"pBrightValue": 0,
			"pContrastValue": 0,
			"pSaturationValue": 0,
			"byExposureModeSet": 0,
			"byShutterSet": 0,
			"byMaxShutterSet": 0,
			"byMinShutterSet": 0,
			"byMaxIrisSet": 0,
			"byMinIrisSet": 0,
			"byFocusMode": 0,
			"wZoomPos": 0,
			"iIrisSet": 0,
			"xmlFocus": 0,
			"createTime": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/cameraPresetParams/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|摄像头预置参数ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|CameraPresetParam|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|osd_str|OSD字符叠加(图片水印)|string||
|pBrightValue|亮度指针,取值范围[1,10]|integer(int32)|integer(int32)|
|pContrastValue|对比度指针,取值范围[1,10]|integer(int32)|integer(int32)|
|pSaturationValue|饱和度指针,取值范围[1,10]|integer(int32)|integer(int32)|
|byExposureModeSet|球机的曝光模式：0-手动模式，1-自动曝光，2-光圈优先，3-快门优先，4-增益优先|integer(int32)|integer(int32)|
|byShutterSet|快门等级：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230|integer(int32)|integer(int32)|
|byMaxShutterSet|最大快门值：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230(在自动曝光模式下生效)|integer(int32)|integer(int32)|
|byMinShutterSet|最小快门值：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230(在自动曝光模式下生效)|integer(int32)|integer(int32)|
|byMaxIrisSet|最大光圈限制值(在自动曝光模式下生效)，取值范围：[0,100]|integer(int32)|integer(int32)|
|byMinIrisSet|最小光圈限制值(在自动曝光模式下生效)，取值范围：[0,100]|integer(int32)|integer(int32)|
|byFocusMode|聚焦模式：0-自动，1-手动，2-半自动|integer(int32)|integer(int32)|
|wZoomPos|Z参数（变倍参数）|integer(int32)|integer(int32)|
|iIrisSet|光圈，为实际取值*100的值，0表示关闭光圈|integer(int32)|integer(int32)|
|xmlFocus|可见光单目摄像头调整焦距|integer(int32)|integer(int32)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"osd_str": "",
	"pBrightValue": 0,
	"pContrastValue": 0,
	"pSaturationValue": 0,
	"byExposureModeSet": 0,
	"byShutterSet": 0,
	"byMaxShutterSet": 0,
	"byMinShutterSet": 0,
	"byMaxIrisSet": 0,
	"byMinIrisSet": 0,
	"byFocusMode": 0,
	"wZoomPos": 0,
	"iIrisSet": 0,
	"xmlFocus": 0,
	"createTime": "",
	"updateTime": ""
}
```


## 更新


**接口地址**:`/api/v3/cameraPresetParams/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"name": "",
	"osd_str": "",
	"pBrightValue": 0,
	"pContrastValue": 0,
	"pSaturationValue": 0,
	"byExposureModeSet": 0,
	"byShutterSet": 0,
	"byMaxShutterSet": 0,
	"byMinShutterSet": 0,
	"byMaxIrisSet": 0,
	"byMinIrisSet": 0,
	"byFocusMode": 0,
	"wZoomPos": 0,
	"iIrisSet": 0,
	"xmlFocus": 0,
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|cameraPresetParam|摄像头预置参数|body|true|CameraPresetParam|CameraPresetParam|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;osd_str|OSD字符叠加(图片水印)||false|string||
|&emsp;&emsp;pBrightValue|亮度指针,取值范围[1,10]||false|integer(int32)||
|&emsp;&emsp;pContrastValue|对比度指针,取值范围[1,10]||false|integer(int32)||
|&emsp;&emsp;pSaturationValue|饱和度指针,取值范围[1,10]||false|integer(int32)||
|&emsp;&emsp;byExposureModeSet|球机的曝光模式：0-手动模式，1-自动曝光，2-光圈优先，3-快门优先，4-增益优先||false|integer(int32)||
|&emsp;&emsp;byShutterSet|快门等级：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230||false|integer(int32)||
|&emsp;&emsp;byMaxShutterSet|最大快门值：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230(在自动曝光模式下生效)||false|integer(int32)||
|&emsp;&emsp;byMinShutterSet|最小快门值：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230(在自动曝光模式下生效)||false|integer(int32)||
|&emsp;&emsp;byMaxIrisSet|最大光圈限制值(在自动曝光模式下生效)，取值范围：[0,100]||false|integer(int32)||
|&emsp;&emsp;byMinIrisSet|最小光圈限制值(在自动曝光模式下生效)，取值范围：[0,100]||false|integer(int32)||
|&emsp;&emsp;byFocusMode|聚焦模式：0-自动，1-手动，2-半自动||false|integer(int32)||
|&emsp;&emsp;wZoomPos|Z参数（变倍参数）||false|integer(int32)||
|&emsp;&emsp;iIrisSet|光圈，为实际取值*100的值，0表示关闭光圈||false|integer(int32)||
|&emsp;&emsp;xmlFocus|可见光单目摄像头调整焦距||false|integer(int32)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|id|摄像头预置参数ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|CameraPresetParam|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|osd_str|OSD字符叠加(图片水印)|string||
|pBrightValue|亮度指针,取值范围[1,10]|integer(int32)|integer(int32)|
|pContrastValue|对比度指针,取值范围[1,10]|integer(int32)|integer(int32)|
|pSaturationValue|饱和度指针,取值范围[1,10]|integer(int32)|integer(int32)|
|byExposureModeSet|球机的曝光模式：0-手动模式，1-自动曝光，2-光圈优先，3-快门优先，4-增益优先|integer(int32)|integer(int32)|
|byShutterSet|快门等级：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230|integer(int32)|integer(int32)|
|byMaxShutterSet|最大快门值：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230(在自动曝光模式下生效)|integer(int32)|integer(int32)|
|byMinShutterSet|最小快门值：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230(在自动曝光模式下生效)|integer(int32)|integer(int32)|
|byMaxIrisSet|最大光圈限制值(在自动曝光模式下生效)，取值范围：[0,100]|integer(int32)|integer(int32)|
|byMinIrisSet|最小光圈限制值(在自动曝光模式下生效)，取值范围：[0,100]|integer(int32)|integer(int32)|
|byFocusMode|聚焦模式：0-自动，1-手动，2-半自动|integer(int32)|integer(int32)|
|wZoomPos|Z参数（变倍参数）|integer(int32)|integer(int32)|
|iIrisSet|光圈，为实际取值*100的值，0表示关闭光圈|integer(int32)|integer(int32)|
|xmlFocus|可见光单目摄像头调整焦距|integer(int32)|integer(int32)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"osd_str": "",
	"pBrightValue": 0,
	"pContrastValue": 0,
	"pSaturationValue": 0,
	"byExposureModeSet": 0,
	"byShutterSet": 0,
	"byMaxShutterSet": 0,
	"byMinShutterSet": 0,
	"byMaxIrisSet": 0,
	"byMinIrisSet": 0,
	"byFocusMode": 0,
	"wZoomPos": 0,
	"iIrisSet": 0,
	"xmlFocus": 0,
	"createTime": "",
	"updateTime": ""
}
```


## 删除


**接口地址**:`/api/v3/cameraPresetParams/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|摄像头预置参数ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 日志操作,默认操作地址：/server/ads/logs/


## 查询日志文件列表


**接口地址**:`/api/v3/logHandle`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|logFileDir|日志参数，选填：logFileDir(文件夹，默认为/server/ads/logs/)|query|true|ref||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|LogParam|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|fileName|操作文件或文件夹名称|string||
|isFile|是否为文件 false:文件，true:文件夹|boolean||
|lastModified|最后修改时间|integer(int64)|integer(int64)|


**响应示例**:
```javascript
[
	{
		"fileName": "",
		"isFile": true,
		"lastModified": 0
	}
]
```


## 删除日志文件或文件夹


**接口地址**:`/api/v3/logHandle`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|filePath|日志参数，必填：filePath(被删除文件名全路径)|query|true|ref||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 下载日志文件


**接口地址**:`/api/v3/logHandle/downLogFile`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|filePath|日志参数，必填：filePath(下载文件名称，/文件名)|query|true|ref||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 查看日志文件(可通过关键字查询)


**接口地址**:`/api/v3/logHandle/viewFile`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json;charset=UTF-8`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|filePath|filePath(文件名称，全路径)|query|true|string||
|keyWord|keyWord(关键字)||true|String|String|
|keyword|keyword|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 机器人


## 详情


**接口地址**:`/api/v3/vehicles`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|VehicleData|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|AGV ID|string||
|name|名称|string||
|ip|IP|string||
|agvMapId|AGV地图ID|string||
|navigationType|导航类型 LASER:激光导航 QR_CODE:二维码导航 BLEND:混合导航|string||
|connectedTime|连接时间|string(date-time)|string(date-time)|
|mapStatus|地图状态 1、正常 2、无地图 3、未同步 4、同步中 5、同步失败 6、未启用|integer(int32)|integer(int32)|
|recordStatus|录制状态 1、未录制 2、开始中 3、录制栅格 4、录制特征|integer(int32)|integer(int32)|
|workStatus|任务状态 1、空闲 2、任务 3、充电 4、归位|integer(int32)|integer(int32)|
|abnormalStatus|异常状态 1、无异常 2、任务异常 3、充电异常 4、归位异常|integer(int32)|integer(int32)|
|connectStatus|连接状态 1、已连接 2、连接中 3、未连接|integer(int32)|integer(int32)|
|manualStatus|手动状态 1、无动作 2、动作中 3、动作异常|integer(int32)|integer(int32)|
|controlMode|控制模式 1、自动模式 2、手动模式 3、录制模式|integer(int32)|integer(int32)|
|vehicleInfo|基本信息|VehicleDefaultInfo|VehicleDefaultInfo|
|&emsp;&emsp;agv|AGV|AGVInfo|AGVInfo|
|&emsp;&emsp;&emsp;&emsp;agv_id|AGV ID||false|string||
|&emsp;&emsp;&emsp;&emsp;agv_name|AGV名称||false|string||
|&emsp;&emsp;&emsp;&emsp;agv_version|AGV版本号||false|string||
|&emsp;&emsp;device|设备|DeviceInfo|DeviceInfo|
|&emsp;&emsp;&emsp;&emsp;imu|IMU型号||false|string||
|&emsp;&emsp;&emsp;&emsp;motor|电机型号||false|string||
|&emsp;&emsp;&emsp;&emsp;pc|工控机型号||false|string||
|&emsp;&emsp;network|网络|NetworkInfo|NetworkInfo|
|&emsp;&emsp;&emsp;&emsp;net_ip|机器人IP||false|string||
|&emsp;&emsp;&emsp;&emsp;net_mac|机器人MAC地址||false|string||
|&emsp;&emsp;&emsp;&emsp;net_protocol_version|网络协议版本||false|string||
|&emsp;&emsp;&emsp;&emsp;net_wifi_rssi|机器人当前连接的信号强度||false|string||
|&emsp;&emsp;&emsp;&emsp;net_wifi_ssid|机器人连接的AP名称||false|string||
|&emsp;&emsp;shape|外型|ShapeInfo|ShapeInfo|
|&emsp;&emsp;&emsp;&emsp;length|机器人长度 单位：mm||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;radius|机器人半径 单位：mm||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;width|机器人宽度 单位：mm||false|integer(int32)||
|vehicleDeviceInfoList|设备信息|array|VehicleDeviceInfo|
|&emsp;&emsp;id|id|string||
|&emsp;&emsp;model|型号|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;property|参数|object||
|&emsp;&emsp;type|类型|string||
|missionWork|任务信息|MissionWork|MissionWork|
|&emsp;&emsp;currentActionName|指令名称|string||
|&emsp;&emsp;currentActionSequence|指令序号|integer(int32)||
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;releaseButtonAddress||integer(int32)||
|&emsp;&emsp;releaseDeviceAddress||integer(int32)||
|&emsp;&emsp;releaseSuccess||boolean||
|&emsp;&emsp;code|任务编码|string||
|&emsp;&emsp;missionCallId|预设任务ID|string||
|&emsp;&emsp;missionId|预设任务ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;schedulePlanId|调度计划的ID|string||
|&emsp;&emsp;callbackUrl|回调接口|string||
|&emsp;&emsp;sequence|优先级: 1、低  2、普通  3、高  4、最高  默认是2|integer(int32)||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;status|状态 CREATE:创建(未执行) START:开始执行 WAIT:等待(继续)执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 PAUSE:暂停 BEING_PAUSE:暂停中 BEING_RESUME:恢复中 SHUTDOWN:已停止 BEING_SHUTDOWN:停止中 WAITINPUT:等待输入|string||
|&emsp;&emsp;message|异常信息|string||
|&emsp;&emsp;interrupt|是否可中断|boolean||
|&emsp;&emsp;runtimeParam|运行时参数(json格式) 如：{"marker1":"1001"}|string||
|&emsp;&emsp;missionWorkChainId|任务链ID|string||
|&emsp;&emsp;allocationStatus|分配状态 已分配：ASSIGNED  未分配：UNASSIGNED|string||
|&emsp;&emsp;totalMileage|任务总里程 单位 米|number(double)||
|&emsp;&emsp;errorCode|异常错误代码|integer(int32)||
|&emsp;&emsp;startTime|开始时间|string(date-time)||
|&emsp;&emsp;endTime|结束时间|string(date-time)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;agvCode|机器人编码|string||
|&emsp;&emsp;triggerSelectorId|触发器ID|string||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|&emsp;&emsp;createdBy|创建者 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||
|defaultVehicleStatus|状态信息|DefaultVehicleStatus|DefaultVehicleStatus|
|&emsp;&emsp;agvStatus||agv_status|agv_status|
|&emsp;&emsp;&emsp;&emsp;resetting_status|||false|boolean||
|&emsp;&emsp;&emsp;&emsp;unlock_brake_status|||false|boolean||
|&emsp;&emsp;battery|电池|BatteryStatus|BatteryStatus|
|&emsp;&emsp;&emsp;&emsp;battery_charge|充电电流, 单位 A||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;battery_discharge|放电电流，单位A||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;battery_fullcapacity|电池充满的电池电量 单位 mah||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;battery_leftcapacity|电池剩余的电池电量 单位 mah||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;battery_status|电池是否正在充电,1：充电，0：未充电||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;battery_temp|机器人电池电芯最高温度, 单位 ℃||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;battery_value|机器人电池电量, 范围 [0, 100]||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;battery_voltage|电压, 单位 V||false|number(double)||
|&emsp;&emsp;deviceStatus|机器人配置状态|DeviceStatus|DeviceStatus|
|&emsp;&emsp;&emsp;&emsp;motorStatus|||false|motor_status|motor_status|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;left_error|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;left_status|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;lift_error|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;lift_status|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;right_error|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;right_status|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rotate_error|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rotate_status|||false|integer(int32)||
|&emsp;&emsp;emec|电机|EmecStatus|EmecStatus|
|&emsp;&emsp;&emsp;&emsp;emc_jam_start_time|路径导航急停时间||false|integer(int64)||
|&emsp;&emsp;&emsp;&emsp;emc_reason|急停原因  1:表示急停按钮处于激活状态(按下) 2:安全激光雷达触发导致的急停 3:碰撞开类导致的急停 4:路径导航急停||false|array|integer|
|&emsp;&emsp;&emsp;&emsp;emc_status|急停状态 0:未急停, 1:急停||false|integer(int32)||
|&emsp;&emsp;fallPrevent|防跌落|FallPreventStatus|FallPreventStatus|
|&emsp;&emsp;&emsp;&emsp;status|||false|string||
|&emsp;&emsp;&emsp;&emsp;switch_|||false|string||
|&emsp;&emsp;lift|升降平台|LiftStatus|LiftStatus|
|&emsp;&emsp;&emsp;&emsp;controller_error|升降平台是否报错  1、报错 0、未报错||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;emc_stop|升降平台是否急停  1、急停 0、未急停||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;goal_reached|升降平台是否到达目标位置  1、到达 0、未到达||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;limit|升降平台是否触发限位 1、触发 0、未触发||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;origin_point|升降平台是否找到原点  1、找到 0、未找到||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;position|升降平台的当前位置脉冲数||false|integer(int64)||
|&emsp;&emsp;&emsp;&emsp;status_word|升降电机状态字||false|integer(int32)||
|&emsp;&emsp;map|地图|MapStatus|MapStatus|
|&emsp;&emsp;&emsp;&emsp;current_feature_id|当前正在生效的特征地图Id||false|string||
|&emsp;&emsp;&emsp;&emsp;current_map_id|地图ID||false|string||
|&emsp;&emsp;&emsp;&emsp;current_map_type|地图类型 1:激光地图  2:虚拟地图  3:CAD地图||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;scan_feature_status|特征地图状态  1：正在扫图  2：表示暂停中  3：表示建图完成||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;scan_status|扫图状态  1：正在扫图  2：表示暂停中  3：表示建图完成||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;scan_update_status|更新地图状态 1:正在更新地图 2：暂停更新地图 3：更新地图完成||false|integer(int32)||
|&emsp;&emsp;motorStatus||motor_status|motor_status|
|&emsp;&emsp;&emsp;&emsp;left_error|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;left_status|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;lift_error|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;lift_status|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;right_error|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;right_status|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;rotate_error|||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;rotate_status|||false|integer(int32)||
|&emsp;&emsp;position|位置|PositionStatus|PositionStatus|
|&emsp;&emsp;&emsp;&emsp;covariance|协方差矩阵||false|array|number|
|&emsp;&emsp;&emsp;&emsp;pos_angle|角度 单位:rad||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;pos_confidence|机器人激光定位的置信度, 范围 [0, 1]||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;pos_current_station|当前站点ID||false|string||
|&emsp;&emsp;&emsp;&emsp;pos_islocated|当前是否有定位，0，未定位，1，已定位||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;pos_x|X位置||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;pos_y|Y位置||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;segment_id|机器人在那条曲线上||false|string||
|&emsp;&emsp;&emsp;&emsp;t|机器人在曲线上的位置||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;update_time_millis|||false|integer(int64)||
|&emsp;&emsp;runtime|运行|RuntimeStatus|RuntimeStatus|
|&emsp;&emsp;&emsp;&emsp;agv_mode|控制模式 1:自动 2:手动||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;agv_status|当前状态 1:空闲中,2:动作中 3,被阻档,4冲电中,5异常中,6急停7:正在进行重定位||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;controller_temp|控制器当前温度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;docking_status|对接状态 1:未对接,2:对接中 3,已对接,4脱离中,5异常||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;follow_status|随动状态 0、无  1、顶升货架随动||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;motor_temp|电机当前温度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;odom|累计行驶里程, 单位:米(m)||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;time|今天开机运行时间,单位:小时(h)||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;total_time|累计运行时间, 单位:小时(h)||false|number(double)||
|&emsp;&emsp;speed|速度|SpeedStatus|SpeedStatus|
|&emsp;&emsp;&emsp;&emsp;speed_r_vx|X方向接收到的速度,单位 m/s||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;speed_r_vy|Y方向收到的速度,单位 m/s||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;speed_r_w|收到的角速度,单位 rad/s||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;speed_vx|X方向实际的速度,单位 m/s||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;speed_vy|Y方向实际的速度,单位 m/s||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;speed_w|实际的角速度,单位 rad/s||false|number(double)||
|&emsp;&emsp;status|异常状态|error_status|error_status|
|&emsp;&emsp;&emsp;&emsp;err_code|||false|array|integer|
|&emsp;&emsp;&emsp;&emsp;robot_status|||false|string||
|errorMessage|错误信息(目前只提示智能充电/归位的报错信息)|string||
|missionWorkChainId|任务链ID|string||
|paths|AGV规划的路径|array|Path|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;agvMapName|地图ID|string||
|&emsp;&emsp;startMarkerId|开始标记点|string||
|&emsp;&emsp;endMarkerId|结束标记点|string||
|&emsp;&emsp;startControl|开始点的控制点xy坐标|string||
|&emsp;&emsp;endControl|结束点的控制点xy坐标|string||
|&emsp;&emsp;length|长度|number(double)||
|&emsp;&emsp;lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）|integer(int32)||
|&emsp;&emsp;direction|方向 0、双向 1、正向 2、反向|integer(int32)||
|&emsp;&emsp;forwardAgvDirection|正向行驶时agv方向 1、正向 2、反向|integer(int32)||
|&emsp;&emsp;reverseAgvDirection|反向行驶时agv方向 1、正向 2、反向|integer(int32)||
|&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|&emsp;&emsp;autoDoorId|自动门ID|string||
|modeControlSource|模式控制源  1、软件控制  2、硬件控制|integer(int32)|integer(int32)|
|errorMsgShow|异常信息显示|string||


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"ip": "",
	"agvMapId": "",
	"navigationType": "",
	"connectedTime": "",
	"mapStatus": 0,
	"recordStatus": 0,
	"workStatus": 0,
	"abnormalStatus": 0,
	"connectStatus": 0,
	"manualStatus": 0,
	"controlMode": 0,
	"vehicleInfo": {
		"agv": {
			"agv_id": "",
			"agv_name": "",
			"agv_version": ""
		},
		"device": {
			"imu": "",
			"motor": "",
			"pc": ""
		},
		"network": {
			"net_ip": "",
			"net_mac": "",
			"net_protocol_version": "",
			"net_wifi_rssi": "",
			"net_wifi_ssid": ""
		},
		"shape": {
			"length": 0,
			"radius": 0,
			"width": 0
		}
	},
	"vehicleDeviceInfoList": [
		{
			"id": "",
			"model": "",
			"name": "",
			"property": {},
			"type": ""
		}
	],
	"missionWork": {
		"currentActionName": "",
		"currentActionSequence": 0,
		"id": "",
		"releaseButtonAddress": 0,
		"releaseDeviceAddress": 0,
		"releaseSuccess": true,
		"code": "",
		"missionCallId": "",
		"missionId": "",
		"name": "",
		"schedulePlanId": "",
		"callbackUrl": "",
		"sequence": 0,
		"description": "",
		"status": "",
		"message": "",
		"interrupt": true,
		"runtimeParam": "",
		"missionWorkChainId": "",
		"allocationStatus": "",
		"totalMileage": 0,
		"errorCode": 0,
		"startTime": "",
		"endTime": "",
		"createTime": "",
		"agvCode": "",
		"triggerSelectorId": "",
		"updateTime": "",
		"createdBy": ""
	},
	"defaultVehicleStatus": {
		"agvStatus": {
			"resetting_status": true,
			"unlock_brake_status": true
		},
		"battery": {
			"battery_charge": 0,
			"battery_discharge": 0,
			"battery_fullcapacity": 0,
			"battery_leftcapacity": 0,
			"battery_status": 0,
			"battery_temp": 0,
			"battery_value": 0,
			"battery_voltage": 0
		},
		"deviceStatus": {
			"motorStatus": {
				"left_error": 0,
				"left_status": 0,
				"lift_error": 0,
				"lift_status": 0,
				"right_error": 0,
				"right_status": 0,
				"rotate_error": 0,
				"rotate_status": 0
			}
		},
		"emec": {
			"emc_jam_start_time": 0,
			"emc_reason": [],
			"emc_status": 0
		},
		"fallPrevent": {
			"status": "",
			"switch_": ""
		},
		"lift": {
			"controller_error": 0,
			"emc_stop": 0,
			"goal_reached": 0,
			"limit": 0,
			"origin_point": 0,
			"position": 0,
			"status_word": 0
		},
		"map": {
			"current_feature_id": "",
			"current_map_id": "",
			"current_map_type": 0,
			"scan_feature_status": 0,
			"scan_status": 0,
			"scan_update_status": 0
		},
		"motorStatus": {
			"left_error": 0,
			"left_status": 0,
			"lift_error": 0,
			"lift_status": 0,
			"right_error": 0,
			"right_status": 0,
			"rotate_error": 0,
			"rotate_status": 0
		},
		"position": {
			"covariance": [],
			"pos_angle": 0,
			"pos_confidence": 0,
			"pos_current_station": "",
			"pos_islocated": 0,
			"pos_x": 0,
			"pos_y": 0,
			"segment_id": "",
			"t": 0,
			"update_time_millis": 0
		},
		"runtime": {
			"agv_mode": 0,
			"agv_status": 0,
			"controller_temp": 0,
			"docking_status": 0,
			"follow_status": 0,
			"motor_temp": 0,
			"odom": 0,
			"time": 0,
			"total_time": 0
		},
		"speed": {
			"speed_r_vx": 0,
			"speed_r_vy": 0,
			"speed_r_w": 0,
			"speed_vx": 0,
			"speed_vy": 0,
			"speed_w": 0
		},
		"status": {
			"err_code": [],
			"robot_status": ""
		}
	},
	"errorMessage": "",
	"missionWorkChainId": "",
	"paths": [
		{
			"id": "",
			"agvMapName": "",
			"startMarkerId": "",
			"endMarkerId": "",
			"startControl": "",
			"endControl": "",
			"length": 0,
			"lineType": 0,
			"direction": 0,
			"forwardAgvDirection": 0,
			"reverseAgvDirection": 0,
			"usageStatus": "",
			"autoDoorId": ""
		}
	],
	"modeControlSource": 0,
	"errorMsgShow": ""
}
```


## 机器人位置和角度和规划路径


**接口地址**:`/api/v3/vehicles/getPositionAndSidePaths`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 机器人保养和维护操作记录


## 新增保养和维修记录


**接口地址**:`/api/v3/operationRecord`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"operationType": 0,
	"description": "",
	"operationName": "",
	"operationTime": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|operationRecord|AGV保养和维修记录|body|true|OperationRecord|OperationRecord|
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;operationType|操作类型: 0保养、1维修||false|integer(int32)||
|&emsp;&emsp;description|描述信息||false|string||
|&emsp;&emsp;operationName|操作/保养人员||false|string||
|&emsp;&emsp;operationTime|操作/保养时间||false|string(date-time)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 分页查询


**接口地址**:`/api/v3/operationRecord/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||
|endTime|保养结束时间|query|false|integer(int64)||
|startTime|保养开始时间|query|false|integer(int64)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«OperationRecord»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|OperationRecord|
|&emsp;&emsp;id|id|string||
|&emsp;&emsp;operationType|操作类型: 0保养、1维修|integer(int32)||
|&emsp;&emsp;description|描述信息|string||
|&emsp;&emsp;operationName|操作/保养人员|string||
|&emsp;&emsp;operationTime|操作/保养时间|string(date-time)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"operationType": 0,
			"description": "",
			"operationName": "",
			"operationTime": "",
			"createTime": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 查看单个保养和维修记录


**接口地址**:`/api/v3/operationRecord/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|查看单个保养和维修记录|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|OperationRecord|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|id|string||
|operationType|操作类型: 0保养、1维修|integer(int32)|integer(int32)|
|description|描述信息|string||
|operationName|操作/保养人员|string||
|operationTime|操作/保养时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"operationType": 0,
	"description": "",
	"operationName": "",
	"operationTime": "",
	"createTime": "",
	"updateTime": ""
}
```


## 修改保养和维修记录


**接口地址**:`/api/v3/operationRecord/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|path|true|string||
|operationRecord|修改保养和维修记录|path|true|ref||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 删除保养和维修记录


**接口地址**:`/api/v3/operationRecord/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|删除保养和维修记录|path|true|ref||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 机器人功能配置


## 列表


**接口地址**:`/api/v3/agvFunctionConfigs`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AGVFunctionConfig|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|type|功能类型 SMART_CHARGE:智能充电, SMART_WAIT:智能归位|string||
|parameter|参数(以json的格式存储), \n如果type为SMART_CHARGE, 参数key值有：\n1、isEnable:是否启用 0、启用 1、不启用 值为int类型  \n2、mustChargeBatteryValue:必须充电电量 值为double类型 取值范围(0, 100), \n3、canChargeBatteryValue:可充电电量(与freeTime组合使用，需两者都满足) 值为double类型 取值范围(0, 100),\n4、freeTime:空闲时间(与canChargeBatteryValue组合使用) 值为double类型 [0, +∞)  单位:秒, \n5、chargePlan:充电计划 0:指定时间 1:充满 值为int类型 取值范围[0, 1], \n6、chargeTime:充电时间(当chargePlan==0时生效)  值为int类型 取值范围[0, +∞)  单位:分钟\n7、interruptBatteryValue:可中断电量 值为double类型 取值范围[1, 99], \n8、chargeMode:充电方式 0:对接充电 1:普通充电 值为int类型 取值范围[0, 1], \n9、chargeMarkerId:充电点markerId 置为String类型 通过/api/v2/markers?type=CHARGING_MARKER接口获取下拉列表\n10、retryCount: 失败重试次数 值为int类型 取值范围[0, +∞), \n11、retryInterval: 失败重试间隔 值为int类型 取值范围[0, +∞) 单位:秒 \n12、minChargeTime：最低充电时间\n如果type为SMART_WAIT, 参数key值有：\n1、isEnable:是否启用 0、启用 1、不启用 值为int类型 \n2、freeTime:空闲时间 值为double类型 取值范围[1, +∞) 单位:秒, \n3、waitMarkerId:待机点markerId 值为string类型 通过/api/v2/markers?type=WAIT_MARKER接口获取下拉列表|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"type": "",
		"parameter": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


## 分页查询


**接口地址**:`/api/v3/agvFunctionConfigs/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«AGVFunctionConfig»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|AGVFunctionConfig|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;type|功能类型 SMART_CHARGE:智能充电, SMART_WAIT:智能归位|string||
|&emsp;&emsp;parameter|参数(以json的格式存储), \n如果type为SMART_CHARGE, 参数key值有：\n1、isEnable:是否启用 0、启用 1、不启用 值为int类型  \n2、mustChargeBatteryValue:必须充电电量 值为double类型 取值范围(0, 100), \n3、canChargeBatteryValue:可充电电量(与freeTime组合使用，需两者都满足) 值为double类型 取值范围(0, 100),\n4、freeTime:空闲时间(与canChargeBatteryValue组合使用) 值为double类型 [0, +∞)  单位:秒, \n5、chargePlan:充电计划 0:指定时间 1:充满 值为int类型 取值范围[0, 1], \n6、chargeTime:充电时间(当chargePlan==0时生效)  值为int类型 取值范围[0, +∞)  单位:分钟\n7、interruptBatteryValue:可中断电量 值为double类型 取值范围[1, 99], \n8、chargeMode:充电方式 0:对接充电 1:普通充电 值为int类型 取值范围[0, 1], \n9、chargeMarkerId:充电点markerId 置为String类型 通过/api/v2/markers?type=CHARGING_MARKER接口获取下拉列表\n10、retryCount: 失败重试次数 值为int类型 取值范围[0, +∞), \n11、retryInterval: 失败重试间隔 值为int类型 取值范围[0, +∞) 单位:秒 \n12、minChargeTime：最低充电时间\n如果type为SMART_WAIT, 参数key值有：\n1、isEnable:是否启用 0、启用 1、不启用 值为int类型 \n2、freeTime:空闲时间 值为double类型 取值范围[1, +∞) 单位:秒, \n3、waitMarkerId:待机点markerId 值为string类型 通过/api/v2/markers?type=WAIT_MARKER接口获取下拉列表|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"type": "",
			"parameter": "",
			"createTime": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/agvFunctionConfigs/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|机器人功能配置ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AGVFunctionConfig|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|type|功能类型 SMART_CHARGE:智能充电, SMART_WAIT:智能归位|string||
|parameter|参数(以json的格式存储), \n如果type为SMART_CHARGE, 参数key值有：\n1、isEnable:是否启用 0、启用 1、不启用 值为int类型  \n2、mustChargeBatteryValue:必须充电电量 值为double类型 取值范围(0, 100), \n3、canChargeBatteryValue:可充电电量(与freeTime组合使用，需两者都满足) 值为double类型 取值范围(0, 100),\n4、freeTime:空闲时间(与canChargeBatteryValue组合使用) 值为double类型 [0, +∞)  单位:秒, \n5、chargePlan:充电计划 0:指定时间 1:充满 值为int类型 取值范围[0, 1], \n6、chargeTime:充电时间(当chargePlan==0时生效)  值为int类型 取值范围[0, +∞)  单位:分钟\n7、interruptBatteryValue:可中断电量 值为double类型 取值范围[1, 99], \n8、chargeMode:充电方式 0:对接充电 1:普通充电 值为int类型 取值范围[0, 1], \n9、chargeMarkerId:充电点markerId 置为String类型 通过/api/v2/markers?type=CHARGING_MARKER接口获取下拉列表\n10、retryCount: 失败重试次数 值为int类型 取值范围[0, +∞), \n11、retryInterval: 失败重试间隔 值为int类型 取值范围[0, +∞) 单位:秒 \n12、minChargeTime：最低充电时间\n如果type为SMART_WAIT, 参数key值有：\n1、isEnable:是否启用 0、启用 1、不启用 值为int类型 \n2、freeTime:空闲时间 值为double类型 取值范围[1, +∞) 单位:秒, \n3、waitMarkerId:待机点markerId 值为string类型 通过/api/v2/markers?type=WAIT_MARKER接口获取下拉列表|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"type": "",
	"parameter": "",
	"createTime": "",
	"updateTime": ""
}
```


## 更新


**接口地址**:`/api/v3/agvFunctionConfigs/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:根据ID更新机器人功能配置信息


**请求示例**:


```javascript
{
	"id": "",
	"type": "",
	"parameter": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|agvFunctionConfig|AGV功能配置|body|true|AGVFunctionConfig|AGVFunctionConfig|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;type|功能类型 SMART_CHARGE:智能充电, SMART_WAIT:智能归位||false|string||
|&emsp;&emsp;parameter|参数(以json的格式存储), \n如果type为SMART_CHARGE, 参数key值有：\n1、isEnable:是否启用 0、启用 1、不启用 值为int类型  \n2、mustChargeBatteryValue:必须充电电量 值为double类型 取值范围(0, 100), \n3、canChargeBatteryValue:可充电电量(与freeTime组合使用，需两者都满足) 值为double类型 取值范围(0, 100),\n4、freeTime:空闲时间(与canChargeBatteryValue组合使用) 值为double类型 [0, +∞)  单位:秒, \n5、chargePlan:充电计划 0:指定时间 1:充满 值为int类型 取值范围[0, 1], \n6、chargeTime:充电时间(当chargePlan==0时生效)  值为int类型 取值范围[0, +∞)  单位:分钟\n7、interruptBatteryValue:可中断电量 值为double类型 取值范围[1, 99], \n8、chargeMode:充电方式 0:对接充电 1:普通充电 值为int类型 取值范围[0, 1], \n9、chargeMarkerId:充电点markerId 置为String类型 通过/api/v2/markers?type=CHARGING_MARKER接口获取下拉列表\n10、retryCount: 失败重试次数 值为int类型 取值范围[0, +∞), \n11、retryInterval: 失败重试间隔 值为int类型 取值范围[0, +∞) 单位:秒 \n12、minChargeTime：最低充电时间\n如果type为SMART_WAIT, 参数key值有：\n1、isEnable:是否启用 0、启用 1、不启用 值为int类型 \n2、freeTime:空闲时间 值为double类型 取值范围[1, +∞) 单位:秒, \n3、waitMarkerId:待机点markerId 值为string类型 通过/api/v2/markers?type=WAIT_MARKER接口获取下拉列表||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|id|机器人功能配置ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AGVFunctionConfig|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|type|功能类型 SMART_CHARGE:智能充电, SMART_WAIT:智能归位|string||
|parameter|参数(以json的格式存储), \n如果type为SMART_CHARGE, 参数key值有：\n1、isEnable:是否启用 0、启用 1、不启用 值为int类型  \n2、mustChargeBatteryValue:必须充电电量 值为double类型 取值范围(0, 100), \n3、canChargeBatteryValue:可充电电量(与freeTime组合使用，需两者都满足) 值为double类型 取值范围(0, 100),\n4、freeTime:空闲时间(与canChargeBatteryValue组合使用) 值为double类型 [0, +∞)  单位:秒, \n5、chargePlan:充电计划 0:指定时间 1:充满 值为int类型 取值范围[0, 1], \n6、chargeTime:充电时间(当chargePlan==0时生效)  值为int类型 取值范围[0, +∞)  单位:分钟\n7、interruptBatteryValue:可中断电量 值为double类型 取值范围[1, 99], \n8、chargeMode:充电方式 0:对接充电 1:普通充电 值为int类型 取值范围[0, 1], \n9、chargeMarkerId:充电点markerId 置为String类型 通过/api/v2/markers?type=CHARGING_MARKER接口获取下拉列表\n10、retryCount: 失败重试次数 值为int类型 取值范围[0, +∞), \n11、retryInterval: 失败重试间隔 值为int类型 取值范围[0, +∞) 单位:秒 \n12、minChargeTime：最低充电时间\n如果type为SMART_WAIT, 参数key值有：\n1、isEnable:是否启用 0、启用 1、不启用 值为int类型 \n2、freeTime:空闲时间 值为double类型 取值范围[1, +∞) 单位:秒, \n3、waitMarkerId:待机点markerId 值为string类型 通过/api/v2/markers?type=WAIT_MARKER接口获取下拉列表|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"type": "",
	"parameter": "",
	"createTime": "",
	"updateTime": ""
}
```


# 机器人动作、任务


## 继续执行任务


**接口地址**:`/api/v3/vehicles/task/missionWork/continue`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 路径导航到指定标记点


**接口地址**:`/api/v3/vehicles/task/moveToMarker`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"markerId": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param|移动到指定标记点参数|body|true|MoveToMarkerParam|MoveToMarkerParam|
|&emsp;&emsp;markerId|位置ID||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 自由导航到指定坐标


**接口地址**:`/api/v3/vehicles/task/moveToPosition`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"goal_rad": 0,
	"goal_x": 0,
	"goal_y": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param|移动到指定位置参数|body|true|MoveToPositionParam|MoveToPositionParam|
|&emsp;&emsp;goal_rad|目标弧度||false|number(double)||
|&emsp;&emsp;goal_x|目标x坐标||false|number(double)||
|&emsp;&emsp;goal_y|目标y坐标||false|number(double)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## AGV一键重置(清错充电异常、归位异常、工作异常)


**接口地址**:`/api/v3/vehicles/task/oneKeyReset`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## AGV一键恢复(充电异常恢复、归位异常恢复、任务异常恢复)


**接口地址**:`/api/v3/vehicles/task/oneKeyResume`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## AGV一键停止(停止充电动作、归位动作、任务工作)


**接口地址**:`/api/v3/vehicles/task/oneKeyStop`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## AGV重启


**接口地址**:`/api/v3/vehicles/task/reboot`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## Vehicle开始充电


**接口地址**:`/api/v3/vehicles/task/startCharge`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## Vehicle停止充电


**接口地址**:`/api/v3/vehicles/task/stopCharge`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 机器人地图操作


## 录制初始位置


**接口地址**:`/api/v3/vehicles/maps/markers/homes`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle在激光地图中录制初始位置


**请求示例**:


```javascript
{
	"agvMapId": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param|录制初始点参数|body|true|RecordHomeMarkerParam|RecordHomeMarkerParam|
|&emsp;&emsp;agvMapId|地图ID||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Marker|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|code|编码|string||
|x|x坐标|number(double)|number(double)|
|y|y坐标|number(double)|number(double)|
|agvMapName|地图名称|string||
|angle|角度|number(double)|number(double)|
|type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点|string||
|covariance|协方差矩阵|string||
|usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|dockingPoint|对接点|DockingPoint|DockingPoint|
|&emsp;&emsp;qrDockId|地面二维码坐标ID|integer(int32)||
|&emsp;&emsp;relativeX|相对x坐标|number(double)||
|&emsp;&emsp;relativeY|相对y坐标|number(double)||
|&emsp;&emsp;relativeAngle|相对角度|number(double)||
|&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点|string||
|&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接|integer(int32)||
|&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否|integer(int32)||
|isPark|是否可泊车, 0:不可泊车，1：可泊车|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"id": "",
	"code": "",
	"x": 0,
	"y": 0,
	"agvMapName": "",
	"angle": 0,
	"type": "",
	"covariance": "",
	"usageStatus": "",
	"dockingPoint": {
		"qrDockId": 0,
		"relativeX": 0,
		"relativeY": 0,
		"relativeAngle": 0,
		"type": "",
		"direction": 0,
		"isChargeStation": 0
	},
	"isPark": 0
}
```


## 录制地图


**接口地址**:`/api/v3/vehicles/maps/record/start`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle录制激光地图/特征地图


**请求示例**:


```javascript
{
	"agvMapId": "",
	"mapType": 0,
	"recordMode": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param|录制地图参数|body|true|RecordingMapParam|RecordingMapParam|
|&emsp;&emsp;agvMapId|地图ID||false|string||
|&emsp;&emsp;mapType|地图类型 1、栅格地图 2、二维码地图 3、特征地图||false|integer(int32)||
|&emsp;&emsp;recordMode|录制方式 1、重新录制||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 停止录制地图


**接口地址**:`/api/v3/vehicles/maps/record/stop`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle停止录制激光地图


**请求示例**:


```javascript
{
	"is_save": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param|停止录制地图参数|body|true|StopRecordingParam|StopRecordingParam|
|&emsp;&emsp;is_save|是否保存地图 1、保存  0、不保存||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 自动重定位


**接口地址**:`/api/v3/vehicles/maps/relocation/auto`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle自动重定位


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 初始点重定位


**接口地址**:`/api/v3/vehicles/maps/relocation/home`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle初始点重定位


**请求示例**:


```javascript
{
	"agvMapName": "",
	"markerId": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param|AGV初始点重定位参数|body|true|HomeRelocationParam|HomeRelocationParam|
|&emsp;&emsp;agvMapName|地图名称||false|string||
|&emsp;&emsp;markerId|标记点(初始点)ID||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 手动重定位


**接口地址**:`/api/v3/vehicles/maps/relocation/manual`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle手动重定位


**请求示例**:


```javascript
{
	"init_angle": 0,
	"init_x": 0,
	"init_y": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param|AGV手动重定位参数|body|true|ManualRelocationParam|ManualRelocationParam|
|&emsp;&emsp;init_angle|初始化角度, 单位rad||false|number(double)||
|&emsp;&emsp;init_x|初始化X坐标, 单位m||false|number(double)||
|&emsp;&emsp;init_y|初始化Y坐标, 单位m||false|number(double)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 指定地图


**接口地址**:`/api/v3/vehicles/maps/syncCurrentMapId`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle指定地图


**请求示例**:


```javascript
{
	"agvMapId": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|currentMapParam|指定地图参数|body|true|CurrentMapParam|CurrentMapParam|
|&emsp;&emsp;agvMapId|地图ID||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 机器人控制模式


## 切换为自动控制模式


**接口地址**:`/api/v3/vehicles/controls/autoMode`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 切换为手工控制模式


**接口地址**:`/api/v3/vehicles/controls/manualMode`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 强制切换为手工控制模式。会强制停止任务、充电、归位和录制地图等动作


**接口地址**:`/api/v3/vehicles/controls/manualMode/force`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 机器人统计


## 统计系统总数据


**接口地址**:`/api/v3/statistics`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`*/*`


**接口描述**:统计系统总数据


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|dataType|数据类型：天:1，周:7，月:30，所有:0||true|integer||
|endTime|结束时间||false|integer||
|searchMap|searchMap|query|false||object|
|startTime|开始时间||false|integer||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AGVStatistics|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|workTime|工作时间 单位：秒|integer(int64)|integer(int64)|
|freeTime|空闲时间 单位：秒|integer(int64)|integer(int64)|
|onTime|总在线时间 单位：秒|integer(int64)|integer(int64)|
|missionCount|总任务数|integer(int32)|integer(int32)|
|missionFinishCount|已完成任务数|integer(int32)|integer(int32)|
|missionCancelCount|取消任务数|integer(int32)|integer(int32)|
|chargeCount|充电总次数|integer(int32)|integer(int32)|
|chargeTime|充电总时间 单位：秒|integer(int64)|integer(int64)|
|dataType|数据类型： 1:day,7:week,30:month,0:all|integer(int32)|integer(int32)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|
|belongTime|数据归属时间（年月日），日：当前日期；周：当前周最后一天，月：当前月最后一天；所有：空字符串|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"id": "",
	"workTime": 0,
	"freeTime": 0,
	"onTime": 0,
	"missionCount": 0,
	"missionFinishCount": 0,
	"missionCancelCount": 0,
	"chargeCount": 0,
	"chargeTime": 0,
	"dataType": 0,
	"createTime": "",
	"updateTime": "",
	"belongTime": 0
}
```


# 机器人设备控制


## 查询摄像头参数


**接口地址**:`/api/v3/vehicles/devices/camera/param`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:vehicle查询摄像头参数


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|CameraSettingParam|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|osd_str|OSD字符叠加(图片水印)|string||
|pBrightValue|亮度指针,取值范围[1,10]|integer(int32)|integer(int32)|
|pContrastValue|对比度指针,取值范围[1,10]|integer(int32)|integer(int32)|
|pSaturationValue|饱和度指针,取值范围[1,10]|integer(int32)|integer(int32)|
|byExposureModeSet|球机的曝光模式：0-手动模式，1-自动曝光，2-光圈优先，3-快门优先，4-增益优先|integer(int32)|integer(int32)|
|byShutterSet|快门等级：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230|integer(int32)|integer(int32)|
|byMaxShutterSet|最大快门值：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230(在自动曝光模式下生效)|integer(int32)|integer(int32)|
|byMinShutterSet|最小快门值：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230(在自动曝光模式下生效)|integer(int32)|integer(int32)|
|byMaxIrisSet|最大光圈限制值(在自动曝光模式下生效)，取值范围：[0,100]|integer(int32)|integer(int32)|
|byMinIrisSet|最小光圈限制值(在自动曝光模式下生效)，取值范围：[0,100]|integer(int32)|integer(int32)|
|byFocusMode|聚焦模式：0-自动，1-手动，2-半自动|integer(int32)|integer(int32)|
|wZoomPos|Z参数（变倍参数）|integer(int32)|integer(int32)|
|iIrisSet|光圈，为实际取值*100的值，0表示关闭光圈|integer(int32)|integer(int32)|
|xmlFocus|可见光单目摄像头调整焦距|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"osd_str": "",
	"pBrightValue": 0,
	"pContrastValue": 0,
	"pSaturationValue": 0,
	"byExposureModeSet": 0,
	"byShutterSet": 0,
	"byMaxShutterSet": 0,
	"byMinShutterSet": 0,
	"byMaxIrisSet": 0,
	"byMinIrisSet": 0,
	"byFocusMode": 0,
	"wZoomPos": 0,
	"iIrisSet": 0,
	"xmlFocus": 0
}
```


## 摄像头设置参数


**接口地址**:`/api/v3/vehicles/devices/camera/param`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle摄像头设置参数


**请求示例**:


```javascript
{
	"osd_str": "",
	"pBrightValue": 0,
	"pContrastValue": 0,
	"pSaturationValue": 0,
	"byExposureModeSet": 0,
	"byShutterSet": 0,
	"byMaxShutterSet": 0,
	"byMinShutterSet": 0,
	"byMaxIrisSet": 0,
	"byMinIrisSet": 0,
	"byFocusMode": 0,
	"wZoomPos": 0,
	"iIrisSet": 0,
	"xmlFocus": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param|摄像头设置参数|body|true|CameraSettingParam|CameraSettingParam|
|&emsp;&emsp;osd_str|OSD字符叠加(图片水印)||false|string||
|&emsp;&emsp;pBrightValue|亮度指针,取值范围[1,10]||false|integer(int32)||
|&emsp;&emsp;pContrastValue|对比度指针,取值范围[1,10]||false|integer(int32)||
|&emsp;&emsp;pSaturationValue|饱和度指针,取值范围[1,10]||false|integer(int32)||
|&emsp;&emsp;byExposureModeSet|球机的曝光模式：0-手动模式，1-自动曝光，2-光圈优先，3-快门优先，4-增益优先||false|integer(int32)||
|&emsp;&emsp;byShutterSet|快门等级：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230||false|integer(int32)||
|&emsp;&emsp;byMaxShutterSet|最大快门值：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230(在自动曝光模式下生效)||false|integer(int32)||
|&emsp;&emsp;byMinShutterSet|最小快门值：0-关，1-自动x1，2-自动x2，3-自动x4，4-自动x8，5-自动x16，6-自动x32，7-自动x64，8-自动x128，9-1/1，10-1/2，11-1/3，12-1/4，13-1/6，14-1/8，15-1/12，16-1/15，17-1/25，18-1/30，19-1/50，20-1/60，21-1/75，22-1/90，23-1/100，24-1/120，25-1/125，26-1/150，27-1/180，28-1/200，29-1/215，30-1/250，31-1/300，32-1/350，33-1/425，34-1/500，35-1/600，36-1/725，37-1/1000，38-1/1250，39-1500,40-1/1750，41-1/2000，42-1/2500，43-3000,44-1/3500，45-1/4000，46-1/6000，47-1/10000，48-1/30000，49-1/100000，50-1/175，51-1/195，52-1/225，53-1/230(在自动曝光模式下生效)||false|integer(int32)||
|&emsp;&emsp;byMaxIrisSet|最大光圈限制值(在自动曝光模式下生效)，取值范围：[0,100]||false|integer(int32)||
|&emsp;&emsp;byMinIrisSet|最小光圈限制值(在自动曝光模式下生效)，取值范围：[0,100]||false|integer(int32)||
|&emsp;&emsp;byFocusMode|聚焦模式：0-自动，1-手动，2-半自动||false|integer(int32)||
|&emsp;&emsp;wZoomPos|Z参数（变倍参数）||false|integer(int32)||
|&emsp;&emsp;iIrisSet|光圈，为实际取值*100的值，0表示关闭光圈||false|integer(int32)||
|&emsp;&emsp;xmlFocus|可见光单目摄像头调整焦距||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 摄像头拍照


**接口地址**:`/api/v3/vehicles/devices/camera/photograph`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle摄像头拍照


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|CameraPhotographResult|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|imageBase64|图片的base64编码|string||


**响应示例**:
```javascript
{
	"imageBase64": ""
}
```


## 摄像头预置点设置


**接口地址**:`/api/v3/vehicles/devices/camera/presetPoint`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle摄像头预置点设置


**请求示例**:


```javascript
{
	"dwPTZPresetCmd": 0,
	"dwPresetIndex": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param|摄像头预置点参数设置|body|true|CameraPresetPointParam|CameraPresetPointParam|
|&emsp;&emsp;dwPTZPresetCmd|8:设置点  9:删除点  10:调用点||false|integer(int32)||
|&emsp;&emsp;dwPresetIndex|预置点的ID，最大支持300个点||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## AGV手动充电


**接口地址**:`/api/v3/vehicles/devices/charge`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 取消AMR电机软急停


**接口地址**:`/api/v3/vehicles/devices/emergencyStop/close`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle取消AMR电机软急停


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 开启AMR电机软急停


**接口地址**:`/api/v3/vehicles/devices/emergencyStop/open`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle开启AMR电机软急停


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 补光灯控制


**接口地址**:`/api/v3/vehicles/devices/fillLightControl`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle补光灯控制


**请求示例**:


```javascript
{
	"operation": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param|控制补光灯参数|body|true|FillLightControlParam|FillLightControlParam|
|&emsp;&emsp;operation|操作  1、打开  0、关闭||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 气体检测


**接口地址**:`/api/v3/vehicles/devices/gas/detection`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:vehicle传感器气体检测


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|GasDetectionResult|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|gas||array|GasDetail|
|&emsp;&emsp;concentration|浓度|number(double)||
|&emsp;&emsp;name|气体名称|string||
|&emsp;&emsp;status|气体状态 0、正常  1、过低报警  2、过高报警  4、通讯错误  6、传感器错误|integer(int32)||
|&emsp;&emsp;unit|气体单位 LEL VOL PPM PPB|string||


**响应示例**:
```javascript
{
	"gas": [
		{
			"concentration": 0,
			"name": "",
			"status": 0,
			"unit": ""
		}
	]
}
```


## 读取温湿度


**接口地址**:`/api/v3/vehicles/devices/humiture/read`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:vehicle读取温湿度


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|HumitureReadResult|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|hum|湿度 单位：%RH|number(double)|number(double)|
|temp|温度 单位：℃|number(double)|number(double)|


**响应示例**:
```javascript
{
	"hum": 0,
	"temp": 0
}
```


## 升降平台控制


**接口地址**:`/api/v3/vehicles/devices/liftingPlatform/control`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle的升降平台控制


**请求示例**:


```javascript
{
	"rpm": 0,
	"target_ticks": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param|升降平台控制参数|body|true|LiftingPlatformParam|LiftingPlatformParam|
|&emsp;&emsp;rpm|梯形速度  单位：r/min||false|integer(int32)||
|&emsp;&emsp;target_ticks|目标位置  范围[0, 1000]||false|integer(int64)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 机械臂控制


**接口地址**:`/api/v3/vehicles/devices/manipulatorArm/control`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle机械臂控制


**请求示例**:


```javascript
{
	"joints1": 0,
	"joints2": 0,
	"joints3": 0,
	"joints4": 0,
	"joints5": 0,
	"joints6": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param|机械臂控制参数|body|true|ManipulatorArmControlParam|ManipulatorArmControlParam|
|&emsp;&emsp;joints1|第一个关节角度||false|number(double)||
|&emsp;&emsp;joints2|第二个关节角度||false|number(double)||
|&emsp;&emsp;joints3|第三个关节角度||false|number(double)||
|&emsp;&emsp;joints4|第四个关节角度||false|number(double)||
|&emsp;&emsp;joints5|第五个关节角度||false|number(double)||
|&emsp;&emsp;joints6|第六个关节角度||false|number(double)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 机械臂示教控制


**接口地址**:`/api/v3/vehicles/devices/manipulatorArm/demoControl`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle机械臂示教控制


**请求示例**:


```javascript
{
	"direction": 0,
	"mode": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param|机械臂控制参数|body|true|ManipulatorArmDemoControlParam|ManipulatorArmDemoControlParam|
|&emsp;&emsp;direction|方向 1、正方向 0、反方向||false|integer(int32)||
|&emsp;&emsp;mode|模式 可填参数：六个关节角度(JOINT1 JOINT2 JOINT3 JOINT4 JOINT5 JOINT6) 移动xyz方向(MOV_X MOV_Y MOV_Z) 旋转xyz方向(ROT_X ROT_Y ROT_Z) 停止示教(CLOSE)||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 机械臂登录(清错)


**接口地址**:`/api/v3/vehicles/devices/manipulatorArm/login`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle机械臂登录(清错)


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 读取噪音


**接口地址**:`/api/v3/vehicles/devices/noise/read`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:vehicle读取噪音


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|NoiseReadResult|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|decibel|DB 环境噪音分贝数|number(double)|number(double)|


**响应示例**:
```javascript
{
	"decibel": 0
}
```


## 云台控制


**接口地址**:`/api/v3/vehicles/devices/ptz/control`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle的云台控制


**请求示例**:


```javascript
{
	"fPan": 0,
	"fTilt": 0,
	"fZoom": 0,
	"fHorizontalSpeed": 0,
	"fVerticalSpeed": 0,
	"wAction": 0,
	"wPanPos": 0,
	"wTiltPos": 0,
	"wZoomPos": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param|云台控制参数|body|true|PTZControlParam|PTZControlParam|
|&emsp;&emsp;fPan|云台P参数（水平参数） 取值范围:[0,360.0]||false|number(double)||
|&emsp;&emsp;fTilt|云台T参数（垂直参数） 取值范围:[-90.0,270.0]||false|number(double)||
|&emsp;&emsp;fZoom|云台Z参数（变倍参数） 取值范围:[0.0,100000.0]||false|number(double)||
|&emsp;&emsp;fHorizontalSpeed|水平转动速度 范围:[0.01,1000.00]  单位：度/S||false|number(double)||
|&emsp;&emsp;fVerticalSpeed|垂直转动速度 范围:[0.01,1000.00]  单位：度/S||false|number(double)||
|&emsp;&emsp;wAction|操作类型，仅在设置时有效。1-定位 PTZ 参数，2-定位 P 参数，3-定位 T 参数，4-定位 Z 参数，5-定位 PT 参数||false|integer(int32)||
|&emsp;&emsp;wPanPos|P参数（水平参数）||false|integer(int32)||
|&emsp;&emsp;wTiltPos|T参数（垂直参数）||false|integer(int32)||
|&emsp;&emsp;wZoomPos|Z参数（变倍参数）||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 查询云台参数


**接口地址**:`/api/v3/vehicles/devices/ptz/param`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:vehicle查询云台参数


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PTZControlParam|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|fPan|云台P参数（水平参数） 取值范围:[0,360.0]|number(double)|number(double)|
|fTilt|云台T参数（垂直参数） 取值范围:[-90.0,270.0]|number(double)|number(double)|
|fZoom|云台Z参数（变倍参数） 取值范围:[0.0,100000.0]|number(double)|number(double)|
|fHorizontalSpeed|水平转动速度 范围:[0.01,1000.00]  单位：度/S|number(double)|number(double)|
|fVerticalSpeed|垂直转动速度 范围:[0.01,1000.00]  单位：度/S|number(double)|number(double)|
|wAction|操作类型，仅在设置时有效。1-定位 PTZ 参数，2-定位 P 参数，3-定位 T 参数，4-定位 Z 参数，5-定位 PT 参数|integer(int32)|integer(int32)|
|wPanPos|P参数（水平参数）|integer(int32)|integer(int32)|
|wTiltPos|T参数（垂直参数）|integer(int32)|integer(int32)|
|wZoomPos|Z参数（变倍参数）|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"fPan": 0,
	"fTilt": 0,
	"fZoom": 0,
	"fHorizontalSpeed": 0,
	"fVerticalSpeed": 0,
	"wAction": 0,
	"wPanPos": 0,
	"wTiltPos": 0,
	"wZoomPos": 0
}
```


## 货架随动控制


**接口地址**:`/api/v3/vehicles/devices/shelf/follow`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle货架随动控制


**请求示例**:


```javascript
{
	"id": "",
	"operation": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param|货架随动控制参数|body|true|ShelfFollowControlParam|ShelfFollowControlParam|
|&emsp;&emsp;id|执行动作的ID||false|string||
|&emsp;&emsp;operation|操作 0、关闭随动  1、打开随动||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 解除碰撞(短暂)急停


**接口地址**:`/api/v3/vehicles/devices/shortStopRecovery`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:vehicle解除碰撞(短暂)急停


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 六氟化硫浓度检测


**接口地址**:`/api/v3/vehicles/devices/sixSulfurFluoride/detection`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:vehicle六氟化硫浓度检测


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|SixSulfurFluorideResult|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|concentration|浓度 单位:PPM|number(double)|number(double)|


**响应示例**:
```javascript
{
	"concentration": 0
}
```


# 机器人配置信息


## 查询机器人配置列表


**接口地址**:`/api/v3/vehicles/configs`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:根据机器人的ID获取机器人配置列表


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 更新Vehicle配置列表


**接口地址**:`/api/v3/vehicles/configs`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|dataJson|dataJson|body|true|||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 机械臂预置参数


## 列表


**接口地址**:`/api/v3/manipulatorArmPresetParams`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|ManipulatorArmPresetParam|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|joints1|第一个关节角度|number(double)|number(double)|
|joints2|第二个关节角度|number(double)|number(double)|
|joints3|第三个关节角度|number(double)|number(double)|
|joints4|第四个关节角度|number(double)|number(double)|
|joints5|第五个关节角度|number(double)|number(double)|
|joints6|第六个关节角度|number(double)|number(double)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"name": "",
		"joints1": 0,
		"joints2": 0,
		"joints3": 0,
		"joints4": 0,
		"joints5": 0,
		"joints6": 0,
		"createTime": "",
		"updateTime": ""
	}
]
```


## 创建


**接口地址**:`/api/v3/manipulatorArmPresetParams`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"name": "",
	"joints1": 0,
	"joints2": 0,
	"joints3": 0,
	"joints4": 0,
	"joints5": 0,
	"joints6": 0,
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|manipulatorArmPresetParam|机械臂预置参数|body|true|ManipulatorArmPresetParam|ManipulatorArmPresetParam|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;joints1|第一个关节角度||false|number(double)||
|&emsp;&emsp;joints2|第二个关节角度||false|number(double)||
|&emsp;&emsp;joints3|第三个关节角度||false|number(double)||
|&emsp;&emsp;joints4|第四个关节角度||false|number(double)||
|&emsp;&emsp;joints5|第五个关节角度||false|number(double)||
|&emsp;&emsp;joints6|第六个关节角度||false|number(double)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|ManipulatorArmPresetParam|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|joints1|第一个关节角度|number(double)|number(double)|
|joints2|第二个关节角度|number(double)|number(double)|
|joints3|第三个关节角度|number(double)|number(double)|
|joints4|第四个关节角度|number(double)|number(double)|
|joints5|第五个关节角度|number(double)|number(double)|
|joints6|第六个关节角度|number(double)|number(double)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"joints1": 0,
	"joints2": 0,
	"joints3": 0,
	"joints4": 0,
	"joints5": 0,
	"joints6": 0,
	"createTime": "",
	"updateTime": ""
}
```


## 分页查询


**接口地址**:`/api/v3/manipulatorArmPresetParams/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«ManipulatorArmPresetParam»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|ManipulatorArmPresetParam|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;joints1|第一个关节角度|number(double)||
|&emsp;&emsp;joints2|第二个关节角度|number(double)||
|&emsp;&emsp;joints3|第三个关节角度|number(double)||
|&emsp;&emsp;joints4|第四个关节角度|number(double)||
|&emsp;&emsp;joints5|第五个关节角度|number(double)||
|&emsp;&emsp;joints6|第六个关节角度|number(double)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"name": "",
			"joints1": 0,
			"joints2": 0,
			"joints3": 0,
			"joints4": 0,
			"joints5": 0,
			"joints6": 0,
			"createTime": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/manipulatorArmPresetParams/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|机械臂预置参数ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|ManipulatorArmPresetParam|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|joints1|第一个关节角度|number(double)|number(double)|
|joints2|第二个关节角度|number(double)|number(double)|
|joints3|第三个关节角度|number(double)|number(double)|
|joints4|第四个关节角度|number(double)|number(double)|
|joints5|第五个关节角度|number(double)|number(double)|
|joints6|第六个关节角度|number(double)|number(double)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"joints1": 0,
	"joints2": 0,
	"joints3": 0,
	"joints4": 0,
	"joints5": 0,
	"joints6": 0,
	"createTime": "",
	"updateTime": ""
}
```


## 更新


**接口地址**:`/api/v3/manipulatorArmPresetParams/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"name": "",
	"joints1": 0,
	"joints2": 0,
	"joints3": 0,
	"joints4": 0,
	"joints5": 0,
	"joints6": 0,
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|机械臂预置参数ID|path|true|string||
|manipulatorArmPresetParam|机械臂预置参数|body|true|ManipulatorArmPresetParam|ManipulatorArmPresetParam|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;joints1|第一个关节角度||false|number(double)||
|&emsp;&emsp;joints2|第二个关节角度||false|number(double)||
|&emsp;&emsp;joints3|第三个关节角度||false|number(double)||
|&emsp;&emsp;joints4|第四个关节角度||false|number(double)||
|&emsp;&emsp;joints5|第五个关节角度||false|number(double)||
|&emsp;&emsp;joints6|第六个关节角度||false|number(double)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|ManipulatorArmPresetParam|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|joints1|第一个关节角度|number(double)|number(double)|
|joints2|第二个关节角度|number(double)|number(double)|
|joints3|第三个关节角度|number(double)|number(double)|
|joints4|第四个关节角度|number(double)|number(double)|
|joints5|第五个关节角度|number(double)|number(double)|
|joints6|第六个关节角度|number(double)|number(double)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"joints1": 0,
	"joints2": 0,
	"joints3": 0,
	"joints4": 0,
	"joints5": 0,
	"joints6": 0,
	"createTime": "",
	"updateTime": ""
}
```


## 删除


**接口地址**:`/api/v3/manipulatorArmPresetParams/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|机械臂预置参数ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 查询MOS物料信息状态


## 查询物料信息


**接口地址**:`/api/v3/robotCoach/getRobotCoachInfo`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 标记点


## 列表


**接口地址**:`/api/v3/markers`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|agvMapName|标记点ID|query|true|string||
|isDraft|是否查询草稿文件数据|query|true|boolean||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Marker|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|code|编码|string||
|x|x坐标|number(double)|number(double)|
|y|y坐标|number(double)|number(double)|
|agvMapName|地图名称|string||
|angle|角度|number(double)|number(double)|
|type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点|string||
|covariance|协方差矩阵|string||
|usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|dockingPoint|对接点|DockingPoint|DockingPoint|
|&emsp;&emsp;qrDockId|地面二维码坐标ID|integer(int32)||
|&emsp;&emsp;relativeX|相对x坐标|number(double)||
|&emsp;&emsp;relativeY|相对y坐标|number(double)||
|&emsp;&emsp;relativeAngle|相对角度|number(double)||
|&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点|string||
|&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接|integer(int32)||
|&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否|integer(int32)||
|isPark|是否可泊车, 0:不可泊车，1：可泊车|integer(int32)|integer(int32)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"code": "",
		"x": 0,
		"y": 0,
		"agvMapName": "",
		"angle": 0,
		"type": "",
		"covariance": "",
		"usageStatus": "",
		"dockingPoint": {
			"qrDockId": 0,
			"relativeX": 0,
			"relativeY": 0,
			"relativeAngle": 0,
			"type": "",
			"direction": 0,
			"isChargeStation": 0
		},
		"isPark": 0
	}
]
```


## 创建


**接口地址**:`/api/v3/markers`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"code": "",
	"x": 0,
	"y": 0,
	"agvMapName": "",
	"angle": 0,
	"type": "",
	"covariance": "",
	"usageStatus": "",
	"dockingPoint": {
		"qrDockId": 0,
		"relativeX": 0,
		"relativeY": 0,
		"relativeAngle": 0,
		"type": "",
		"direction": 0,
		"isChargeStation": 0
	},
	"isPark": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|marker|标记点|body|true|Marker|Marker|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;code|编码||false|string||
|&emsp;&emsp;x|x坐标||false|number(double)||
|&emsp;&emsp;y|y坐标||false|number(double)||
|&emsp;&emsp;agvMapName|地图名称||false|string||
|&emsp;&emsp;angle|角度||false|number(double)||
|&emsp;&emsp;type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点||false|string||
|&emsp;&emsp;covariance|协方差矩阵||false|string||
|&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;dockingPoint|对接点||false|DockingPoint|DockingPoint|
|&emsp;&emsp;&emsp;&emsp;qrDockId|地面二维码坐标ID||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;relativeX|相对x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;relativeY|相对y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;relativeAngle|相对角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点||false|string||
|&emsp;&emsp;&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否||false|integer(int32)||
|&emsp;&emsp;isPark|是否可泊车, 0:不可泊车，1：可泊车||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|Marker|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|code|编码|string||
|x|x坐标|number(double)|number(double)|
|y|y坐标|number(double)|number(double)|
|agvMapName|地图名称|string||
|angle|角度|number(double)|number(double)|
|type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点|string||
|covariance|协方差矩阵|string||
|usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|dockingPoint|对接点|DockingPoint|DockingPoint|
|&emsp;&emsp;qrDockId|地面二维码坐标ID|integer(int32)||
|&emsp;&emsp;relativeX|相对x坐标|number(double)||
|&emsp;&emsp;relativeY|相对y坐标|number(double)||
|&emsp;&emsp;relativeAngle|相对角度|number(double)||
|&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点|string||
|&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接|integer(int32)||
|&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否|integer(int32)||
|isPark|是否可泊车, 0:不可泊车，1：可泊车|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"id": "",
	"code": "",
	"x": 0,
	"y": 0,
	"agvMapName": "",
	"angle": 0,
	"type": "",
	"covariance": "",
	"usageStatus": "",
	"dockingPoint": {
		"qrDockId": 0,
		"relativeX": 0,
		"relativeY": 0,
		"relativeAngle": 0,
		"type": "",
		"direction": 0,
		"isChargeStation": 0
	},
	"isPark": 0
}
```


## 详情


**接口地址**:`/api/v3/markers/{agvMapName}/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|agvMapName|标记点ID|path|true|string||
|id|标记点ID|path|true|string||
|isDraft|是否查询草稿文件数据|query|true|boolean||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Marker|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|code|编码|string||
|x|x坐标|number(double)|number(double)|
|y|y坐标|number(double)|number(double)|
|agvMapName|地图名称|string||
|angle|角度|number(double)|number(double)|
|type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点|string||
|covariance|协方差矩阵|string||
|usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|dockingPoint|对接点|DockingPoint|DockingPoint|
|&emsp;&emsp;qrDockId|地面二维码坐标ID|integer(int32)||
|&emsp;&emsp;relativeX|相对x坐标|number(double)||
|&emsp;&emsp;relativeY|相对y坐标|number(double)||
|&emsp;&emsp;relativeAngle|相对角度|number(double)||
|&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点|string||
|&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接|integer(int32)||
|&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否|integer(int32)||
|isPark|是否可泊车, 0:不可泊车，1：可泊车|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"id": "",
	"code": "",
	"x": 0,
	"y": 0,
	"agvMapName": "",
	"angle": 0,
	"type": "",
	"covariance": "",
	"usageStatus": "",
	"dockingPoint": {
		"qrDockId": 0,
		"relativeX": 0,
		"relativeY": 0,
		"relativeAngle": 0,
		"type": "",
		"direction": 0,
		"isChargeStation": 0
	},
	"isPark": 0
}
```


## 删除


**接口地址**:`/api/v3/markers/{agvMapName}/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|agvMapName|标记点ID|path|true|string||
|id|标记点ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 更新


**接口地址**:`/api/v3/markers/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"code": "",
	"x": 0,
	"y": 0,
	"agvMapName": "",
	"angle": 0,
	"type": "",
	"covariance": "",
	"usageStatus": "",
	"dockingPoint": {
		"qrDockId": 0,
		"relativeX": 0,
		"relativeY": 0,
		"relativeAngle": 0,
		"type": "",
		"direction": 0,
		"isChargeStation": 0
	},
	"isPark": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|标记点ID|path|true|string||
|marker|标记点|body|true|Marker|Marker|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;code|编码||false|string||
|&emsp;&emsp;x|x坐标||false|number(double)||
|&emsp;&emsp;y|y坐标||false|number(double)||
|&emsp;&emsp;agvMapName|地图名称||false|string||
|&emsp;&emsp;angle|角度||false|number(double)||
|&emsp;&emsp;type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点||false|string||
|&emsp;&emsp;covariance|协方差矩阵||false|string||
|&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;dockingPoint|对接点||false|DockingPoint|DockingPoint|
|&emsp;&emsp;&emsp;&emsp;qrDockId|地面二维码坐标ID||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;relativeX|相对x坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;relativeY|相对y坐标||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;relativeAngle|相对角度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点||false|string||
|&emsp;&emsp;&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否||false|integer(int32)||
|&emsp;&emsp;isPark|是否可泊车, 0:不可泊车，1：可泊车||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Marker|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|code|编码|string||
|x|x坐标|number(double)|number(double)|
|y|y坐标|number(double)|number(double)|
|agvMapName|地图名称|string||
|angle|角度|number(double)|number(double)|
|type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点|string||
|covariance|协方差矩阵|string||
|usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|dockingPoint|对接点|DockingPoint|DockingPoint|
|&emsp;&emsp;qrDockId|地面二维码坐标ID|integer(int32)||
|&emsp;&emsp;relativeX|相对x坐标|number(double)||
|&emsp;&emsp;relativeY|相对y坐标|number(double)||
|&emsp;&emsp;relativeAngle|相对角度|number(double)||
|&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点|string||
|&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接|integer(int32)||
|&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否|integer(int32)||
|isPark|是否可泊车, 0:不可泊车，1：可泊车|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"id": "",
	"code": "",
	"x": 0,
	"y": 0,
	"agvMapName": "",
	"angle": 0,
	"type": "",
	"covariance": "",
	"usageStatus": "",
	"dockingPoint": {
		"qrDockId": 0,
		"relativeX": 0,
		"relativeY": 0,
		"relativeAngle": 0,
		"type": "",
		"direction": 0,
		"isChargeStation": 0
	},
	"isPark": 0
}
```


## 根据标记点类型查询与当前标记点有路径的所有点位列表


**接口地址**:`/api/v3/markers/{id}/listMakerIds`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:根据标记点类型查询与当前标记点有路径的所有点位列表


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|agvMapId|地图id|query|true|string||
|id|标记ID|path|true|string||
|isDraft|是否查询操作数据|query|true|boolean||
|type|标记点类型|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Marker|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|code|编码|string||
|x|x坐标|number(double)|number(double)|
|y|y坐标|number(double)|number(double)|
|agvMapName|地图名称|string||
|angle|角度|number(double)|number(double)|
|type|类型 INITIAL_MARKER:初始点, CHARGING_MARKER:充电点, NAVIGATION_MARKER:导航点, WORK_MARKER:工作点, ADJUST_MARKER:调整点, ELEVATOR_MARKER:电梯点 , AVOID_MARKER:避让点|string||
|covariance|协方差矩阵|string||
|usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|dockingPoint|对接点|DockingPoint|DockingPoint|
|&emsp;&emsp;qrDockId|地面二维码坐标ID|integer(int32)||
|&emsp;&emsp;relativeX|相对x坐标|number(double)||
|&emsp;&emsp;relativeY|相对y坐标|number(double)||
|&emsp;&emsp;relativeAngle|相对角度|number(double)||
|&emsp;&emsp;type|类型 REFLECTOR_POINT:反光条特征对接点, V_POINT:V型特征对接点|string||
|&emsp;&emsp;direction|对接方式 1、车头对接  2、车尾对接|integer(int32)||
|&emsp;&emsp;isChargeStation|是否是充电桩 1、是  0、否|integer(int32)||
|isPark|是否可泊车, 0:不可泊车，1：可泊车|integer(int32)|integer(int32)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"code": "",
		"x": 0,
		"y": 0,
		"agvMapName": "",
		"angle": 0,
		"type": "",
		"covariance": "",
		"usageStatus": "",
		"dockingPoint": {
			"qrDockId": 0,
			"relativeX": 0,
			"relativeY": 0,
			"relativeAngle": 0,
			"type": "",
			"direction": 0,
			"isChargeStation": 0
		},
		"isPark": 0
	}
]
```


# 楼层


## 列表


**接口地址**:`/api/v3/floors`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Floor|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|elevatorId|电梯ID|string||
|agvMapId|地图ID|string||
|markerId|标记点ID, type=ELEVATOR_MARKER的标记点才可添加|string||
|number|楼层数|integer(int32)|integer(int32)|
|createdBy|创建方式 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||
|markerCode|标记点code|string||
|readFunctionCode|读modbus功能码|string||
|statusAddress|门状态地址|integer(int32)|integer(int32)|
|openStatusValue|开门状态值|integer(int32)|integer(int32)|
|closeStatusValue|关门状态值|integer(int32)|integer(int32)|
|writeFunctionCode|写modbus功能码|string||
|operateAddress|门操作地址|integer(int32)|integer(int32)|
|operate_out_open_value|操作外呼开门值|integer(int32)|integer(int32)|
|operate_in_open_value|操作内呼开门值|integer(int32)|integer(int32)|
|operateCloseValue|操作关门值|integer(int32)|integer(int32)|
|createTime|创建时间|string(date-time)|string(date-time)|
|elevatorArriveAddress|电梯到位地址|integer(int32)|integer(int32)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"elevatorId": "",
		"agvMapId": "",
		"markerId": "",
		"number": 0,
		"createdBy": "",
		"markerCode": "",
		"readFunctionCode": "",
		"statusAddress": 0,
		"openStatusValue": 0,
		"closeStatusValue": 0,
		"writeFunctionCode": "",
		"operateAddress": 0,
		"operate_out_open_value": 0,
		"operate_in_open_value": 0,
		"operateCloseValue": 0,
		"createTime": "",
		"elevatorArriveAddress": 0,
		"updateTime": ""
	}
]
```


## 创建


**接口地址**:`/api/v3/floors`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"elevatorId": "",
	"agvMapId": "",
	"markerId": "",
	"number": 0,
	"createdBy": "",
	"markerCode": "",
	"readFunctionCode": "",
	"statusAddress": 0,
	"openStatusValue": 0,
	"closeStatusValue": 0,
	"writeFunctionCode": "",
	"operateAddress": 0,
	"operate_out_open_value": 0,
	"operate_in_open_value": 0,
	"operateCloseValue": 0,
	"createTime": "",
	"elevatorArriveAddress": 0,
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|floor|楼层|body|true|Floor|Floor|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;elevatorId|电梯ID||false|string||
|&emsp;&emsp;agvMapId|地图ID||false|string||
|&emsp;&emsp;markerId|标记点ID, type=ELEVATOR_MARKER的标记点才可添加||false|string||
|&emsp;&emsp;number|楼层数||false|integer(int32)||
|&emsp;&emsp;createdBy|创建方式 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass||false|string||
|&emsp;&emsp;markerCode|标记点code||false|string||
|&emsp;&emsp;readFunctionCode|读modbus功能码||false|string||
|&emsp;&emsp;statusAddress|门状态地址||false|integer(int32)||
|&emsp;&emsp;openStatusValue|开门状态值||false|integer(int32)||
|&emsp;&emsp;closeStatusValue|关门状态值||false|integer(int32)||
|&emsp;&emsp;writeFunctionCode|写modbus功能码||false|string||
|&emsp;&emsp;operateAddress|门操作地址||false|integer(int32)||
|&emsp;&emsp;operate_out_open_value|操作外呼开门值||false|integer(int32)||
|&emsp;&emsp;operate_in_open_value|操作内呼开门值||false|integer(int32)||
|&emsp;&emsp;operateCloseValue|操作关门值||false|integer(int32)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;elevatorArriveAddress|电梯到位地址||false|integer(int32)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|Floor|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|elevatorId|电梯ID|string||
|agvMapId|地图ID|string||
|markerId|标记点ID, type=ELEVATOR_MARKER的标记点才可添加|string||
|number|楼层数|integer(int32)|integer(int32)|
|createdBy|创建方式 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||
|markerCode|标记点code|string||
|readFunctionCode|读modbus功能码|string||
|statusAddress|门状态地址|integer(int32)|integer(int32)|
|openStatusValue|开门状态值|integer(int32)|integer(int32)|
|closeStatusValue|关门状态值|integer(int32)|integer(int32)|
|writeFunctionCode|写modbus功能码|string||
|operateAddress|门操作地址|integer(int32)|integer(int32)|
|operate_out_open_value|操作外呼开门值|integer(int32)|integer(int32)|
|operate_in_open_value|操作内呼开门值|integer(int32)|integer(int32)|
|operateCloseValue|操作关门值|integer(int32)|integer(int32)|
|createTime|创建时间|string(date-time)|string(date-time)|
|elevatorArriveAddress|电梯到位地址|integer(int32)|integer(int32)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"elevatorId": "",
	"agvMapId": "",
	"markerId": "",
	"number": 0,
	"createdBy": "",
	"markerCode": "",
	"readFunctionCode": "",
	"statusAddress": 0,
	"openStatusValue": 0,
	"closeStatusValue": 0,
	"writeFunctionCode": "",
	"operateAddress": 0,
	"operate_out_open_value": 0,
	"operate_in_open_value": 0,
	"operateCloseValue": 0,
	"createTime": "",
	"elevatorArriveAddress": 0,
	"updateTime": ""
}
```


## 分页查询


**接口地址**:`/api/v3/floors/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«Floor»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|Floor|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;elevatorId|电梯ID|string||
|&emsp;&emsp;agvMapId|地图ID|string||
|&emsp;&emsp;markerId|标记点ID, type=ELEVATOR_MARKER的标记点才可添加|string||
|&emsp;&emsp;number|楼层数|integer(int32)||
|&emsp;&emsp;createdBy|创建方式 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||
|&emsp;&emsp;markerCode|标记点code|string||
|&emsp;&emsp;readFunctionCode|读modbus功能码|string||
|&emsp;&emsp;statusAddress|门状态地址|integer(int32)||
|&emsp;&emsp;openStatusValue|开门状态值|integer(int32)||
|&emsp;&emsp;closeStatusValue|关门状态值|integer(int32)||
|&emsp;&emsp;writeFunctionCode|写modbus功能码|string||
|&emsp;&emsp;operateAddress|门操作地址|integer(int32)||
|&emsp;&emsp;operate_out_open_value|操作外呼开门值|integer(int32)||
|&emsp;&emsp;operate_in_open_value|操作内呼开门值|integer(int32)||
|&emsp;&emsp;operateCloseValue|操作关门值|integer(int32)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;elevatorArriveAddress|电梯到位地址|integer(int32)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"elevatorId": "",
			"agvMapId": "",
			"markerId": "",
			"number": 0,
			"createdBy": "",
			"markerCode": "",
			"readFunctionCode": "",
			"statusAddress": 0,
			"openStatusValue": 0,
			"closeStatusValue": 0,
			"writeFunctionCode": "",
			"operateAddress": 0,
			"operate_out_open_value": 0,
			"operate_in_open_value": 0,
			"operateCloseValue": 0,
			"createTime": "",
			"elevatorArriveAddress": 0,
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/floors/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|楼层ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Floor|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|elevatorId|电梯ID|string||
|agvMapId|地图ID|string||
|markerId|标记点ID, type=ELEVATOR_MARKER的标记点才可添加|string||
|number|楼层数|integer(int32)|integer(int32)|
|createdBy|创建方式 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||
|markerCode|标记点code|string||
|readFunctionCode|读modbus功能码|string||
|statusAddress|门状态地址|integer(int32)|integer(int32)|
|openStatusValue|开门状态值|integer(int32)|integer(int32)|
|closeStatusValue|关门状态值|integer(int32)|integer(int32)|
|writeFunctionCode|写modbus功能码|string||
|operateAddress|门操作地址|integer(int32)|integer(int32)|
|operate_out_open_value|操作外呼开门值|integer(int32)|integer(int32)|
|operate_in_open_value|操作内呼开门值|integer(int32)|integer(int32)|
|operateCloseValue|操作关门值|integer(int32)|integer(int32)|
|createTime|创建时间|string(date-time)|string(date-time)|
|elevatorArriveAddress|电梯到位地址|integer(int32)|integer(int32)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"elevatorId": "",
	"agvMapId": "",
	"markerId": "",
	"number": 0,
	"createdBy": "",
	"markerCode": "",
	"readFunctionCode": "",
	"statusAddress": 0,
	"openStatusValue": 0,
	"closeStatusValue": 0,
	"writeFunctionCode": "",
	"operateAddress": 0,
	"operate_out_open_value": 0,
	"operate_in_open_value": 0,
	"operateCloseValue": 0,
	"createTime": "",
	"elevatorArriveAddress": 0,
	"updateTime": ""
}
```


## 更新


**接口地址**:`/api/v3/floors/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"elevatorId": "",
	"agvMapId": "",
	"markerId": "",
	"number": 0,
	"createdBy": "",
	"markerCode": "",
	"readFunctionCode": "",
	"statusAddress": 0,
	"openStatusValue": 0,
	"closeStatusValue": 0,
	"writeFunctionCode": "",
	"operateAddress": 0,
	"operate_out_open_value": 0,
	"operate_in_open_value": 0,
	"operateCloseValue": 0,
	"createTime": "",
	"elevatorArriveAddress": 0,
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|floor|楼层|body|true|Floor|Floor|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;elevatorId|电梯ID||false|string||
|&emsp;&emsp;agvMapId|地图ID||false|string||
|&emsp;&emsp;markerId|标记点ID, type=ELEVATOR_MARKER的标记点才可添加||false|string||
|&emsp;&emsp;number|楼层数||false|integer(int32)||
|&emsp;&emsp;createdBy|创建方式 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass||false|string||
|&emsp;&emsp;markerCode|标记点code||false|string||
|&emsp;&emsp;readFunctionCode|读modbus功能码||false|string||
|&emsp;&emsp;statusAddress|门状态地址||false|integer(int32)||
|&emsp;&emsp;openStatusValue|开门状态值||false|integer(int32)||
|&emsp;&emsp;closeStatusValue|关门状态值||false|integer(int32)||
|&emsp;&emsp;writeFunctionCode|写modbus功能码||false|string||
|&emsp;&emsp;operateAddress|门操作地址||false|integer(int32)||
|&emsp;&emsp;operate_out_open_value|操作外呼开门值||false|integer(int32)||
|&emsp;&emsp;operate_in_open_value|操作内呼开门值||false|integer(int32)||
|&emsp;&emsp;operateCloseValue|操作关门值||false|integer(int32)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;elevatorArriveAddress|电梯到位地址||false|integer(int32)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|id|楼层ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Floor|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|elevatorId|电梯ID|string||
|agvMapId|地图ID|string||
|markerId|标记点ID, type=ELEVATOR_MARKER的标记点才可添加|string||
|number|楼层数|integer(int32)|integer(int32)|
|createdBy|创建方式 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||
|markerCode|标记点code|string||
|readFunctionCode|读modbus功能码|string||
|statusAddress|门状态地址|integer(int32)|integer(int32)|
|openStatusValue|开门状态值|integer(int32)|integer(int32)|
|closeStatusValue|关门状态值|integer(int32)|integer(int32)|
|writeFunctionCode|写modbus功能码|string||
|operateAddress|门操作地址|integer(int32)|integer(int32)|
|operate_out_open_value|操作外呼开门值|integer(int32)|integer(int32)|
|operate_in_open_value|操作内呼开门值|integer(int32)|integer(int32)|
|operateCloseValue|操作关门值|integer(int32)|integer(int32)|
|createTime|创建时间|string(date-time)|string(date-time)|
|elevatorArriveAddress|电梯到位地址|integer(int32)|integer(int32)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"elevatorId": "",
	"agvMapId": "",
	"markerId": "",
	"number": 0,
	"createdBy": "",
	"markerCode": "",
	"readFunctionCode": "",
	"statusAddress": 0,
	"openStatusValue": 0,
	"closeStatusValue": 0,
	"writeFunctionCode": "",
	"operateAddress": 0,
	"operate_out_open_value": 0,
	"operate_in_open_value": 0,
	"operateCloseValue": 0,
	"createTime": "",
	"elevatorArriveAddress": 0,
	"updateTime": ""
}
```


## 删除


**接口地址**:`/api/v3/floors/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|楼层ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 消息管理界面


## 列表


**接口地址**:`/api/v3/messageManagement`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AbnormalPrompt|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|abnormalLevel|异常等级 1：普通 2：警告 3：错误|integer(int32)|integer(int32)|
|abnormalType|异常类型|string||
|abnormalCode|异常编码|integer(int32)|integer(int32)|
|abnormalDescription|异常描述|string||
|help|异常处理建议|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"abnormalLevel": 0,
		"abnormalType": "",
		"abnormalCode": 0,
		"abnormalDescription": "",
		"help": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


## 创建


**接口地址**:`/api/v3/messageManagement`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"abnormalLevel": 0,
	"abnormalType": "",
	"abnormalCode": 0,
	"abnormalDescription": "",
	"help": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|abnormalPrompt|异常信息|body|true|AbnormalPrompt|AbnormalPrompt|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;abnormalLevel|异常等级 1：普通 2：警告 3：错误||false|integer(int32)||
|&emsp;&emsp;abnormalType|异常类型||false|string||
|&emsp;&emsp;abnormalCode|异常编码||false|integer(int32)||
|&emsp;&emsp;abnormalDescription|异常描述||false|string||
|&emsp;&emsp;help|异常处理建议||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 更新


**接口地址**:`/api/v3/messageManagement`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"abnormalLevel": 0,
	"abnormalType": "",
	"abnormalCode": 0,
	"abnormalDescription": "",
	"help": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|abnormalPrompt|异常信息|body|true|AbnormalPrompt|AbnormalPrompt|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;abnormalLevel|异常等级 1：普通 2：警告 3：错误||false|integer(int32)||
|&emsp;&emsp;abnormalType|异常类型||false|string||
|&emsp;&emsp;abnormalCode|异常编码||false|integer(int32)||
|&emsp;&emsp;abnormalDescription|异常描述||false|string||
|&emsp;&emsp;help|异常处理建议||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AbnormalPrompt|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|abnormalLevel|异常等级 1：普通 2：警告 3：错误|integer(int32)|integer(int32)|
|abnormalType|异常类型|string||
|abnormalCode|异常编码|integer(int32)|integer(int32)|
|abnormalDescription|异常描述|string||
|help|异常处理建议|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"abnormalLevel": 0,
	"abnormalType": "",
	"abnormalCode": 0,
	"abnormalDescription": "",
	"help": "",
	"createTime": "",
	"updateTime": ""
}
```


## 导出


**接口地址**:`/api/v3/messageManagement/downExcelFile`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|abnormalCode|异常编码|path|false|ref||
|abnormalDescription|异常描述|path|false|string||
|abnormalLevel|异常等级|path|false|ref||
|abnormalType|异常类型|path|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 获取异常类型列表


**接口地址**:`/api/v3/messageManagement/getAbnormalTypeList`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 分页查询


**接口地址**:`/api/v3/messageManagement/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«AbnormalPrompt»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|AbnormalPrompt|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;abnormalLevel|异常等级 1：普通 2：警告 3：错误|integer(int32)||
|&emsp;&emsp;abnormalType|异常类型|string||
|&emsp;&emsp;abnormalCode|异常编码|integer(int32)||
|&emsp;&emsp;abnormalDescription|异常描述|string||
|&emsp;&emsp;help|异常处理建议|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"abnormalLevel": 0,
			"abnormalType": "",
			"abnormalCode": 0,
			"abnormalDescription": "",
			"help": "",
			"createTime": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 导入


**接口地址**:`/api/v3/messageManagement/uploadExcelFile`


**请求方式**:`POST`


**请求数据类型**:`multipart/form-data`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|multiPartFile|异常信息文件|formData|true|ref||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 详情


**接口地址**:`/api/v3/messageManagement/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|异常信息ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AbnormalPrompt|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|abnormalLevel|异常等级 1：普通 2：警告 3：错误|integer(int32)|integer(int32)|
|abnormalType|异常类型|string||
|abnormalCode|异常编码|integer(int32)|integer(int32)|
|abnormalDescription|异常描述|string||
|help|异常处理建议|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"abnormalLevel": 0,
	"abnormalType": "",
	"abnormalCode": 0,
	"abnormalDescription": "",
	"help": "",
	"createTime": "",
	"updateTime": ""
}
```


## 删除


**接口地址**:`/api/v3/messageManagement/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|异常信息ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 消息通知


## 列表


**接口地址**:`/api/v3/notification`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Notification|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|description|描述|string||
|type|消息类型|string||
|missionWorkId|任务的uuid|string||
|missionWorkName|任务的名字|string||
|haveRead|是否已读 UNREAD：未读； READ：已读|string||
|scale|消息级别 1：普通； 2：警告； 3：错误|integer(int32)|integer(int32)|
|errorCode|异常码|integer(int32)|integer(int32)|
|help|处理建议|string||
|mode|工作模式 本地:LOCAL 调度:SCHEDULER|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"description": "",
		"type": "",
		"missionWorkId": "",
		"missionWorkName": "",
		"haveRead": "",
		"scale": 0,
		"errorCode": 0,
		"help": "",
		"mode": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


## 创建


**接口地址**:`/api/v3/notification`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"description": "",
	"type": "",
	"missionWorkId": "",
	"missionWorkName": "",
	"haveRead": "",
	"scale": 0,
	"errorCode": 0,
	"help": "",
	"mode": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|notification|消息通知类型|body|true|Notification|Notification|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;type|消息类型||false|string||
|&emsp;&emsp;missionWorkId|任务的uuid||false|string||
|&emsp;&emsp;missionWorkName|任务的名字||false|string||
|&emsp;&emsp;haveRead|是否已读 UNREAD：未读； READ：已读||false|string||
|&emsp;&emsp;scale|消息级别 1：普通； 2：警告； 3：错误||false|integer(int32)||
|&emsp;&emsp;errorCode|异常码||false|integer(int32)||
|&emsp;&emsp;help|处理建议||false|string||
|&emsp;&emsp;mode|工作模式 本地:LOCAL 调度:SCHEDULER||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|Notification|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|description|描述|string||
|type|消息类型|string||
|missionWorkId|任务的uuid|string||
|missionWorkName|任务的名字|string||
|haveRead|是否已读 UNREAD：未读； READ：已读|string||
|scale|消息级别 1：普通； 2：警告； 3：错误|integer(int32)|integer(int32)|
|errorCode|异常码|integer(int32)|integer(int32)|
|help|处理建议|string||
|mode|工作模式 本地:LOCAL 调度:SCHEDULER|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"description": "",
	"type": "",
	"missionWorkId": "",
	"missionWorkName": "",
	"haveRead": "",
	"scale": 0,
	"errorCode": 0,
	"help": "",
	"mode": "",
	"createTime": "",
	"updateTime": ""
}
```


## 获取消息类型列表


**接口地址**:`/api/v3/notification/getNotificationTypeList`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 分页查询


**接口地址**:`/api/v3/notification/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«Notification»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|Notification|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;type|消息类型|string||
|&emsp;&emsp;missionWorkId|任务的uuid|string||
|&emsp;&emsp;missionWorkName|任务的名字|string||
|&emsp;&emsp;haveRead|是否已读 UNREAD：未读； READ：已读|string||
|&emsp;&emsp;scale|消息级别 1：普通； 2：警告； 3：错误|integer(int32)||
|&emsp;&emsp;errorCode|异常码|integer(int32)||
|&emsp;&emsp;help|处理建议|string||
|&emsp;&emsp;mode|工作模式 本地:LOCAL 调度:SCHEDULER|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"description": "",
			"type": "",
			"missionWorkId": "",
			"missionWorkName": "",
			"haveRead": "",
			"scale": 0,
			"errorCode": 0,
			"help": "",
			"mode": "",
			"createTime": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/notification/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:根据ID获取Notification详情


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|NotificationID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Notification|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|description|描述|string||
|type|消息类型|string||
|missionWorkId|任务的uuid|string||
|missionWorkName|任务的名字|string||
|haveRead|是否已读 UNREAD：未读； READ：已读|string||
|scale|消息级别 1：普通； 2：警告； 3：错误|integer(int32)|integer(int32)|
|errorCode|异常码|integer(int32)|integer(int32)|
|help|处理建议|string||
|mode|工作模式 本地:LOCAL 调度:SCHEDULER|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"description": "",
	"type": "",
	"missionWorkId": "",
	"missionWorkName": "",
	"haveRead": "",
	"scale": 0,
	"errorCode": 0,
	"help": "",
	"mode": "",
	"createTime": "",
	"updateTime": ""
}
```


## 更新


**接口地址**:`/api/v3/notification/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:根据ID更新Notification信息


**请求示例**:


```javascript
{
	"id": "",
	"description": "",
	"type": "",
	"missionWorkId": "",
	"missionWorkName": "",
	"haveRead": "",
	"scale": 0,
	"errorCode": 0,
	"help": "",
	"mode": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|NotificationID|path|true|string||
|notification|消息通知类型|body|true|Notification|Notification|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;type|消息类型||false|string||
|&emsp;&emsp;missionWorkId|任务的uuid||false|string||
|&emsp;&emsp;missionWorkName|任务的名字||false|string||
|&emsp;&emsp;haveRead|是否已读 UNREAD：未读； READ：已读||false|string||
|&emsp;&emsp;scale|消息级别 1：普通； 2：警告； 3：错误||false|integer(int32)||
|&emsp;&emsp;errorCode|异常码||false|integer(int32)||
|&emsp;&emsp;help|处理建议||false|string||
|&emsp;&emsp;mode|工作模式 本地:LOCAL 调度:SCHEDULER||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Notification|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|description|描述|string||
|type|消息类型|string||
|missionWorkId|任务的uuid|string||
|missionWorkName|任务的名字|string||
|haveRead|是否已读 UNREAD：未读； READ：已读|string||
|scale|消息级别 1：普通； 2：警告； 3：错误|integer(int32)|integer(int32)|
|errorCode|异常码|integer(int32)|integer(int32)|
|help|处理建议|string||
|mode|工作模式 本地:LOCAL 调度:SCHEDULER|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"description": "",
	"type": "",
	"missionWorkId": "",
	"missionWorkName": "",
	"haveRead": "",
	"scale": 0,
	"errorCode": 0,
	"help": "",
	"mode": "",
	"createTime": "",
	"updateTime": ""
}
```


## 删除


**接口地址**:`/api/v3/notification/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:根据ID删除Notification信息


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|NotificationID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 用户操作指南下载模板(DownloadController)


## 操作手册下载


**接口地址**:`/api/v3/download/file/{fileType}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`*/*`


**接口描述**:用户点击后下载操作手册


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|fileType|下载类型(1:用户手册下载，2:API操作手册下载)|path|true|ref||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 电梯


## 列表


**接口地址**:`/api/v3/elevators`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Elevator|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|description|描述|string||
|customer|客户 TAI_CHI:太极|string||
|ip|操作电梯的IP地址|string||
|port|操作电梯的端口号|integer(int32)|integer(int32)|
|applyTimeout|申请电梯超时时间 单位：秒|integer(int32)|integer(int32)|
|controlTimeout|控制电梯超时时间 单位：秒|integer(int32)|integer(int32)|
|createdBy|创建方式 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"name": "",
		"description": "",
		"customer": "",
		"ip": "",
		"port": 0,
		"applyTimeout": 0,
		"controlTimeout": 0,
		"createdBy": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


## 创建


**接口地址**:`/api/v3/elevators`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"name": "",
	"description": "",
	"customer": "",
	"ip": "",
	"port": 0,
	"applyTimeout": 0,
	"controlTimeout": 0,
	"createdBy": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|elevator|电梯|body|true|Elevator|Elevator|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;customer|客户 TAI_CHI:太极||false|string||
|&emsp;&emsp;ip|操作电梯的IP地址||false|string||
|&emsp;&emsp;port|操作电梯的端口号||false|integer(int32)||
|&emsp;&emsp;applyTimeout|申请电梯超时时间 单位：秒||false|integer(int32)||
|&emsp;&emsp;controlTimeout|控制电梯超时时间 单位：秒||false|integer(int32)||
|&emsp;&emsp;createdBy|创建方式 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|Elevator|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|description|描述|string||
|customer|客户 TAI_CHI:太极|string||
|ip|操作电梯的IP地址|string||
|port|操作电梯的端口号|integer(int32)|integer(int32)|
|applyTimeout|申请电梯超时时间 单位：秒|integer(int32)|integer(int32)|
|controlTimeout|控制电梯超时时间 单位：秒|integer(int32)|integer(int32)|
|createdBy|创建方式 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"description": "",
	"customer": "",
	"ip": "",
	"port": 0,
	"applyTimeout": 0,
	"controlTimeout": 0,
	"createdBy": "",
	"createTime": "",
	"updateTime": ""
}
```


## 分页查询


**接口地址**:`/api/v3/elevators/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«Elevator»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|Elevator|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;customer|客户 TAI_CHI:太极|string||
|&emsp;&emsp;ip|操作电梯的IP地址|string||
|&emsp;&emsp;port|操作电梯的端口号|integer(int32)||
|&emsp;&emsp;applyTimeout|申请电梯超时时间 单位：秒|integer(int32)||
|&emsp;&emsp;controlTimeout|控制电梯超时时间 单位：秒|integer(int32)||
|&emsp;&emsp;createdBy|创建方式 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"name": "",
			"description": "",
			"customer": "",
			"ip": "",
			"port": 0,
			"applyTimeout": 0,
			"controlTimeout": 0,
			"createdBy": "",
			"createTime": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/elevators/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|电梯ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Elevator|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|description|描述|string||
|customer|客户 TAI_CHI:太极|string||
|ip|操作电梯的IP地址|string||
|port|操作电梯的端口号|integer(int32)|integer(int32)|
|applyTimeout|申请电梯超时时间 单位：秒|integer(int32)|integer(int32)|
|controlTimeout|控制电梯超时时间 单位：秒|integer(int32)|integer(int32)|
|createdBy|创建方式 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"description": "",
	"customer": "",
	"ip": "",
	"port": 0,
	"applyTimeout": 0,
	"controlTimeout": 0,
	"createdBy": "",
	"createTime": "",
	"updateTime": ""
}
```


## 更新


**接口地址**:`/api/v3/elevators/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"name": "",
	"description": "",
	"customer": "",
	"ip": "",
	"port": 0,
	"applyTimeout": 0,
	"controlTimeout": 0,
	"createdBy": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|elevator|电梯|body|true|Elevator|Elevator|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;customer|客户 TAI_CHI:太极||false|string||
|&emsp;&emsp;ip|操作电梯的IP地址||false|string||
|&emsp;&emsp;port|操作电梯的端口号||false|integer(int32)||
|&emsp;&emsp;applyTimeout|申请电梯超时时间 单位：秒||false|integer(int32)||
|&emsp;&emsp;controlTimeout|控制电梯超时时间 单位：秒||false|integer(int32)||
|&emsp;&emsp;createdBy|创建方式 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|id|电梯ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Elevator|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|description|描述|string||
|customer|客户 TAI_CHI:太极|string||
|ip|操作电梯的IP地址|string||
|port|操作电梯的端口号|integer(int32)|integer(int32)|
|applyTimeout|申请电梯超时时间 单位：秒|integer(int32)|integer(int32)|
|controlTimeout|控制电梯超时时间 单位：秒|integer(int32)|integer(int32)|
|createdBy|创建方式 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"description": "",
	"customer": "",
	"ip": "",
	"port": 0,
	"applyTimeout": 0,
	"controlTimeout": 0,
	"createdBy": "",
	"createTime": "",
	"updateTime": ""
}
```


## 删除


**接口地址**:`/api/v3/elevators/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|电梯ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 登录


## 用户验证


**接口地址**:`/api/v3/login/listUser`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:用户验证


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|loginName|用户名|query|true|string||
|password|admin用户密码|query|true|string||
|createTime|创建时间|query|false|string(date-time)||
|dashboardId|dashboard的ID|query|false|string||
|email|邮箱|query|false|string||
|id|ID|query|false|string||
|name|名称|query|false|string||
|phone|电话|query|false|string||
|updateTime|更新时间|query|false|string(date-time)||
|userGroupId|用户组的ID|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|User|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|dashboardId|dashboard的ID|string||
|userGroupId|用户组的ID|string||
|name|名称|string||
|loginName|登陆帐号|string||
|password|登陆密码|string||
|email|邮箱|string||
|phone|电话|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"dashboardId": "",
	"userGroupId": "",
	"name": "",
	"loginName": "",
	"password": "",
	"email": "",
	"phone": "",
	"createTime": "",
	"updateTime": ""
}
```


## 修改密码


**接口地址**:`/api/v3/login/updateUser`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:修改用户密码


**请求示例**:


```javascript
{
	"password": "",
	"oldPassword": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param|修改用户密码参数|body|true|UserPwdUpdateParam|UserPwdUpdateParam|
|&emsp;&emsp;password|登陆密码||false|string||
|&emsp;&emsp;oldPassword|原始密码||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|User|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|dashboardId|dashboard的ID|string||
|userGroupId|用户组的ID|string||
|name|名称|string||
|loginName|登陆帐号|string||
|password|登陆密码|string||
|email|邮箱|string||
|phone|电话|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"dashboardId": "",
	"userGroupId": "",
	"name": "",
	"loginName": "",
	"password": "",
	"email": "",
	"phone": "",
	"createTime": "",
	"updateTime": ""
}
```


## 登录


**接口地址**:`/api/v3/login/userLogin`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:登录


**请求示例**:


```javascript
{
	"loginName": "",
	"password": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param|用户登录参数|body|true|UserLoginParam|UserLoginParam|
|&emsp;&emsp;loginName|登录名称||false|string||
|&emsp;&emsp;password|登录密码||false|string||
|user|用户||true|User|User|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;dashboardId|dashboard的ID||false|string||
|&emsp;&emsp;userGroupId|用户组的ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;loginName|登陆帐号||false|string||
|&emsp;&emsp;password|登陆密码||false|string||
|&emsp;&emsp;email|邮箱||false|string||
|&emsp;&emsp;phone|电话||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 系统工作模式


## 详情


**接口地址**:`/api/v3/systemWorkMode`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|SystemWorkMode|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|mode|工作模式 LOCAL:本地模式 SCHEDULER:调度模式|string||
|schedulerUrl|调度地址|string||
|loginStatus|登录状态 当mode=SCHEDULER生效 NO_LOGGED_IN:未登录 LOGGED_IN:已登录 LOGGED_FAULT:登录失败|string||
|onlineStatus|在线状态 ONLINE:在线  OFFLINE:离线|string||
|message|错误信息|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"mode": "",
	"schedulerUrl": "",
	"loginStatus": "",
	"onlineStatus": "",
	"message": "",
	"createTime": "",
	"updateTime": ""
}
```


## 更新


**接口地址**:`/api/v3/systemWorkMode/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:更新


**请求示例**:


```javascript
{
	"id": "",
	"mode": "",
	"schedulerUrl": "",
	"loginStatus": "",
	"onlineStatus": "",
	"message": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|ID|path|true|string||
|systemWorkMode|系统工作模式|body|true|SystemWorkMode|SystemWorkMode|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;mode|工作模式 LOCAL:本地模式 SCHEDULER:调度模式||false|string||
|&emsp;&emsp;schedulerUrl|调度地址||false|string||
|&emsp;&emsp;loginStatus|登录状态 当mode=SCHEDULER生效 NO_LOGGED_IN:未登录 LOGGED_IN:已登录 LOGGED_FAULT:登录失败||false|string||
|&emsp;&emsp;onlineStatus|在线状态 ONLINE:在线  OFFLINE:离线||false|string||
|&emsp;&emsp;message|错误信息||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|SystemWorkMode|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|mode|工作模式 LOCAL:本地模式 SCHEDULER:调度模式|string||
|schedulerUrl|调度地址|string||
|loginStatus|登录状态 当mode=SCHEDULER生效 NO_LOGGED_IN:未登录 LOGGED_IN:已登录 LOGGED_FAULT:登录失败|string||
|onlineStatus|在线状态 ONLINE:在线  OFFLINE:离线|string||
|message|错误信息|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"mode": "",
	"schedulerUrl": "",
	"loginStatus": "",
	"onlineStatus": "",
	"message": "",
	"createTime": "",
	"updateTime": ""
}
```


# 系统文档操作


## 下载api帮助手册


**接口地址**:`/api/v3/file/apiManual/download`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:用户点击后下载用户操作手册


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 下载用户操作手册


**接口地址**:`/api/v3/file/userManual/download`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:用户点击后下载用户操作手册


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 系统配置


## 查看系统配置


**接口地址**:`/api/v3/config`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|SystemConfig|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionWork|任务日志 单位:天|integer(int32)|integer(int32)|
|logFile|系统日志文件 单位:天|integer(int32)|integer(int32)|
|systemNotify|系统通知 单位:天|integer(int32)|integer(int32)|
|mqMessage|emq消息 单位:天|integer(int32)|integer(int32)|
|ftpUrl|ftp的主机|string||
|timeZone|系统时区|string||
|fleetInterval|系统时间与调度服务器的时间容差|integer(int32)|integer(int32)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|
|mapFileCleanInterval|地图文件清理周期 默认为:10天|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"id": "",
	"missionWork": 0,
	"logFile": 0,
	"systemNotify": 0,
	"mqMessage": 0,
	"ftpUrl": "",
	"timeZone": "",
	"fleetInterval": 0,
	"createTime": "",
	"updateTime": "",
	"mapFileCleanInterval": 0
}
```


## 修改系统配置


**接口地址**:`/api/v3/config`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"missionWork": 0,
	"logFile": 0,
	"systemNotify": 0,
	"mqMessage": 0,
	"ftpUrl": "",
	"timeZone": "",
	"fleetInterval": 0,
	"createTime": "",
	"updateTime": "",
	"mapFileCleanInterval": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|systemConfig|系统配置信息|body|true|SystemConfig|SystemConfig|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;missionWork|任务日志 单位:天||false|integer(int32)||
|&emsp;&emsp;logFile|系统日志文件 单位:天||false|integer(int32)||
|&emsp;&emsp;systemNotify|系统通知 单位:天||false|integer(int32)||
|&emsp;&emsp;mqMessage|emq消息 单位:天||false|integer(int32)||
|&emsp;&emsp;ftpUrl|ftp的主机||false|string||
|&emsp;&emsp;timeZone|系统时区||false|string||
|&emsp;&emsp;fleetInterval|系统时间与调度服务器的时间容差||false|integer(int32)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|&emsp;&emsp;mapFileCleanInterval|地图文件清理周期 默认为:10天||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 查看系统ftp配置


**接口地址**:`/api/v3/config/ftp`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|系统ftp设置|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|url|地址|string||
|port|端口|integer(int32)|integer(int32)|
|username|用户名|string||
|password|密码|string||
|rootPath|ftp根目录|string||


**响应示例**:
```javascript
{
	"url": "",
	"port": 0,
	"username": "",
	"password": "",
	"rootPath": ""
}
```


## 修改ftp系统配置


**接口地址**:`/api/v3/config/ftp`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ftpConfig|修改ftp系统配置|body|true|FtpConfig|FtpConfig|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 自动门


## 自动门和风淋门列表


**接口地址**:`/api/v3/autoDoor`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AutoDoor|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|ip|自动门ip|string||
|port|自动门端口|integer(int32)|integer(int32)|
|openAddress|开门地址|integer(int32)|integer(int32)|
|openStatusAddress|开门状态地址|integer(int32)|integer(int32)|
|closeAddress|关门地址|integer(int32)|integer(int32)|
|closeStatusAddress|关门状态地址|integer(int32)|integer(int32)|
|currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH|string||
|type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门|string||
|position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门|string||
|relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值|string||
|residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间|integer(int32)|integer(int32)|
|lastCloseDoorTime|最后一次关门完成时间|string(date-time)|string(date-time)|
|controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"name": "",
		"ip": "",
		"port": 0,
		"openAddress": 0,
		"openStatusAddress": 0,
		"closeAddress": 0,
		"closeStatusAddress": 0,
		"currentStatus": "",
		"type": "",
		"position": "",
		"relationDoorId": "",
		"residenceTime": 0,
		"lastCloseDoorTime": "",
		"controlMode": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


## 创建自动门


**接口地址**:`/api/v3/autoDoor`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"name": "",
	"ip": "",
	"port": 0,
	"openAddress": 0,
	"openStatusAddress": 0,
	"closeAddress": 0,
	"closeStatusAddress": 0,
	"currentStatus": "",
	"type": "",
	"position": "",
	"relationDoorId": "",
	"residenceTime": 0,
	"lastCloseDoorTime": "",
	"controlMode": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|autoDoor|自动门|body|true|AutoDoor|AutoDoor|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;ip|自动门ip||false|string||
|&emsp;&emsp;port|自动门端口||false|integer(int32)||
|&emsp;&emsp;openAddress|开门地址||false|integer(int32)||
|&emsp;&emsp;openStatusAddress|开门状态地址||false|integer(int32)||
|&emsp;&emsp;closeAddress|关门地址||false|integer(int32)||
|&emsp;&emsp;closeStatusAddress|关门状态地址||false|integer(int32)||
|&emsp;&emsp;currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH||false|string||
|&emsp;&emsp;type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门||false|string||
|&emsp;&emsp;position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门||false|string||
|&emsp;&emsp;relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值||false|string||
|&emsp;&emsp;residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间||false|integer(int32)||
|&emsp;&emsp;lastCloseDoorTime|最后一次关门完成时间||false|string(date-time)||
|&emsp;&emsp;controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|AutoDoor|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|ip|自动门ip|string||
|port|自动门端口|integer(int32)|integer(int32)|
|openAddress|开门地址|integer(int32)|integer(int32)|
|openStatusAddress|开门状态地址|integer(int32)|integer(int32)|
|closeAddress|关门地址|integer(int32)|integer(int32)|
|closeStatusAddress|关门状态地址|integer(int32)|integer(int32)|
|currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH|string||
|type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门|string||
|position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门|string||
|relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值|string||
|residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间|integer(int32)|integer(int32)|
|lastCloseDoorTime|最后一次关门完成时间|string(date-time)|string(date-time)|
|controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"ip": "",
	"port": 0,
	"openAddress": 0,
	"openStatusAddress": 0,
	"closeAddress": 0,
	"closeStatusAddress": 0,
	"currentStatus": "",
	"type": "",
	"position": "",
	"relationDoorId": "",
	"residenceTime": 0,
	"lastCloseDoorTime": "",
	"controlMode": "",
	"createTime": "",
	"updateTime": ""
}
```


## 更新自动门


**接口地址**:`/api/v3/autoDoor`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"name": "",
	"ip": "",
	"port": 0,
	"openAddress": 0,
	"openStatusAddress": 0,
	"closeAddress": 0,
	"closeStatusAddress": 0,
	"currentStatus": "",
	"type": "",
	"position": "",
	"relationDoorId": "",
	"residenceTime": 0,
	"lastCloseDoorTime": "",
	"controlMode": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|autoDoor|自动门|body|true|AutoDoor|AutoDoor|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;ip|自动门ip||false|string||
|&emsp;&emsp;port|自动门端口||false|integer(int32)||
|&emsp;&emsp;openAddress|开门地址||false|integer(int32)||
|&emsp;&emsp;openStatusAddress|开门状态地址||false|integer(int32)||
|&emsp;&emsp;closeAddress|关门地址||false|integer(int32)||
|&emsp;&emsp;closeStatusAddress|关门状态地址||false|integer(int32)||
|&emsp;&emsp;currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH||false|string||
|&emsp;&emsp;type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门||false|string||
|&emsp;&emsp;position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门||false|string||
|&emsp;&emsp;relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值||false|string||
|&emsp;&emsp;residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间||false|integer(int32)||
|&emsp;&emsp;lastCloseDoorTime|最后一次关门完成时间||false|string(date-time)||
|&emsp;&emsp;controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AutoDoor|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|ip|自动门ip|string||
|port|自动门端口|integer(int32)|integer(int32)|
|openAddress|开门地址|integer(int32)|integer(int32)|
|openStatusAddress|开门状态地址|integer(int32)|integer(int32)|
|closeAddress|关门地址|integer(int32)|integer(int32)|
|closeStatusAddress|关门状态地址|integer(int32)|integer(int32)|
|currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH|string||
|type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门|string||
|position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门|string||
|relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值|string||
|residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间|integer(int32)|integer(int32)|
|lastCloseDoorTime|最后一次关门完成时间|string(date-time)|string(date-time)|
|controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"ip": "",
	"port": 0,
	"openAddress": 0,
	"openStatusAddress": 0,
	"closeAddress": 0,
	"closeStatusAddress": 0,
	"currentStatus": "",
	"type": "",
	"position": "",
	"relationDoorId": "",
	"residenceTime": 0,
	"lastCloseDoorTime": "",
	"controlMode": "",
	"createTime": "",
	"updateTime": ""
}
```


## 创建风淋门


**接口地址**:`/api/v3/autoDoor/airShowerDoor`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"frontDoor": {
		"id": "",
		"name": "",
		"ip": "",
		"port": 0,
		"openAddress": 0,
		"openStatusAddress": 0,
		"closeAddress": 0,
		"closeStatusAddress": 0,
		"currentStatus": "",
		"type": "",
		"position": "",
		"relationDoorId": "",
		"residenceTime": 0,
		"lastCloseDoorTime": "",
		"controlMode": "",
		"createTime": "",
		"updateTime": ""
	},
	"backDoor": {
		"id": "",
		"name": "",
		"ip": "",
		"port": 0,
		"openAddress": 0,
		"openStatusAddress": 0,
		"closeAddress": 0,
		"closeStatusAddress": 0,
		"currentStatus": "",
		"type": "",
		"position": "",
		"relationDoorId": "",
		"residenceTime": 0,
		"lastCloseDoorTime": "",
		"controlMode": "",
		"createTime": "",
		"updateTime": ""
	}
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|airShowerDoor|风淋门|body|true|AirShowerDoor|AirShowerDoor|
|&emsp;&emsp;frontDoor|前门||false|AutoDoor|AutoDoor|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;&emsp;&emsp;ip|自动门ip||false|string||
|&emsp;&emsp;&emsp;&emsp;port|自动门端口||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;openAddress|开门地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;openStatusAddress|开门状态地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;closeAddress|关门地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;closeStatusAddress|关门状态地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH||false|string||
|&emsp;&emsp;&emsp;&emsp;type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门||false|string||
|&emsp;&emsp;&emsp;&emsp;position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门||false|string||
|&emsp;&emsp;&emsp;&emsp;relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值||false|string||
|&emsp;&emsp;&emsp;&emsp;residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;lastCloseDoorTime|最后一次关门完成时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|&emsp;&emsp;backDoor|后门||false|AutoDoor|AutoDoor|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;&emsp;&emsp;ip|自动门ip||false|string||
|&emsp;&emsp;&emsp;&emsp;port|自动门端口||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;openAddress|开门地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;openStatusAddress|开门状态地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;closeAddress|关门地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;closeStatusAddress|关门状态地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH||false|string||
|&emsp;&emsp;&emsp;&emsp;type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门||false|string||
|&emsp;&emsp;&emsp;&emsp;position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门||false|string||
|&emsp;&emsp;&emsp;&emsp;relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值||false|string||
|&emsp;&emsp;&emsp;&emsp;residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;lastCloseDoorTime|最后一次关门完成时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|AirShowerDoor|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|frontDoor|前门|AutoDoor|AutoDoor|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;ip|自动门ip|string||
|&emsp;&emsp;port|自动门端口|integer(int32)||
|&emsp;&emsp;openAddress|开门地址|integer(int32)||
|&emsp;&emsp;openStatusAddress|开门状态地址|integer(int32)||
|&emsp;&emsp;closeAddress|关门地址|integer(int32)||
|&emsp;&emsp;closeStatusAddress|关门状态地址|integer(int32)||
|&emsp;&emsp;currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH|string||
|&emsp;&emsp;type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门|string||
|&emsp;&emsp;position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门|string||
|&emsp;&emsp;relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值|string||
|&emsp;&emsp;residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间|integer(int32)||
|&emsp;&emsp;lastCloseDoorTime|最后一次关门完成时间|string(date-time)||
|&emsp;&emsp;controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|backDoor|后门|AutoDoor|AutoDoor|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;ip|自动门ip|string||
|&emsp;&emsp;port|自动门端口|integer(int32)||
|&emsp;&emsp;openAddress|开门地址|integer(int32)||
|&emsp;&emsp;openStatusAddress|开门状态地址|integer(int32)||
|&emsp;&emsp;closeAddress|关门地址|integer(int32)||
|&emsp;&emsp;closeStatusAddress|关门状态地址|integer(int32)||
|&emsp;&emsp;currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH|string||
|&emsp;&emsp;type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门|string||
|&emsp;&emsp;position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门|string||
|&emsp;&emsp;relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值|string||
|&emsp;&emsp;residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间|integer(int32)||
|&emsp;&emsp;lastCloseDoorTime|最后一次关门完成时间|string(date-time)||
|&emsp;&emsp;controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||


**响应示例**:
```javascript
{
	"frontDoor": {
		"id": "",
		"name": "",
		"ip": "",
		"port": 0,
		"openAddress": 0,
		"openStatusAddress": 0,
		"closeAddress": 0,
		"closeStatusAddress": 0,
		"currentStatus": "",
		"type": "",
		"position": "",
		"relationDoorId": "",
		"residenceTime": 0,
		"lastCloseDoorTime": "",
		"controlMode": "",
		"createTime": "",
		"updateTime": ""
	},
	"backDoor": {
		"id": "",
		"name": "",
		"ip": "",
		"port": 0,
		"openAddress": 0,
		"openStatusAddress": 0,
		"closeAddress": 0,
		"closeStatusAddress": 0,
		"currentStatus": "",
		"type": "",
		"position": "",
		"relationDoorId": "",
		"residenceTime": 0,
		"lastCloseDoorTime": "",
		"controlMode": "",
		"createTime": "",
		"updateTime": ""
	}
}
```


## 更新风淋门


**接口地址**:`/api/v3/autoDoor/airShowerDoor`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"frontDoor": {
		"id": "",
		"name": "",
		"ip": "",
		"port": 0,
		"openAddress": 0,
		"openStatusAddress": 0,
		"closeAddress": 0,
		"closeStatusAddress": 0,
		"currentStatus": "",
		"type": "",
		"position": "",
		"relationDoorId": "",
		"residenceTime": 0,
		"lastCloseDoorTime": "",
		"controlMode": "",
		"createTime": "",
		"updateTime": ""
	},
	"backDoor": {
		"id": "",
		"name": "",
		"ip": "",
		"port": 0,
		"openAddress": 0,
		"openStatusAddress": 0,
		"closeAddress": 0,
		"closeStatusAddress": 0,
		"currentStatus": "",
		"type": "",
		"position": "",
		"relationDoorId": "",
		"residenceTime": 0,
		"lastCloseDoorTime": "",
		"controlMode": "",
		"createTime": "",
		"updateTime": ""
	}
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|airShowerDoor|风淋门|body|true|AirShowerDoor|AirShowerDoor|
|&emsp;&emsp;frontDoor|前门||false|AutoDoor|AutoDoor|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;&emsp;&emsp;ip|自动门ip||false|string||
|&emsp;&emsp;&emsp;&emsp;port|自动门端口||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;openAddress|开门地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;openStatusAddress|开门状态地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;closeAddress|关门地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;closeStatusAddress|关门状态地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH||false|string||
|&emsp;&emsp;&emsp;&emsp;type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门||false|string||
|&emsp;&emsp;&emsp;&emsp;position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门||false|string||
|&emsp;&emsp;&emsp;&emsp;relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值||false|string||
|&emsp;&emsp;&emsp;&emsp;residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;lastCloseDoorTime|最后一次关门完成时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|&emsp;&emsp;backDoor|后门||false|AutoDoor|AutoDoor|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;&emsp;&emsp;ip|自动门ip||false|string||
|&emsp;&emsp;&emsp;&emsp;port|自动门端口||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;openAddress|开门地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;openStatusAddress|开门状态地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;closeAddress|关门地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;closeStatusAddress|关门状态地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH||false|string||
|&emsp;&emsp;&emsp;&emsp;type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门||false|string||
|&emsp;&emsp;&emsp;&emsp;position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门||false|string||
|&emsp;&emsp;&emsp;&emsp;relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值||false|string||
|&emsp;&emsp;&emsp;&emsp;residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;lastCloseDoorTime|最后一次关门完成时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AirShowerDoor|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|frontDoor|前门|AutoDoor|AutoDoor|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;ip|自动门ip|string||
|&emsp;&emsp;port|自动门端口|integer(int32)||
|&emsp;&emsp;openAddress|开门地址|integer(int32)||
|&emsp;&emsp;openStatusAddress|开门状态地址|integer(int32)||
|&emsp;&emsp;closeAddress|关门地址|integer(int32)||
|&emsp;&emsp;closeStatusAddress|关门状态地址|integer(int32)||
|&emsp;&emsp;currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH|string||
|&emsp;&emsp;type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门|string||
|&emsp;&emsp;position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门|string||
|&emsp;&emsp;relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值|string||
|&emsp;&emsp;residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间|integer(int32)||
|&emsp;&emsp;lastCloseDoorTime|最后一次关门完成时间|string(date-time)||
|&emsp;&emsp;controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|backDoor|后门|AutoDoor|AutoDoor|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;ip|自动门ip|string||
|&emsp;&emsp;port|自动门端口|integer(int32)||
|&emsp;&emsp;openAddress|开门地址|integer(int32)||
|&emsp;&emsp;openStatusAddress|开门状态地址|integer(int32)||
|&emsp;&emsp;closeAddress|关门地址|integer(int32)||
|&emsp;&emsp;closeStatusAddress|关门状态地址|integer(int32)||
|&emsp;&emsp;currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH|string||
|&emsp;&emsp;type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门|string||
|&emsp;&emsp;position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门|string||
|&emsp;&emsp;relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值|string||
|&emsp;&emsp;residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间|integer(int32)||
|&emsp;&emsp;lastCloseDoorTime|最后一次关门完成时间|string(date-time)||
|&emsp;&emsp;controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||


**响应示例**:
```javascript
{
	"frontDoor": {
		"id": "",
		"name": "",
		"ip": "",
		"port": 0,
		"openAddress": 0,
		"openStatusAddress": 0,
		"closeAddress": 0,
		"closeStatusAddress": 0,
		"currentStatus": "",
		"type": "",
		"position": "",
		"relationDoorId": "",
		"residenceTime": 0,
		"lastCloseDoorTime": "",
		"controlMode": "",
		"createTime": "",
		"updateTime": ""
	},
	"backDoor": {
		"id": "",
		"name": "",
		"ip": "",
		"port": 0,
		"openAddress": 0,
		"openStatusAddress": 0,
		"closeAddress": 0,
		"closeStatusAddress": 0,
		"currentStatus": "",
		"type": "",
		"position": "",
		"relationDoorId": "",
		"residenceTime": 0,
		"lastCloseDoorTime": "",
		"controlMode": "",
		"createTime": "",
		"updateTime": ""
	}
}
```


## 风淋门列表


**接口地址**:`/api/v3/autoDoor/airShowerDoorAll`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AirShowerDoor|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|frontDoor|前门|AutoDoor|AutoDoor|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;ip|自动门ip|string||
|&emsp;&emsp;port|自动门端口|integer(int32)||
|&emsp;&emsp;openAddress|开门地址|integer(int32)||
|&emsp;&emsp;openStatusAddress|开门状态地址|integer(int32)||
|&emsp;&emsp;closeAddress|关门地址|integer(int32)||
|&emsp;&emsp;closeStatusAddress|关门状态地址|integer(int32)||
|&emsp;&emsp;currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH|string||
|&emsp;&emsp;type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门|string||
|&emsp;&emsp;position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门|string||
|&emsp;&emsp;relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值|string||
|&emsp;&emsp;residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间|integer(int32)||
|&emsp;&emsp;lastCloseDoorTime|最后一次关门完成时间|string(date-time)||
|&emsp;&emsp;controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|backDoor|后门|AutoDoor|AutoDoor|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;ip|自动门ip|string||
|&emsp;&emsp;port|自动门端口|integer(int32)||
|&emsp;&emsp;openAddress|开门地址|integer(int32)||
|&emsp;&emsp;openStatusAddress|开门状态地址|integer(int32)||
|&emsp;&emsp;closeAddress|关门地址|integer(int32)||
|&emsp;&emsp;closeStatusAddress|关门状态地址|integer(int32)||
|&emsp;&emsp;currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH|string||
|&emsp;&emsp;type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门|string||
|&emsp;&emsp;position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门|string||
|&emsp;&emsp;relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值|string||
|&emsp;&emsp;residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间|integer(int32)||
|&emsp;&emsp;lastCloseDoorTime|最后一次关门完成时间|string(date-time)||
|&emsp;&emsp;controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||


**响应示例**:
```javascript
[
	{
		"frontDoor": {
			"id": "",
			"name": "",
			"ip": "",
			"port": 0,
			"openAddress": 0,
			"openStatusAddress": 0,
			"closeAddress": 0,
			"closeStatusAddress": 0,
			"currentStatus": "",
			"type": "",
			"position": "",
			"relationDoorId": "",
			"residenceTime": 0,
			"lastCloseDoorTime": "",
			"controlMode": "",
			"createTime": "",
			"updateTime": ""
		},
		"backDoor": {
			"id": "",
			"name": "",
			"ip": "",
			"port": 0,
			"openAddress": 0,
			"openStatusAddress": 0,
			"closeAddress": 0,
			"closeStatusAddress": 0,
			"currentStatus": "",
			"type": "",
			"position": "",
			"relationDoorId": "",
			"residenceTime": 0,
			"lastCloseDoorTime": "",
			"controlMode": "",
			"createTime": "",
			"updateTime": ""
		}
	}
]
```


## 风淋门分页查询


**接口地址**:`/api/v3/autoDoor/airShowerDoorPage`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«AirShowerDoor»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|AirShowerDoor|
|&emsp;&emsp;frontDoor|前门|AutoDoor|AutoDoor|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;&emsp;&emsp;ip|自动门ip||false|string||
|&emsp;&emsp;&emsp;&emsp;port|自动门端口||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;openAddress|开门地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;openStatusAddress|开门状态地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;closeAddress|关门地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;closeStatusAddress|关门状态地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH||false|string||
|&emsp;&emsp;&emsp;&emsp;type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门||false|string||
|&emsp;&emsp;&emsp;&emsp;position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门||false|string||
|&emsp;&emsp;&emsp;&emsp;relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值||false|string||
|&emsp;&emsp;&emsp;&emsp;residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;lastCloseDoorTime|最后一次关门完成时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|&emsp;&emsp;backDoor|后门|AutoDoor|AutoDoor|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;&emsp;&emsp;ip|自动门ip||false|string||
|&emsp;&emsp;&emsp;&emsp;port|自动门端口||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;openAddress|开门地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;openStatusAddress|开门状态地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;closeAddress|关门地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;closeStatusAddress|关门状态地址||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH||false|string||
|&emsp;&emsp;&emsp;&emsp;type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门||false|string||
|&emsp;&emsp;&emsp;&emsp;position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门||false|string||
|&emsp;&emsp;&emsp;&emsp;relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值||false|string||
|&emsp;&emsp;&emsp;&emsp;residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;lastCloseDoorTime|最后一次关门完成时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"frontDoor": {
				"id": "",
				"name": "",
				"ip": "",
				"port": 0,
				"openAddress": 0,
				"openStatusAddress": 0,
				"closeAddress": 0,
				"closeStatusAddress": 0,
				"currentStatus": "",
				"type": "",
				"position": "",
				"relationDoorId": "",
				"residenceTime": 0,
				"lastCloseDoorTime": "",
				"controlMode": "",
				"createTime": "",
				"updateTime": ""
			},
			"backDoor": {
				"id": "",
				"name": "",
				"ip": "",
				"port": 0,
				"openAddress": 0,
				"openStatusAddress": 0,
				"closeAddress": 0,
				"closeStatusAddress": 0,
				"currentStatus": "",
				"type": "",
				"position": "",
				"relationDoorId": "",
				"residenceTime": 0,
				"lastCloseDoorTime": "",
				"controlMode": "",
				"createTime": "",
				"updateTime": ""
			}
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 自动门列表


**接口地址**:`/api/v3/autoDoor/autoDoorAll`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AutoDoor|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|ip|自动门ip|string||
|port|自动门端口|integer(int32)|integer(int32)|
|openAddress|开门地址|integer(int32)|integer(int32)|
|openStatusAddress|开门状态地址|integer(int32)|integer(int32)|
|closeAddress|关门地址|integer(int32)|integer(int32)|
|closeStatusAddress|关门状态地址|integer(int32)|integer(int32)|
|currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH|string||
|type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门|string||
|position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门|string||
|relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值|string||
|residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间|integer(int32)|integer(int32)|
|lastCloseDoorTime|最后一次关门完成时间|string(date-time)|string(date-time)|
|controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"name": "",
		"ip": "",
		"port": 0,
		"openAddress": 0,
		"openStatusAddress": 0,
		"closeAddress": 0,
		"closeStatusAddress": 0,
		"currentStatus": "",
		"type": "",
		"position": "",
		"relationDoorId": "",
		"residenceTime": 0,
		"lastCloseDoorTime": "",
		"controlMode": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


## 自动门分页查询


**接口地址**:`/api/v3/autoDoor/autoDoorPage`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«AutoDoor»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|AutoDoor|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;ip|自动门ip|string||
|&emsp;&emsp;port|自动门端口|integer(int32)||
|&emsp;&emsp;openAddress|开门地址|integer(int32)||
|&emsp;&emsp;openStatusAddress|开门状态地址|integer(int32)||
|&emsp;&emsp;closeAddress|关门地址|integer(int32)||
|&emsp;&emsp;closeStatusAddress|关门状态地址|integer(int32)||
|&emsp;&emsp;currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH|string||
|&emsp;&emsp;type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门|string||
|&emsp;&emsp;position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门|string||
|&emsp;&emsp;relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值|string||
|&emsp;&emsp;residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间|integer(int32)||
|&emsp;&emsp;lastCloseDoorTime|最后一次关门完成时间|string(date-time)||
|&emsp;&emsp;controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"name": "",
			"ip": "",
			"port": 0,
			"openAddress": 0,
			"openStatusAddress": 0,
			"closeAddress": 0,
			"closeStatusAddress": 0,
			"currentStatus": "",
			"type": "",
			"position": "",
			"relationDoorId": "",
			"residenceTime": 0,
			"lastCloseDoorTime": "",
			"controlMode": "",
			"createTime": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 自动门详情


**接口地址**:`/api/v3/autoDoor/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|自动门id|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AutoDoor|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|ip|自动门ip|string||
|port|自动门端口|integer(int32)|integer(int32)|
|openAddress|开门地址|integer(int32)|integer(int32)|
|openStatusAddress|开门状态地址|integer(int32)|integer(int32)|
|closeAddress|关门地址|integer(int32)|integer(int32)|
|closeStatusAddress|关门状态地址|integer(int32)|integer(int32)|
|currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH|string||
|type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门|string||
|position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门|string||
|relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值|string||
|residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间|integer(int32)|integer(int32)|
|lastCloseDoorTime|最后一次关门完成时间|string(date-time)|string(date-time)|
|controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"ip": "",
	"port": 0,
	"openAddress": 0,
	"openStatusAddress": 0,
	"closeAddress": 0,
	"closeStatusAddress": 0,
	"currentStatus": "",
	"type": "",
	"position": "",
	"relationDoorId": "",
	"residenceTime": 0,
	"lastCloseDoorTime": "",
	"controlMode": "",
	"createTime": "",
	"updateTime": ""
}
```


## 删除自动门/风淋门


**接口地址**:`/api/v3/autoDoor/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|自动门ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 风淋门详情


**接口地址**:`/api/v3/autoDoor/{id}/airShowerDoor`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|前门或后门ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|AirShowerDoor|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|frontDoor|前门|AutoDoor|AutoDoor|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;ip|自动门ip|string||
|&emsp;&emsp;port|自动门端口|integer(int32)||
|&emsp;&emsp;openAddress|开门地址|integer(int32)||
|&emsp;&emsp;openStatusAddress|开门状态地址|integer(int32)||
|&emsp;&emsp;closeAddress|关门地址|integer(int32)||
|&emsp;&emsp;closeStatusAddress|关门状态地址|integer(int32)||
|&emsp;&emsp;currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH|string||
|&emsp;&emsp;type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门|string||
|&emsp;&emsp;position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门|string||
|&emsp;&emsp;relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值|string||
|&emsp;&emsp;residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间|integer(int32)||
|&emsp;&emsp;lastCloseDoorTime|最后一次关门完成时间|string(date-time)||
|&emsp;&emsp;controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|backDoor|后门|AutoDoor|AutoDoor|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;ip|自动门ip|string||
|&emsp;&emsp;port|自动门端口|integer(int32)||
|&emsp;&emsp;openAddress|开门地址|integer(int32)||
|&emsp;&emsp;openStatusAddress|开门状态地址|integer(int32)||
|&emsp;&emsp;closeAddress|关门地址|integer(int32)||
|&emsp;&emsp;closeStatusAddress|关门状态地址|integer(int32)||
|&emsp;&emsp;currentStatus|门已开:OPEN 门未开:NOT_OPEN 通讯异常:ERROR 未绑路径:UNBOUND_PATH|string||
|&emsp;&emsp;type|类型 AUTO_DOOR:自动门   AIR_SHOWER_DOOR:风淋门|string||
|&emsp;&emsp;position|位置 当type=AIR_SHOWER_DOOR时有值  FRONT:前门  BACK:后门|string||
|&emsp;&emsp;relationDoorId|关联门ID 当type=AIR_SHOWER_DOOR时有值|string||
|&emsp;&emsp;residenceTime|停留时间 单位:秒  机器人需要在两道风淋门间停留一段时间|integer(int32)||
|&emsp;&emsp;lastCloseDoorTime|最后一次关门完成时间|string(date-time)||
|&emsp;&emsp;controlMode|控制模式 LOCAL:本地控制 SCHEDULER:调度控制|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||


**响应示例**:
```javascript
{
	"frontDoor": {
		"id": "",
		"name": "",
		"ip": "",
		"port": 0,
		"openAddress": 0,
		"openStatusAddress": 0,
		"closeAddress": 0,
		"closeStatusAddress": 0,
		"currentStatus": "",
		"type": "",
		"position": "",
		"relationDoorId": "",
		"residenceTime": 0,
		"lastCloseDoorTime": "",
		"controlMode": "",
		"createTime": "",
		"updateTime": ""
	},
	"backDoor": {
		"id": "",
		"name": "",
		"ip": "",
		"port": 0,
		"openAddress": 0,
		"openStatusAddress": 0,
		"closeAddress": 0,
		"closeStatusAddress": 0,
		"currentStatus": "",
		"type": "",
		"position": "",
		"relationDoorId": "",
		"residenceTime": 0,
		"lastCloseDoorTime": "",
		"controlMode": "",
		"createTime": "",
		"updateTime": ""
	}
}
```


## 关门自动门/风淋门


**接口地址**:`/api/v3/autoDoor/{id}/close`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|自动门ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 开门自动门/风淋门


**接口地址**:`/api/v3/autoDoor/{id}/open`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|自动门ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 触发器


## 创建


**接口地址**:`/api/v3/triggerSelectors`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"buttonAddress": 0,
	"code": "",
	"completedTimes": 0,
	"createTime": "",
	"deviceAddress": 0,
	"executeTimes": 0,
	"id": "",
	"isDisabled": 0,
	"missionCode": "",
	"missionId": "",
	"missionName": "",
	"name": "",
	"pagerId": "",
	"period": 0,
	"sensorJson": "",
	"startTime": "",
	"startType": 0,
	"type": 0,
	"unit": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|triggerSelector|触发器对象|body|true|TriggerSelector|TriggerSelector|
|&emsp;&emsp;buttonAddress|按钮地址||false|integer(int32)||
|&emsp;&emsp;code|编码||false|string||
|&emsp;&emsp;completedTimes|已经完成次数||false|integer(int32)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;deviceAddress|设备地址||false|integer(int32)||
|&emsp;&emsp;executeTimes|执行次数||false|integer(int32)||
|&emsp;&emsp;id|主键ID||false|string||
|&emsp;&emsp;isDisabled|是否禁用,0:启用、1:禁用||false|integer(int32)||
|&emsp;&emsp;missionCode|触发器关联的任务编码||false|string||
|&emsp;&emsp;missionId|任务ID||false|string||
|&emsp;&emsp;missionName|触发器关联的任务名称||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;pagerId|呼叫器ID||false|string||
|&emsp;&emsp;period|触发间隔||false|integer(int64)||
|&emsp;&emsp;sensorJson|传感器JSON [{"sensorId":"xxxx","value":1}]||false|string||
|&emsp;&emsp;startTime|开始时间||false|string(date-time)||
|&emsp;&emsp;startType|开始类型;1:即时、2:定时||false|integer(int32)||
|&emsp;&emsp;type|触发类型;1:定时触发、2呼叫器触发、3传感器触发||false|integer(int32)||
|&emsp;&emsp;unit|触发间隔的时间单位;SECOND、DAY、WEEK、MONTH||false|string||
|&emsp;&emsp;updateTime|修改时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 分页查询


**接口地址**:`/api/v3/triggerSelectors/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||
|code|触发器编号|query|false|string||
|searchMap|searchMap|query|false||object|
|type|类型:1:定时触发、2呼叫器触发、3传感器触发|query|false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«TriggerSelector»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|TriggerSelector|
|&emsp;&emsp;buttonAddress|按钮地址|integer(int32)||
|&emsp;&emsp;code|编码|string||
|&emsp;&emsp;completedTimes|已经完成次数|integer(int32)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;deviceAddress|设备地址|integer(int32)||
|&emsp;&emsp;executeTimes|执行次数|integer(int32)||
|&emsp;&emsp;id|主键ID|string||
|&emsp;&emsp;isDisabled|是否禁用,0:启用、1:禁用|integer(int32)||
|&emsp;&emsp;missionCode|触发器关联的任务编码|string||
|&emsp;&emsp;missionId|任务ID|string||
|&emsp;&emsp;missionName|触发器关联的任务名称|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;pagerId|呼叫器ID|string||
|&emsp;&emsp;period|触发间隔|integer(int64)||
|&emsp;&emsp;sensorJson|传感器JSON [{"sensorId":"xxxx","value":1}]|string||
|&emsp;&emsp;startTime|开始时间|string(date-time)||
|&emsp;&emsp;startType|开始类型;1:即时、2:定时|integer(int32)||
|&emsp;&emsp;type|触发类型;1:定时触发、2呼叫器触发、3传感器触发|integer(int32)||
|&emsp;&emsp;unit|触发间隔的时间单位;SECOND、DAY、WEEK、MONTH|string||
|&emsp;&emsp;updateTime|修改时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"buttonAddress": 0,
			"code": "",
			"completedTimes": 0,
			"createTime": "",
			"deviceAddress": 0,
			"executeTimes": 0,
			"id": "",
			"isDisabled": 0,
			"missionCode": "",
			"missionId": "",
			"missionName": "",
			"name": "",
			"pagerId": "",
			"period": 0,
			"sensorJson": "",
			"startTime": "",
			"startType": 0,
			"type": 0,
			"unit": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 触发器详情


**接口地址**:`/api/v3/triggerSelectors/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|TriggerSelector|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|buttonAddress|按钮地址|integer(int32)|integer(int32)|
|code|编码|string||
|completedTimes|已经完成次数|integer(int32)|integer(int32)|
|createTime|创建时间|string(date-time)|string(date-time)|
|deviceAddress|设备地址|integer(int32)|integer(int32)|
|executeTimes|执行次数|integer(int32)|integer(int32)|
|id|主键ID|string||
|isDisabled|是否禁用,0:启用、1:禁用|integer(int32)|integer(int32)|
|missionCode|触发器关联的任务编码|string||
|missionId|任务ID|string||
|missionName|触发器关联的任务名称|string||
|name|名称|string||
|pagerId|呼叫器ID|string||
|period|触发间隔|integer(int64)|integer(int64)|
|sensorJson|传感器JSON [{"sensorId":"xxxx","value":1}]|string||
|startTime|开始时间|string(date-time)|string(date-time)|
|startType|开始类型;1:即时、2:定时|integer(int32)|integer(int32)|
|type|触发类型;1:定时触发、2呼叫器触发、3传感器触发|integer(int32)|integer(int32)|
|unit|触发间隔的时间单位;SECOND、DAY、WEEK、MONTH|string||
|updateTime|修改时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"buttonAddress": 0,
	"code": "",
	"completedTimes": 0,
	"createTime": "",
	"deviceAddress": 0,
	"executeTimes": 0,
	"id": "",
	"isDisabled": 0,
	"missionCode": "",
	"missionId": "",
	"missionName": "",
	"name": "",
	"pagerId": "",
	"period": 0,
	"sensorJson": "",
	"startTime": "",
	"startType": 0,
	"type": 0,
	"unit": "",
	"updateTime": ""
}
```


## 修改


**接口地址**:`/api/v3/triggerSelectors/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"buttonAddress": 0,
	"code": "",
	"completedTimes": 0,
	"createTime": "",
	"deviceAddress": 0,
	"executeTimes": 0,
	"id": "",
	"isDisabled": 0,
	"missionCode": "",
	"missionId": "",
	"missionName": "",
	"name": "",
	"pagerId": "",
	"period": 0,
	"sensorJson": "",
	"startTime": "",
	"startType": 0,
	"type": 0,
	"unit": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|触发器ID|path|true|string||
|triggerSelector|触发器对象|body|true|TriggerSelector|TriggerSelector|
|&emsp;&emsp;buttonAddress|按钮地址||false|integer(int32)||
|&emsp;&emsp;code|编码||false|string||
|&emsp;&emsp;completedTimes|已经完成次数||false|integer(int32)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;deviceAddress|设备地址||false|integer(int32)||
|&emsp;&emsp;executeTimes|执行次数||false|integer(int32)||
|&emsp;&emsp;id|主键ID||false|string||
|&emsp;&emsp;isDisabled|是否禁用,0:启用、1:禁用||false|integer(int32)||
|&emsp;&emsp;missionCode|触发器关联的任务编码||false|string||
|&emsp;&emsp;missionId|任务ID||false|string||
|&emsp;&emsp;missionName|触发器关联的任务名称||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;pagerId|呼叫器ID||false|string||
|&emsp;&emsp;period|触发间隔||false|integer(int64)||
|&emsp;&emsp;sensorJson|传感器JSON [{"sensorId":"xxxx","value":1}]||false|string||
|&emsp;&emsp;startTime|开始时间||false|string(date-time)||
|&emsp;&emsp;startType|开始类型;1:即时、2:定时||false|integer(int32)||
|&emsp;&emsp;type|触发类型;1:定时触发、2呼叫器触发、3传感器触发||false|integer(int32)||
|&emsp;&emsp;unit|触发间隔的时间单位;SECOND、DAY、WEEK、MONTH||false|string||
|&emsp;&emsp;updateTime|修改时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 删除


**接口地址**:`/api/v3/triggerSelectors/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 检索触发器下的所有任务记录


**接口地址**:`/api/v3/triggerSelectors/{id}/missionWorks`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|path|true|string||
|searchMap|searchMap|query|false||object|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|TriggerSelectorDetailVO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|alreadyTrigger|已触发|integer(int32)|integer(int32)|
|cancel|已取消|integer(int32)|integer(int32)|
|completed|已完成|integer(int32)|integer(int32)|
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|MissionWork|
|&emsp;&emsp;currentActionName|指令名称|string||
|&emsp;&emsp;currentActionSequence|指令序号|integer(int32)||
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;releaseButtonAddress||integer(int32)||
|&emsp;&emsp;releaseDeviceAddress||integer(int32)||
|&emsp;&emsp;releaseSuccess||boolean||
|&emsp;&emsp;code|任务编码|string||
|&emsp;&emsp;missionCallId|预设任务ID|string||
|&emsp;&emsp;missionId|预设任务ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;schedulePlanId|调度计划的ID|string||
|&emsp;&emsp;callbackUrl|回调接口|string||
|&emsp;&emsp;sequence|优先级: 1、低  2、普通  3、高  4、最高  默认是2|integer(int32)||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;status|状态 CREATE:创建(未执行) START:开始执行 WAIT:等待(继续)执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 PAUSE:暂停 BEING_PAUSE:暂停中 BEING_RESUME:恢复中 SHUTDOWN:已停止 BEING_SHUTDOWN:停止中 WAITINPUT:等待输入|string||
|&emsp;&emsp;message|异常信息|string||
|&emsp;&emsp;interrupt|是否可中断|boolean||
|&emsp;&emsp;runtimeParam|运行时参数(json格式) 如：{"marker1":"1001"}|string||
|&emsp;&emsp;missionWorkChainId|任务链ID|string||
|&emsp;&emsp;allocationStatus|分配状态 已分配：ASSIGNED  未分配：UNASSIGNED|string||
|&emsp;&emsp;totalMileage|任务总里程 单位 米|number(double)||
|&emsp;&emsp;errorCode|异常错误代码|integer(int32)||
|&emsp;&emsp;startTime|开始时间|string(date-time)||
|&emsp;&emsp;endTime|结束时间|string(date-time)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;agvCode|机器人编码|string||
|&emsp;&emsp;triggerSelectorId|触发器ID|string||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|&emsp;&emsp;createdBy|创建者 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|running|执行中|integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"alreadyTrigger": 0,
	"cancel": 0,
	"completed": 0,
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"currentActionName": "",
			"currentActionSequence": 0,
			"id": "",
			"releaseButtonAddress": 0,
			"releaseDeviceAddress": 0,
			"releaseSuccess": true,
			"code": "",
			"missionCallId": "",
			"missionId": "",
			"name": "",
			"schedulePlanId": "",
			"callbackUrl": "",
			"sequence": 0,
			"description": "",
			"status": "",
			"message": "",
			"interrupt": true,
			"runtimeParam": "",
			"missionWorkChainId": "",
			"allocationStatus": "",
			"totalMileage": 0,
			"errorCode": 0,
			"startTime": "",
			"endTime": "",
			"createTime": "",
			"agvCode": "",
			"triggerSelectorId": "",
			"updateTime": "",
			"createdBy": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"running": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


# 证书上传


## 获取证书信息


**接口地址**:`/api/v3/license`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|LicenseDto|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|startTime|生效开始时间|string(date-time)|string(date-time)|
|endTime|生效结束时间|string(date-time)|string(date-time)|
|serverType|服务类型: YOUIFleet/YOUIDrive/YOUIINS/YOUITMS/YOUICompass|string||
|companyName|公司名称|string||
|fileId|文件id/文件名称|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|
|type|0已过期，1生效中，2未生效|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"id": "",
	"startTime": "",
	"endTime": "",
	"serverType": "",
	"companyName": "",
	"fileId": "",
	"createTime": "",
	"updateTime": "",
	"type": 0
}
```


## 删除获取证书信息


**接口地址**:`/api/v3/license`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 上传license文件


**接口地址**:`/api/v3/license/valiadateLicense`


**请求方式**:`POST`


**请求数据类型**:`multipart/form-data`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|mutiPartFile|文件|formData|true|ref||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|LicenseDto|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|startTime|生效开始时间|string(date-time)|string(date-time)|
|endTime|生效结束时间|string(date-time)|string(date-time)|
|serverType|服务类型: YOUIFleet/YOUIDrive/YOUIINS/YOUITMS/YOUICompass|string||
|companyName|公司名称|string||
|fileId|文件id/文件名称|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|
|type|0已过期，1生效中，2未生效|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"id": "",
	"startTime": "",
	"endTime": "",
	"serverType": "",
	"companyName": "",
	"fileId": "",
	"createTime": "",
	"updateTime": "",
	"type": 0
}
```


# 调度计划


## 列表


**接口地址**:`/api/v3/schedulingPlans`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|SchedulePlan|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|任务ID|string||
|name|调度计划名称|string||
|cron|cron表达式|string||
|frequency|执行次数|integer(int32)|integer(int32)|
|executeInterval|执行间隔|integer(int32)|integer(int32)|
|completeFrequency|已经完成次数|integer(int32)|integer(int32)|
|description|描述|string||
|status|状态|string||
|callbackUrl|回调接口|string||
|executeOverCreateNew|是否执行完创建|boolean||
|executeTime|初次执行时间|string(date-time)|string(date-time)|
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"missionId": "",
		"name": "",
		"cron": "",
		"frequency": 0,
		"executeInterval": 0,
		"completeFrequency": 0,
		"description": "",
		"status": "",
		"callbackUrl": "",
		"executeOverCreateNew": true,
		"executeTime": "",
		"startTime": "",
		"endTime": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


## 创建


**接口地址**:`/api/v3/schedulingPlans`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"missionId": "",
	"name": "",
	"cron": "",
	"frequency": 0,
	"executeInterval": 0,
	"completeFrequency": 0,
	"description": "",
	"status": "",
	"callbackUrl": "",
	"executeOverCreateNew": true,
	"executeTime": "",
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schedulePlan|调度计划|body|true|SchedulePlan|SchedulePlan|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;missionId|任务ID||false|string||
|&emsp;&emsp;name|调度计划名称||false|string||
|&emsp;&emsp;cron|cron表达式||false|string||
|&emsp;&emsp;frequency|执行次数||false|integer(int32)||
|&emsp;&emsp;executeInterval|执行间隔||false|integer(int32)||
|&emsp;&emsp;completeFrequency|已经完成次数||false|integer(int32)||
|&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;status|状态||false|string||
|&emsp;&emsp;callbackUrl|回调接口||false|string||
|&emsp;&emsp;executeOverCreateNew|是否执行完创建||false|boolean||
|&emsp;&emsp;executeTime|初次执行时间||false|string(date-time)||
|&emsp;&emsp;startTime|开始时间||false|string(date-time)||
|&emsp;&emsp;endTime|结束时间||false|string(date-time)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|SchedulePlan|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|任务ID|string||
|name|调度计划名称|string||
|cron|cron表达式|string||
|frequency|执行次数|integer(int32)|integer(int32)|
|executeInterval|执行间隔|integer(int32)|integer(int32)|
|completeFrequency|已经完成次数|integer(int32)|integer(int32)|
|description|描述|string||
|status|状态|string||
|callbackUrl|回调接口|string||
|executeOverCreateNew|是否执行完创建|boolean||
|executeTime|初次执行时间|string(date-time)|string(date-time)|
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"missionId": "",
	"name": "",
	"cron": "",
	"frequency": 0,
	"executeInterval": 0,
	"completeFrequency": 0,
	"description": "",
	"status": "",
	"callbackUrl": "",
	"executeOverCreateNew": true,
	"executeTime": "",
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"updateTime": ""
}
```


## 分页查询


**接口地址**:`/api/v3/schedulingPlans/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«SchedulePlan»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|SchedulePlan|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;missionId|任务ID|string||
|&emsp;&emsp;name|调度计划名称|string||
|&emsp;&emsp;cron|cron表达式|string||
|&emsp;&emsp;frequency|执行次数|integer(int32)||
|&emsp;&emsp;executeInterval|执行间隔|integer(int32)||
|&emsp;&emsp;completeFrequency|已经完成次数|integer(int32)||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;status|状态|string||
|&emsp;&emsp;callbackUrl|回调接口|string||
|&emsp;&emsp;executeOverCreateNew|是否执行完创建|boolean||
|&emsp;&emsp;executeTime|初次执行时间|string(date-time)||
|&emsp;&emsp;startTime|开始时间|string(date-time)||
|&emsp;&emsp;endTime|结束时间|string(date-time)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"missionId": "",
			"name": "",
			"cron": "",
			"frequency": 0,
			"executeInterval": 0,
			"completeFrequency": 0,
			"description": "",
			"status": "",
			"callbackUrl": "",
			"executeOverCreateNew": true,
			"executeTime": "",
			"startTime": "",
			"endTime": "",
			"createTime": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/schedulingPlans/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|调度计划ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|SchedulePlan|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|任务ID|string||
|name|调度计划名称|string||
|cron|cron表达式|string||
|frequency|执行次数|integer(int32)|integer(int32)|
|executeInterval|执行间隔|integer(int32)|integer(int32)|
|completeFrequency|已经完成次数|integer(int32)|integer(int32)|
|description|描述|string||
|status|状态|string||
|callbackUrl|回调接口|string||
|executeOverCreateNew|是否执行完创建|boolean||
|executeTime|初次执行时间|string(date-time)|string(date-time)|
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"missionId": "",
	"name": "",
	"cron": "",
	"frequency": 0,
	"executeInterval": 0,
	"completeFrequency": 0,
	"description": "",
	"status": "",
	"callbackUrl": "",
	"executeOverCreateNew": true,
	"executeTime": "",
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"updateTime": ""
}
```


## 更新


**接口地址**:`/api/v3/schedulingPlans/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"missionId": "",
	"name": "",
	"cron": "",
	"frequency": 0,
	"executeInterval": 0,
	"completeFrequency": 0,
	"description": "",
	"status": "",
	"callbackUrl": "",
	"executeOverCreateNew": true,
	"executeTime": "",
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|调度计划ID|path|true|string||
|schedulePlan|调度计划|body|true|SchedulePlan|SchedulePlan|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;missionId|任务ID||false|string||
|&emsp;&emsp;name|调度计划名称||false|string||
|&emsp;&emsp;cron|cron表达式||false|string||
|&emsp;&emsp;frequency|执行次数||false|integer(int32)||
|&emsp;&emsp;executeInterval|执行间隔||false|integer(int32)||
|&emsp;&emsp;completeFrequency|已经完成次数||false|integer(int32)||
|&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;status|状态||false|string||
|&emsp;&emsp;callbackUrl|回调接口||false|string||
|&emsp;&emsp;executeOverCreateNew|是否执行完创建||false|boolean||
|&emsp;&emsp;executeTime|初次执行时间||false|string(date-time)||
|&emsp;&emsp;startTime|开始时间||false|string(date-time)||
|&emsp;&emsp;endTime|结束时间||false|string(date-time)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|SchedulePlan|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|任务ID|string||
|name|调度计划名称|string||
|cron|cron表达式|string||
|frequency|执行次数|integer(int32)|integer(int32)|
|executeInterval|执行间隔|integer(int32)|integer(int32)|
|completeFrequency|已经完成次数|integer(int32)|integer(int32)|
|description|描述|string||
|status|状态|string||
|callbackUrl|回调接口|string||
|executeOverCreateNew|是否执行完创建|boolean||
|executeTime|初次执行时间|string(date-time)|string(date-time)|
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"missionId": "",
	"name": "",
	"cron": "",
	"frequency": 0,
	"executeInterval": 0,
	"completeFrequency": 0,
	"description": "",
	"status": "",
	"callbackUrl": "",
	"executeOverCreateNew": true,
	"executeTime": "",
	"startTime": "",
	"endTime": "",
	"createTime": "",
	"updateTime": ""
}
```


## 删除


**接口地址**:`/api/v3/schedulingPlans/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|调度计划ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 暂停


**接口地址**:`/api/v3/schedulingPlans/{id}/controls/pause`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|调度计划ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 恢复


**接口地址**:`/api/v3/schedulingPlans/{id}/controls/resume`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|调度计划ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 停止


**接口地址**:`/api/v3/schedulingPlans/{id}/controls/shutDown`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|调度计划ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 根据调度ID查询工作列表


**接口地址**:`/api/v3/schedulingPlans/{id}/missionWorks`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|调度计划ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionWork|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|currentActionName|指令名称|string||
|currentActionSequence|指令序号|integer(int32)|integer(int32)|
|id|ID|string||
|releaseButtonAddress||integer(int32)|integer(int32)|
|releaseDeviceAddress||integer(int32)|integer(int32)|
|releaseSuccess||boolean||
|code|任务编码|string||
|missionCallId|预设任务ID|string||
|missionId|预设任务ID|string||
|name|名称|string||
|schedulePlanId|调度计划的ID|string||
|callbackUrl|回调接口|string||
|sequence|优先级: 1、低  2、普通  3、高  4、最高  默认是2|integer(int32)|integer(int32)|
|description|描述|string||
|status|状态 CREATE:创建(未执行) START:开始执行 WAIT:等待(继续)执行 RUNNING:执行中 SUCCESS:执行成功 FAULT:执行错误 PAUSE:暂停 BEING_PAUSE:暂停中 BEING_RESUME:恢复中 SHUTDOWN:已停止 BEING_SHUTDOWN:停止中 WAITINPUT:等待输入|string||
|message|异常信息|string||
|interrupt|是否可中断|boolean||
|runtimeParam|运行时参数(json格式) 如：{"marker1":"1001"}|string||
|missionWorkChainId|任务链ID|string||
|allocationStatus|分配状态 已分配：ASSIGNED  未分配：UNASSIGNED|string||
|totalMileage|任务总里程 单位 米|number(double)|number(double)|
|errorCode|异常错误代码|integer(int32)|integer(int32)|
|startTime|开始时间|string(date-time)|string(date-time)|
|endTime|结束时间|string(date-time)|string(date-time)|
|createTime|创建时间|string(date-time)|string(date-time)|
|agvCode|机器人编码|string||
|triggerSelectorId|触发器ID|string||
|updateTime|更新时间|string(date-time)|string(date-time)|
|createdBy|创建者 多机：YOUIFleet 单机：YOUICompass 默认是YOUICompass|string||


**响应示例**:
```javascript
[
	{
		"currentActionName": "",
		"currentActionSequence": 0,
		"id": "",
		"releaseButtonAddress": 0,
		"releaseDeviceAddress": 0,
		"releaseSuccess": true,
		"code": "",
		"missionCallId": "",
		"missionId": "",
		"name": "",
		"schedulePlanId": "",
		"callbackUrl": "",
		"sequence": 0,
		"description": "",
		"status": "",
		"message": "",
		"interrupt": true,
		"runtimeParam": "",
		"missionWorkChainId": "",
		"allocationStatus": "",
		"totalMileage": 0,
		"errorCode": 0,
		"startTime": "",
		"endTime": "",
		"createTime": "",
		"agvCode": "",
		"triggerSelectorId": "",
		"updateTime": "",
		"createdBy": ""
	}
]
```


# 调整动作


## 调整点列表


**接口地址**:`/api/v3/adjustAction`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|isDraft|是否草稿目录：true、false|query|true|boolean||
|mapName|地图名称||true|String|String|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|adjust_action|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|markerId|关联标记点id|string||
|destMarkerId|目标标记点id|string||
|agvMapId|地图id|string||
|agvRotateAngle|机器人旋转角度|number(double)|number(double)|
|shelvesRotateAngle|货架旋转角度|number(double)|number(double)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"markerId": "",
		"destMarkerId": "",
		"agvMapId": "",
		"agvRotateAngle": 0,
		"shelvesRotateAngle": 0,
		"createTime": "",
		"updateTime": ""
	}
]
```


## 创建


**接口地址**:`/api/v3/adjustAction`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|adjustAction|调整动作|body|true|AdjustAction|AdjustAction|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|adjust_action|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|markerId|关联标记点id|string||
|destMarkerId|目标标记点id|string||
|agvMapId|地图id|string||
|agvRotateAngle|机器人旋转角度|number(double)|number(double)|
|shelvesRotateAngle|货架旋转角度|number(double)|number(double)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"markerId": "",
	"destMarkerId": "",
	"agvMapId": "",
	"agvRotateAngle": 0,
	"shelvesRotateAngle": 0,
	"createTime": "",
	"updateTime": ""
}
```


## 详情


**接口地址**:`/api/v3/adjustAction/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|调整动作主键id|path|true|string||
|isDraft|是否查询草稿数据|query|true|boolean||
|mapName|地图名称|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|adjust_action|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|markerId|关联标记点id|string||
|destMarkerId|目标标记点id|string||
|agvMapId|地图id|string||
|agvRotateAngle|机器人旋转角度|number(double)|number(double)|
|shelvesRotateAngle|货架旋转角度|number(double)|number(double)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"markerId": "",
	"destMarkerId": "",
	"agvMapId": "",
	"agvRotateAngle": 0,
	"shelvesRotateAngle": 0,
	"createTime": "",
	"updateTime": ""
}
```


## 更新


**接口地址**:`/api/v3/adjustAction/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|adjustAction|标记点|body|true|AdjustAction|AdjustAction|
|id|调整动作主键id|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|adjust_action|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|markerId|关联标记点id|string||
|destMarkerId|目标标记点id|string||
|agvMapId|地图id|string||
|agvRotateAngle|机器人旋转角度|number(double)|number(double)|
|shelvesRotateAngle|货架旋转角度|number(double)|number(double)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"markerId": "",
	"destMarkerId": "",
	"agvMapId": "",
	"agvRotateAngle": 0,
	"shelvesRotateAngle": 0,
	"createTime": "",
	"updateTime": ""
}
```


## 删除


**接口地址**:`/api/v3/adjustAction/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|调整动作主键id|path|true|string||
|mapName|地图名称|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 路径


## 列表


**接口地址**:`/api/v3/paths`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|isDraft|是否查询草稿数据|query|true|boolean||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|pathVo|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|weightRatio|路径权重系数|number(double)|number(double)|
|path|路径|Path|Path|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;agvMapName|地图ID|string||
|&emsp;&emsp;startMarkerId|开始标记点|string||
|&emsp;&emsp;endMarkerId|结束标记点|string||
|&emsp;&emsp;startControl|开始点的控制点xy坐标|string||
|&emsp;&emsp;endControl|结束点的控制点xy坐标|string||
|&emsp;&emsp;length|长度|number(double)||
|&emsp;&emsp;lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）|integer(int32)||
|&emsp;&emsp;direction|方向 0、双向 1、正向 2、反向|integer(int32)||
|&emsp;&emsp;forwardAgvDirection|正向行驶时agv方向 1、正向 2、反向|integer(int32)||
|&emsp;&emsp;reverseAgvDirection|反向行驶时agv方向 1、正向 2、反向|integer(int32)||
|&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|&emsp;&emsp;autoDoorId|自动门ID|string||
|sidePathVos|sidePath数据|array|pathVo|
|&emsp;&emsp;weightRatio|路径权重系数|number(double)||
|&emsp;&emsp;path|路径|Path|Path|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;agvMapName|地图ID||false|string||
|&emsp;&emsp;&emsp;&emsp;startMarkerId|开始标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;endMarkerId|结束标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;startControl|开始点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;endControl|结束点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;length|长度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;direction|方向 0、双向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;forwardAgvDirection|正向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;reverseAgvDirection|反向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;&emsp;&emsp;autoDoorId|自动门ID||false|string||
|&emsp;&emsp;sidePathVos|sidePath数据|array|pathVo|
|&emsp;&emsp;&emsp;&emsp;weightRatio|路径权重系数||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;path|路径||false|Path|Path|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;agvMapName|地图ID||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;startMarkerId|开始标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;endMarkerId|结束标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;startControl|开始点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;endControl|结束点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;length|长度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;direction|方向 0、双向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;forwardAgvDirection|正向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;reverseAgvDirection|反向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;autoDoorId|自动门ID||false|string||
|&emsp;&emsp;&emsp;&emsp;sidePathVos|sidePath数据||false|array|pathVo|
|&emsp;&emsp;&emsp;&emsp;startMarkerId|开始标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;endMarkerId|结束标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;agvDirection|agv方向: 0、双向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;directionAgv|AGV要朝向的角度（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;directionAgv2|AGV要朝向的角度2（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;directionShelf|货架要朝向的角度（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;pathType|路径类型: 0、普通路径 1、二维码对接路径 2、脱离对接路径||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;rpmShelf|uint, 货架旋转速度，单位，转/每分钟||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;workStationCode|工位编码||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;directionShelf2|货架要朝向的角度2（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;position|位置，1、起始点 2、结束点||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;effectivePath|生效路径 1、全部路径 2、第一段路径||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;hasAction|是否有动作,1、有 0、没有||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;pathParam|路径导航参数||false|PathParam|PathParam|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;safety_scanner_region|雷达避障区域 0、默认区域||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;safety|避障 1、打开避障  2、关闭避障||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;max_translation_speed|最大平移速度 >0 m/s||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;max_rotate_speed|最大旋转速度 rad/s >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;P|平移加速比例控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;D|平移加速微分控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;translation_acc|平移加（减）速度 m/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rotate_acc|旋转加（减）速度 rad/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;updateTime|修改时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;extend_bit|拓展布尔||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;extend_string|拓展字符串||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;features_requested|融合特征 1、开启 0、关闭||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;agvDirection2|agv方向2: -180 ~ 180||false|integer(int32)||
|&emsp;&emsp;startMarkerId|开始标记点|string||
|&emsp;&emsp;endMarkerId|结束标记点|string||
|&emsp;&emsp;agvDirection|agv方向: 0、双向 1、正向 2、反向|integer(int32)||
|&emsp;&emsp;directionAgv|AGV要朝向的角度（地图坐标系下）  -180 ~ 180|number(double)||
|&emsp;&emsp;directionAgv2|AGV要朝向的角度2（地图坐标系下）  -180 ~ 180|number(double)||
|&emsp;&emsp;directionShelf|货架要朝向的角度（地图坐标系下）  -180 ~ 180|number(double)||
|&emsp;&emsp;pathType|路径类型: 0、普通路径 1、二维码对接路径 2、脱离对接路径|integer(int32)||
|&emsp;&emsp;rpmShelf|uint, 货架旋转速度，单位，转/每分钟|integer(int32)||
|&emsp;&emsp;workStationCode|工位编码|integer(int32)||
|&emsp;&emsp;directionShelf2|货架要朝向的角度2（地图坐标系下）  -180 ~ 180|number(double)||
|&emsp;&emsp;position|位置，1、起始点 2、结束点|integer(int32)||
|&emsp;&emsp;effectivePath|生效路径 1、全部路径 2、第一段路径|integer(int32)||
|&emsp;&emsp;hasAction|是否有动作,1、有 0、没有|integer(int32)||
|&emsp;&emsp;pathParam|路径导航参数|PathParam|PathParam|
|&emsp;&emsp;&emsp;&emsp;safety_scanner_region|雷达避障区域 0、默认区域||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;safety|避障 1、打开避障  2、关闭避障||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;max_translation_speed|最大平移速度 >0 m/s||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;max_rotate_speed|最大旋转速度 rad/s >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;P|平移加速比例控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;D|平移加速微分控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;translation_acc|平移加（减）速度 m/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;rotate_acc|旋转加（减）速度 rad/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;updateTime|修改时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;extend_bit|拓展布尔||false|string||
|&emsp;&emsp;&emsp;&emsp;extend_string|拓展字符串||false|string||
|&emsp;&emsp;&emsp;&emsp;features_requested|融合特征 1、开启 0、关闭||false|integer(int32)||
|&emsp;&emsp;agvDirection2|agv方向2: -180 ~ 180|integer(int32)||
|startMarkerId|开始标记点|string||
|endMarkerId|结束标记点|string||
|agvDirection|agv方向: 0、双向 1、正向 2、反向|integer(int32)|integer(int32)|
|directionAgv|AGV要朝向的角度（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|directionAgv2|AGV要朝向的角度2（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|directionShelf|货架要朝向的角度（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|pathType|路径类型: 0、普通路径 1、二维码对接路径 2、脱离对接路径|integer(int32)|integer(int32)|
|rpmShelf|uint, 货架旋转速度，单位，转/每分钟|integer(int32)|integer(int32)|
|workStationCode|工位编码|integer(int32)|integer(int32)|
|directionShelf2|货架要朝向的角度2（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|position|位置，1、起始点 2、结束点|integer(int32)|integer(int32)|
|effectivePath|生效路径 1、全部路径 2、第一段路径|integer(int32)|integer(int32)|
|hasAction|是否有动作,1、有 0、没有|integer(int32)|integer(int32)|
|pathParam|路径导航参数|PathParam|PathParam|
|&emsp;&emsp;safety_scanner_region|雷达避障区域 0、默认区域|integer(int32)||
|&emsp;&emsp;safety|避障 1、打开避障  2、关闭避障|integer(int32)||
|&emsp;&emsp;max_translation_speed|最大平移速度 >0 m/s|number(double)||
|&emsp;&emsp;max_rotate_speed|最大旋转速度 rad/s >0|number(double)||
|&emsp;&emsp;P|平移加速比例控制系数 >0|number(double)||
|&emsp;&emsp;D|平移加速微分控制系数 >0|number(double)||
|&emsp;&emsp;translation_acc|平移加（减）速度 m/s2 >0|number(double)||
|&emsp;&emsp;rotate_acc|旋转加（减）速度 rad/s2 >0|number(double)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|修改时间|string(date-time)||
|&emsp;&emsp;extend_bit|拓展布尔|string||
|&emsp;&emsp;extend_string|拓展字符串|string||
|&emsp;&emsp;features_requested|融合特征 1、开启 0、关闭|integer(int32)||
|agvDirection2|agv方向2: -180 ~ 180|integer(int32)|integer(int32)|


**响应示例**:
```javascript
[
	{
		"weightRatio": 0,
		"path": {
			"id": "",
			"agvMapName": "",
			"startMarkerId": "",
			"endMarkerId": "",
			"startControl": "",
			"endControl": "",
			"length": 0,
			"lineType": 0,
			"direction": 0,
			"forwardAgvDirection": 0,
			"reverseAgvDirection": 0,
			"usageStatus": "",
			"autoDoorId": ""
		},
		"sidePathVos": [
			{
				"weightRatio": 0,
				"path": "",
				"sidePathVos": [],
				"startMarkerId": "",
				"endMarkerId": "",
				"agvDirection": 0,
				"directionAgv": 0,
				"directionAgv2": 0,
				"directionShelf": 0,
				"pathType": 0,
				"rpmShelf": 0,
				"workStationCode": 0,
				"directionShelf2": 0,
				"position": 0,
				"effectivePath": 0,
				"hasAction": 0,
				"pathParam": "",
				"agvDirection2": 0
			}
		],
		"startMarkerId": "",
		"endMarkerId": "",
		"agvDirection": 0,
		"directionAgv": 0,
		"directionAgv2": 0,
		"directionShelf": 0,
		"pathType": 0,
		"rpmShelf": 0,
		"workStationCode": 0,
		"directionShelf2": 0,
		"position": 0,
		"effectivePath": 0,
		"hasAction": 0,
		"pathParam": {
			"safety_scanner_region": 0,
			"safety": 0,
			"max_translation_speed": 0,
			"max_rotate_speed": 0,
			"P": 0,
			"D": 0,
			"translation_acc": 0,
			"rotate_acc": 0,
			"createTime": "",
			"updateTime": "",
			"extend_bit": "",
			"extend_string": "",
			"features_requested": 0
		},
		"agvDirection2": 0
	}
]
```


## 创建


**接口地址**:`/api/v3/paths`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"agvMapName": "",
	"startMarkerId": "",
	"endMarkerId": "",
	"startControl": "",
	"endControl": "",
	"length": 0,
	"lineType": 0,
	"direction": 0,
	"forwardAgvDirection": 0,
	"reverseAgvDirection": 0,
	"usageStatus": "",
	"autoDoorId": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|path|路径|body|true|Path|Path|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;agvMapName|地图ID||false|string||
|&emsp;&emsp;startMarkerId|开始标记点||false|string||
|&emsp;&emsp;endMarkerId|结束标记点||false|string||
|&emsp;&emsp;startControl|开始点的控制点xy坐标||false|string||
|&emsp;&emsp;endControl|结束点的控制点xy坐标||false|string||
|&emsp;&emsp;length|长度||false|number(double)||
|&emsp;&emsp;lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）||false|integer(int32)||
|&emsp;&emsp;direction|方向 0、双向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;forwardAgvDirection|正向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;reverseAgvDirection|反向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;autoDoorId|自动门ID||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|pathVo|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|weightRatio|路径权重系数|number(double)|number(double)|
|path|路径|Path|Path|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;agvMapName|地图ID|string||
|&emsp;&emsp;startMarkerId|开始标记点|string||
|&emsp;&emsp;endMarkerId|结束标记点|string||
|&emsp;&emsp;startControl|开始点的控制点xy坐标|string||
|&emsp;&emsp;endControl|结束点的控制点xy坐标|string||
|&emsp;&emsp;length|长度|number(double)||
|&emsp;&emsp;lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）|integer(int32)||
|&emsp;&emsp;direction|方向 0、双向 1、正向 2、反向|integer(int32)||
|&emsp;&emsp;forwardAgvDirection|正向行驶时agv方向 1、正向 2、反向|integer(int32)||
|&emsp;&emsp;reverseAgvDirection|反向行驶时agv方向 1、正向 2、反向|integer(int32)||
|&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|&emsp;&emsp;autoDoorId|自动门ID|string||
|sidePathVos|sidePath数据|array|pathVo|
|&emsp;&emsp;weightRatio|路径权重系数|number(double)||
|&emsp;&emsp;path|路径|Path|Path|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;agvMapName|地图ID||false|string||
|&emsp;&emsp;&emsp;&emsp;startMarkerId|开始标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;endMarkerId|结束标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;startControl|开始点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;endControl|结束点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;length|长度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;direction|方向 0、双向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;forwardAgvDirection|正向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;reverseAgvDirection|反向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;&emsp;&emsp;autoDoorId|自动门ID||false|string||
|&emsp;&emsp;sidePathVos|sidePath数据|array|pathVo|
|&emsp;&emsp;&emsp;&emsp;weightRatio|路径权重系数||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;path|路径||false|Path|Path|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;agvMapName|地图ID||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;startMarkerId|开始标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;endMarkerId|结束标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;startControl|开始点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;endControl|结束点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;length|长度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;direction|方向 0、双向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;forwardAgvDirection|正向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;reverseAgvDirection|反向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;autoDoorId|自动门ID||false|string||
|&emsp;&emsp;&emsp;&emsp;sidePathVos|sidePath数据||false|array|pathVo|
|&emsp;&emsp;&emsp;&emsp;startMarkerId|开始标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;endMarkerId|结束标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;agvDirection|agv方向: 0、双向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;directionAgv|AGV要朝向的角度（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;directionAgv2|AGV要朝向的角度2（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;directionShelf|货架要朝向的角度（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;pathType|路径类型: 0、普通路径 1、二维码对接路径 2、脱离对接路径||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;rpmShelf|uint, 货架旋转速度，单位，转/每分钟||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;workStationCode|工位编码||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;directionShelf2|货架要朝向的角度2（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;position|位置，1、起始点 2、结束点||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;effectivePath|生效路径 1、全部路径 2、第一段路径||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;hasAction|是否有动作,1、有 0、没有||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;pathParam|路径导航参数||false|PathParam|PathParam|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;safety_scanner_region|雷达避障区域 0、默认区域||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;safety|避障 1、打开避障  2、关闭避障||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;max_translation_speed|最大平移速度 >0 m/s||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;max_rotate_speed|最大旋转速度 rad/s >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;P|平移加速比例控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;D|平移加速微分控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;translation_acc|平移加（减）速度 m/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rotate_acc|旋转加（减）速度 rad/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;updateTime|修改时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;extend_bit|拓展布尔||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;extend_string|拓展字符串||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;features_requested|融合特征 1、开启 0、关闭||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;agvDirection2|agv方向2: -180 ~ 180||false|integer(int32)||
|&emsp;&emsp;startMarkerId|开始标记点|string||
|&emsp;&emsp;endMarkerId|结束标记点|string||
|&emsp;&emsp;agvDirection|agv方向: 0、双向 1、正向 2、反向|integer(int32)||
|&emsp;&emsp;directionAgv|AGV要朝向的角度（地图坐标系下）  -180 ~ 180|number(double)||
|&emsp;&emsp;directionAgv2|AGV要朝向的角度2（地图坐标系下）  -180 ~ 180|number(double)||
|&emsp;&emsp;directionShelf|货架要朝向的角度（地图坐标系下）  -180 ~ 180|number(double)||
|&emsp;&emsp;pathType|路径类型: 0、普通路径 1、二维码对接路径 2、脱离对接路径|integer(int32)||
|&emsp;&emsp;rpmShelf|uint, 货架旋转速度，单位，转/每分钟|integer(int32)||
|&emsp;&emsp;workStationCode|工位编码|integer(int32)||
|&emsp;&emsp;directionShelf2|货架要朝向的角度2（地图坐标系下）  -180 ~ 180|number(double)||
|&emsp;&emsp;position|位置，1、起始点 2、结束点|integer(int32)||
|&emsp;&emsp;effectivePath|生效路径 1、全部路径 2、第一段路径|integer(int32)||
|&emsp;&emsp;hasAction|是否有动作,1、有 0、没有|integer(int32)||
|&emsp;&emsp;pathParam|路径导航参数|PathParam|PathParam|
|&emsp;&emsp;&emsp;&emsp;safety_scanner_region|雷达避障区域 0、默认区域||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;safety|避障 1、打开避障  2、关闭避障||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;max_translation_speed|最大平移速度 >0 m/s||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;max_rotate_speed|最大旋转速度 rad/s >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;P|平移加速比例控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;D|平移加速微分控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;translation_acc|平移加（减）速度 m/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;rotate_acc|旋转加（减）速度 rad/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;updateTime|修改时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;extend_bit|拓展布尔||false|string||
|&emsp;&emsp;&emsp;&emsp;extend_string|拓展字符串||false|string||
|&emsp;&emsp;&emsp;&emsp;features_requested|融合特征 1、开启 0、关闭||false|integer(int32)||
|&emsp;&emsp;agvDirection2|agv方向2: -180 ~ 180|integer(int32)||
|startMarkerId|开始标记点|string||
|endMarkerId|结束标记点|string||
|agvDirection|agv方向: 0、双向 1、正向 2、反向|integer(int32)|integer(int32)|
|directionAgv|AGV要朝向的角度（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|directionAgv2|AGV要朝向的角度2（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|directionShelf|货架要朝向的角度（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|pathType|路径类型: 0、普通路径 1、二维码对接路径 2、脱离对接路径|integer(int32)|integer(int32)|
|rpmShelf|uint, 货架旋转速度，单位，转/每分钟|integer(int32)|integer(int32)|
|workStationCode|工位编码|integer(int32)|integer(int32)|
|directionShelf2|货架要朝向的角度2（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|position|位置，1、起始点 2、结束点|integer(int32)|integer(int32)|
|effectivePath|生效路径 1、全部路径 2、第一段路径|integer(int32)|integer(int32)|
|hasAction|是否有动作,1、有 0、没有|integer(int32)|integer(int32)|
|pathParam|路径导航参数|PathParam|PathParam|
|&emsp;&emsp;safety_scanner_region|雷达避障区域 0、默认区域|integer(int32)||
|&emsp;&emsp;safety|避障 1、打开避障  2、关闭避障|integer(int32)||
|&emsp;&emsp;max_translation_speed|最大平移速度 >0 m/s|number(double)||
|&emsp;&emsp;max_rotate_speed|最大旋转速度 rad/s >0|number(double)||
|&emsp;&emsp;P|平移加速比例控制系数 >0|number(double)||
|&emsp;&emsp;D|平移加速微分控制系数 >0|number(double)||
|&emsp;&emsp;translation_acc|平移加（减）速度 m/s2 >0|number(double)||
|&emsp;&emsp;rotate_acc|旋转加（减）速度 rad/s2 >0|number(double)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|修改时间|string(date-time)||
|&emsp;&emsp;extend_bit|拓展布尔|string||
|&emsp;&emsp;extend_string|拓展字符串|string||
|&emsp;&emsp;features_requested|融合特征 1、开启 0、关闭|integer(int32)||
|agvDirection2|agv方向2: -180 ~ 180|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"weightRatio": 0,
	"path": {
		"id": "",
		"agvMapName": "",
		"startMarkerId": "",
		"endMarkerId": "",
		"startControl": "",
		"endControl": "",
		"length": 0,
		"lineType": 0,
		"direction": 0,
		"forwardAgvDirection": 0,
		"reverseAgvDirection": 0,
		"usageStatus": "",
		"autoDoorId": ""
	},
	"sidePathVos": [
		{
			"weightRatio": 0,
			"path": "",
			"sidePathVos": [],
			"startMarkerId": "",
			"endMarkerId": "",
			"agvDirection": 0,
			"directionAgv": 0,
			"directionAgv2": 0,
			"directionShelf": 0,
			"pathType": 0,
			"rpmShelf": 0,
			"workStationCode": 0,
			"directionShelf2": 0,
			"position": 0,
			"effectivePath": 0,
			"hasAction": 0,
			"pathParam": "",
			"agvDirection2": 0
		}
	],
	"startMarkerId": "",
	"endMarkerId": "",
	"agvDirection": 0,
	"directionAgv": 0,
	"directionAgv2": 0,
	"directionShelf": 0,
	"pathType": 0,
	"rpmShelf": 0,
	"workStationCode": 0,
	"directionShelf2": 0,
	"position": 0,
	"effectivePath": 0,
	"hasAction": 0,
	"pathParam": {
		"safety_scanner_region": 0,
		"safety": 0,
		"max_translation_speed": 0,
		"max_rotate_speed": 0,
		"P": 0,
		"D": 0,
		"translation_acc": 0,
		"rotate_acc": 0,
		"createTime": "",
		"updateTime": "",
		"extend_bit": "",
		"extend_string": "",
		"features_requested": 0
	},
	"agvDirection2": 0
}
```


## 详情


**接口地址**:`/api/v3/paths/{agvMapName}/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|agvMapName|地图名称|path|true|string||
|id|路径ID|path|true|string||
|isDraft|是否查询草稿数据|query|true|boolean||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|pathVo|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|weightRatio|路径权重系数|number(double)|number(double)|
|path|路径|Path|Path|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;agvMapName|地图ID|string||
|&emsp;&emsp;startMarkerId|开始标记点|string||
|&emsp;&emsp;endMarkerId|结束标记点|string||
|&emsp;&emsp;startControl|开始点的控制点xy坐标|string||
|&emsp;&emsp;endControl|结束点的控制点xy坐标|string||
|&emsp;&emsp;length|长度|number(double)||
|&emsp;&emsp;lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）|integer(int32)||
|&emsp;&emsp;direction|方向 0、双向 1、正向 2、反向|integer(int32)||
|&emsp;&emsp;forwardAgvDirection|正向行驶时agv方向 1、正向 2、反向|integer(int32)||
|&emsp;&emsp;reverseAgvDirection|反向行驶时agv方向 1、正向 2、反向|integer(int32)||
|&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|&emsp;&emsp;autoDoorId|自动门ID|string||
|sidePathVos|sidePath数据|array|pathVo|
|&emsp;&emsp;weightRatio|路径权重系数|number(double)||
|&emsp;&emsp;path|路径|Path|Path|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;agvMapName|地图ID||false|string||
|&emsp;&emsp;&emsp;&emsp;startMarkerId|开始标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;endMarkerId|结束标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;startControl|开始点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;endControl|结束点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;length|长度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;direction|方向 0、双向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;forwardAgvDirection|正向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;reverseAgvDirection|反向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;&emsp;&emsp;autoDoorId|自动门ID||false|string||
|&emsp;&emsp;sidePathVos|sidePath数据|array|pathVo|
|&emsp;&emsp;&emsp;&emsp;weightRatio|路径权重系数||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;path|路径||false|Path|Path|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;agvMapName|地图ID||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;startMarkerId|开始标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;endMarkerId|结束标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;startControl|开始点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;endControl|结束点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;length|长度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;direction|方向 0、双向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;forwardAgvDirection|正向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;reverseAgvDirection|反向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;autoDoorId|自动门ID||false|string||
|&emsp;&emsp;&emsp;&emsp;sidePathVos|sidePath数据||false|array|pathVo|
|&emsp;&emsp;&emsp;&emsp;startMarkerId|开始标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;endMarkerId|结束标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;agvDirection|agv方向: 0、双向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;directionAgv|AGV要朝向的角度（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;directionAgv2|AGV要朝向的角度2（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;directionShelf|货架要朝向的角度（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;pathType|路径类型: 0、普通路径 1、二维码对接路径 2、脱离对接路径||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;rpmShelf|uint, 货架旋转速度，单位，转/每分钟||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;workStationCode|工位编码||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;directionShelf2|货架要朝向的角度2（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;position|位置，1、起始点 2、结束点||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;effectivePath|生效路径 1、全部路径 2、第一段路径||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;hasAction|是否有动作,1、有 0、没有||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;pathParam|路径导航参数||false|PathParam|PathParam|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;safety_scanner_region|雷达避障区域 0、默认区域||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;safety|避障 1、打开避障  2、关闭避障||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;max_translation_speed|最大平移速度 >0 m/s||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;max_rotate_speed|最大旋转速度 rad/s >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;P|平移加速比例控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;D|平移加速微分控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;translation_acc|平移加（减）速度 m/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rotate_acc|旋转加（减）速度 rad/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;updateTime|修改时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;extend_bit|拓展布尔||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;extend_string|拓展字符串||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;features_requested|融合特征 1、开启 0、关闭||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;agvDirection2|agv方向2: -180 ~ 180||false|integer(int32)||
|&emsp;&emsp;startMarkerId|开始标记点|string||
|&emsp;&emsp;endMarkerId|结束标记点|string||
|&emsp;&emsp;agvDirection|agv方向: 0、双向 1、正向 2、反向|integer(int32)||
|&emsp;&emsp;directionAgv|AGV要朝向的角度（地图坐标系下）  -180 ~ 180|number(double)||
|&emsp;&emsp;directionAgv2|AGV要朝向的角度2（地图坐标系下）  -180 ~ 180|number(double)||
|&emsp;&emsp;directionShelf|货架要朝向的角度（地图坐标系下）  -180 ~ 180|number(double)||
|&emsp;&emsp;pathType|路径类型: 0、普通路径 1、二维码对接路径 2、脱离对接路径|integer(int32)||
|&emsp;&emsp;rpmShelf|uint, 货架旋转速度，单位，转/每分钟|integer(int32)||
|&emsp;&emsp;workStationCode|工位编码|integer(int32)||
|&emsp;&emsp;directionShelf2|货架要朝向的角度2（地图坐标系下）  -180 ~ 180|number(double)||
|&emsp;&emsp;position|位置，1、起始点 2、结束点|integer(int32)||
|&emsp;&emsp;effectivePath|生效路径 1、全部路径 2、第一段路径|integer(int32)||
|&emsp;&emsp;hasAction|是否有动作,1、有 0、没有|integer(int32)||
|&emsp;&emsp;pathParam|路径导航参数|PathParam|PathParam|
|&emsp;&emsp;&emsp;&emsp;safety_scanner_region|雷达避障区域 0、默认区域||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;safety|避障 1、打开避障  2、关闭避障||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;max_translation_speed|最大平移速度 >0 m/s||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;max_rotate_speed|最大旋转速度 rad/s >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;P|平移加速比例控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;D|平移加速微分控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;translation_acc|平移加（减）速度 m/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;rotate_acc|旋转加（减）速度 rad/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;updateTime|修改时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;extend_bit|拓展布尔||false|string||
|&emsp;&emsp;&emsp;&emsp;extend_string|拓展字符串||false|string||
|&emsp;&emsp;&emsp;&emsp;features_requested|融合特征 1、开启 0、关闭||false|integer(int32)||
|&emsp;&emsp;agvDirection2|agv方向2: -180 ~ 180|integer(int32)||
|startMarkerId|开始标记点|string||
|endMarkerId|结束标记点|string||
|agvDirection|agv方向: 0、双向 1、正向 2、反向|integer(int32)|integer(int32)|
|directionAgv|AGV要朝向的角度（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|directionAgv2|AGV要朝向的角度2（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|directionShelf|货架要朝向的角度（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|pathType|路径类型: 0、普通路径 1、二维码对接路径 2、脱离对接路径|integer(int32)|integer(int32)|
|rpmShelf|uint, 货架旋转速度，单位，转/每分钟|integer(int32)|integer(int32)|
|workStationCode|工位编码|integer(int32)|integer(int32)|
|directionShelf2|货架要朝向的角度2（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|position|位置，1、起始点 2、结束点|integer(int32)|integer(int32)|
|effectivePath|生效路径 1、全部路径 2、第一段路径|integer(int32)|integer(int32)|
|hasAction|是否有动作,1、有 0、没有|integer(int32)|integer(int32)|
|pathParam|路径导航参数|PathParam|PathParam|
|&emsp;&emsp;safety_scanner_region|雷达避障区域 0、默认区域|integer(int32)||
|&emsp;&emsp;safety|避障 1、打开避障  2、关闭避障|integer(int32)||
|&emsp;&emsp;max_translation_speed|最大平移速度 >0 m/s|number(double)||
|&emsp;&emsp;max_rotate_speed|最大旋转速度 rad/s >0|number(double)||
|&emsp;&emsp;P|平移加速比例控制系数 >0|number(double)||
|&emsp;&emsp;D|平移加速微分控制系数 >0|number(double)||
|&emsp;&emsp;translation_acc|平移加（减）速度 m/s2 >0|number(double)||
|&emsp;&emsp;rotate_acc|旋转加（减）速度 rad/s2 >0|number(double)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|修改时间|string(date-time)||
|&emsp;&emsp;extend_bit|拓展布尔|string||
|&emsp;&emsp;extend_string|拓展字符串|string||
|&emsp;&emsp;features_requested|融合特征 1、开启 0、关闭|integer(int32)||
|agvDirection2|agv方向2: -180 ~ 180|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"weightRatio": 0,
	"path": {
		"id": "",
		"agvMapName": "",
		"startMarkerId": "",
		"endMarkerId": "",
		"startControl": "",
		"endControl": "",
		"length": 0,
		"lineType": 0,
		"direction": 0,
		"forwardAgvDirection": 0,
		"reverseAgvDirection": 0,
		"usageStatus": "",
		"autoDoorId": ""
	},
	"sidePathVos": [
		{
			"weightRatio": 0,
			"path": "",
			"sidePathVos": [],
			"startMarkerId": "",
			"endMarkerId": "",
			"agvDirection": 0,
			"directionAgv": 0,
			"directionAgv2": 0,
			"directionShelf": 0,
			"pathType": 0,
			"rpmShelf": 0,
			"workStationCode": 0,
			"directionShelf2": 0,
			"position": 0,
			"effectivePath": 0,
			"hasAction": 0,
			"pathParam": "",
			"agvDirection2": 0
		}
	],
	"startMarkerId": "",
	"endMarkerId": "",
	"agvDirection": 0,
	"directionAgv": 0,
	"directionAgv2": 0,
	"directionShelf": 0,
	"pathType": 0,
	"rpmShelf": 0,
	"workStationCode": 0,
	"directionShelf2": 0,
	"position": 0,
	"effectivePath": 0,
	"hasAction": 0,
	"pathParam": {
		"safety_scanner_region": 0,
		"safety": 0,
		"max_translation_speed": 0,
		"max_rotate_speed": 0,
		"P": 0,
		"D": 0,
		"translation_acc": 0,
		"rotate_acc": 0,
		"createTime": "",
		"updateTime": "",
		"extend_bit": "",
		"extend_string": "",
		"features_requested": 0
	},
	"agvDirection2": 0
}
```


## 删除


**接口地址**:`/api/v3/paths/{agvMapName}/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|agvMapName|agvMapName|path|true|string||
|id|路径ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 更新


**接口地址**:`/api/v3/paths/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|路径ID|path|true|string||
|pathVo|路径|body|true|PathVo|PathVo|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|pathVo|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|weightRatio|路径权重系数|number(double)|number(double)|
|path|路径|Path|Path|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;agvMapName|地图ID|string||
|&emsp;&emsp;startMarkerId|开始标记点|string||
|&emsp;&emsp;endMarkerId|结束标记点|string||
|&emsp;&emsp;startControl|开始点的控制点xy坐标|string||
|&emsp;&emsp;endControl|结束点的控制点xy坐标|string||
|&emsp;&emsp;length|长度|number(double)||
|&emsp;&emsp;lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）|integer(int32)||
|&emsp;&emsp;direction|方向 0、双向 1、正向 2、反向|integer(int32)||
|&emsp;&emsp;forwardAgvDirection|正向行驶时agv方向 1、正向 2、反向|integer(int32)||
|&emsp;&emsp;reverseAgvDirection|反向行驶时agv方向 1、正向 2、反向|integer(int32)||
|&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|&emsp;&emsp;autoDoorId|自动门ID|string||
|sidePathVos|sidePath数据|array|pathVo|
|&emsp;&emsp;weightRatio|路径权重系数|number(double)||
|&emsp;&emsp;path|路径|Path|Path|
|&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;agvMapName|地图ID||false|string||
|&emsp;&emsp;&emsp;&emsp;startMarkerId|开始标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;endMarkerId|结束标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;startControl|开始点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;endControl|结束点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;length|长度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;direction|方向 0、双向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;forwardAgvDirection|正向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;reverseAgvDirection|反向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;&emsp;&emsp;autoDoorId|自动门ID||false|string||
|&emsp;&emsp;sidePathVos|sidePath数据|array|pathVo|
|&emsp;&emsp;&emsp;&emsp;weightRatio|路径权重系数||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;path|路径||false|Path|Path|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;agvMapName|地图ID||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;startMarkerId|开始标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;endMarkerId|结束标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;startControl|开始点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;endControl|结束点的控制点xy坐标||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;length|长度||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;direction|方向 0、双向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;forwardAgvDirection|正向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;reverseAgvDirection|反向行驶时agv方向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;usageStatus|使用状态 ENABLE:启用  DISABLE:禁用||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;autoDoorId|自动门ID||false|string||
|&emsp;&emsp;&emsp;&emsp;sidePathVos|sidePath数据||false|array|pathVo|
|&emsp;&emsp;&emsp;&emsp;startMarkerId|开始标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;endMarkerId|结束标记点||false|string||
|&emsp;&emsp;&emsp;&emsp;agvDirection|agv方向: 0、双向 1、正向 2、反向||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;directionAgv|AGV要朝向的角度（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;directionAgv2|AGV要朝向的角度2（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;directionShelf|货架要朝向的角度（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;pathType|路径类型: 0、普通路径 1、二维码对接路径 2、脱离对接路径||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;rpmShelf|uint, 货架旋转速度，单位，转/每分钟||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;workStationCode|工位编码||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;directionShelf2|货架要朝向的角度2（地图坐标系下）  -180 ~ 180||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;position|位置，1、起始点 2、结束点||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;effectivePath|生效路径 1、全部路径 2、第一段路径||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;hasAction|是否有动作,1、有 0、没有||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;pathParam|路径导航参数||false|PathParam|PathParam|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;safety_scanner_region|雷达避障区域 0、默认区域||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;safety|避障 1、打开避障  2、关闭避障||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;max_translation_speed|最大平移速度 >0 m/s||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;max_rotate_speed|最大旋转速度 rad/s >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;P|平移加速比例控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;D|平移加速微分控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;translation_acc|平移加（减）速度 m/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rotate_acc|旋转加（减）速度 rad/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;updateTime|修改时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;extend_bit|拓展布尔||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;extend_string|拓展字符串||false|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;features_requested|融合特征 1、开启 0、关闭||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;agvDirection2|agv方向2: -180 ~ 180||false|integer(int32)||
|&emsp;&emsp;startMarkerId|开始标记点|string||
|&emsp;&emsp;endMarkerId|结束标记点|string||
|&emsp;&emsp;agvDirection|agv方向: 0、双向 1、正向 2、反向|integer(int32)||
|&emsp;&emsp;directionAgv|AGV要朝向的角度（地图坐标系下）  -180 ~ 180|number(double)||
|&emsp;&emsp;directionAgv2|AGV要朝向的角度2（地图坐标系下）  -180 ~ 180|number(double)||
|&emsp;&emsp;directionShelf|货架要朝向的角度（地图坐标系下）  -180 ~ 180|number(double)||
|&emsp;&emsp;pathType|路径类型: 0、普通路径 1、二维码对接路径 2、脱离对接路径|integer(int32)||
|&emsp;&emsp;rpmShelf|uint, 货架旋转速度，单位，转/每分钟|integer(int32)||
|&emsp;&emsp;workStationCode|工位编码|integer(int32)||
|&emsp;&emsp;directionShelf2|货架要朝向的角度2（地图坐标系下）  -180 ~ 180|number(double)||
|&emsp;&emsp;position|位置，1、起始点 2、结束点|integer(int32)||
|&emsp;&emsp;effectivePath|生效路径 1、全部路径 2、第一段路径|integer(int32)||
|&emsp;&emsp;hasAction|是否有动作,1、有 0、没有|integer(int32)||
|&emsp;&emsp;pathParam|路径导航参数|PathParam|PathParam|
|&emsp;&emsp;&emsp;&emsp;safety_scanner_region|雷达避障区域 0、默认区域||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;safety|避障 1、打开避障  2、关闭避障||false|integer(int32)||
|&emsp;&emsp;&emsp;&emsp;max_translation_speed|最大平移速度 >0 m/s||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;max_rotate_speed|最大旋转速度 rad/s >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;P|平移加速比例控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;D|平移加速微分控制系数 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;translation_acc|平移加（减）速度 m/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;rotate_acc|旋转加（减）速度 rad/s2 >0||false|number(double)||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;updateTime|修改时间||false|string(date-time)||
|&emsp;&emsp;&emsp;&emsp;extend_bit|拓展布尔||false|string||
|&emsp;&emsp;&emsp;&emsp;extend_string|拓展字符串||false|string||
|&emsp;&emsp;&emsp;&emsp;features_requested|融合特征 1、开启 0、关闭||false|integer(int32)||
|&emsp;&emsp;agvDirection2|agv方向2: -180 ~ 180|integer(int32)||
|startMarkerId|开始标记点|string||
|endMarkerId|结束标记点|string||
|agvDirection|agv方向: 0、双向 1、正向 2、反向|integer(int32)|integer(int32)|
|directionAgv|AGV要朝向的角度（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|directionAgv2|AGV要朝向的角度2（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|directionShelf|货架要朝向的角度（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|pathType|路径类型: 0、普通路径 1、二维码对接路径 2、脱离对接路径|integer(int32)|integer(int32)|
|rpmShelf|uint, 货架旋转速度，单位，转/每分钟|integer(int32)|integer(int32)|
|workStationCode|工位编码|integer(int32)|integer(int32)|
|directionShelf2|货架要朝向的角度2（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|position|位置，1、起始点 2、结束点|integer(int32)|integer(int32)|
|effectivePath|生效路径 1、全部路径 2、第一段路径|integer(int32)|integer(int32)|
|hasAction|是否有动作,1、有 0、没有|integer(int32)|integer(int32)|
|pathParam|路径导航参数|PathParam|PathParam|
|&emsp;&emsp;safety_scanner_region|雷达避障区域 0、默认区域|integer(int32)||
|&emsp;&emsp;safety|避障 1、打开避障  2、关闭避障|integer(int32)||
|&emsp;&emsp;max_translation_speed|最大平移速度 >0 m/s|number(double)||
|&emsp;&emsp;max_rotate_speed|最大旋转速度 rad/s >0|number(double)||
|&emsp;&emsp;P|平移加速比例控制系数 >0|number(double)||
|&emsp;&emsp;D|平移加速微分控制系数 >0|number(double)||
|&emsp;&emsp;translation_acc|平移加（减）速度 m/s2 >0|number(double)||
|&emsp;&emsp;rotate_acc|旋转加（减）速度 rad/s2 >0|number(double)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|修改时间|string(date-time)||
|&emsp;&emsp;extend_bit|拓展布尔|string||
|&emsp;&emsp;extend_string|拓展字符串|string||
|&emsp;&emsp;features_requested|融合特征 1、开启 0、关闭|integer(int32)||
|agvDirection2|agv方向2: -180 ~ 180|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"weightRatio": 0,
	"path": {
		"id": "",
		"agvMapName": "",
		"startMarkerId": "",
		"endMarkerId": "",
		"startControl": "",
		"endControl": "",
		"length": 0,
		"lineType": 0,
		"direction": 0,
		"forwardAgvDirection": 0,
		"reverseAgvDirection": 0,
		"usageStatus": "",
		"autoDoorId": ""
	},
	"sidePathVos": [
		{
			"weightRatio": 0,
			"path": "",
			"sidePathVos": [],
			"startMarkerId": "",
			"endMarkerId": "",
			"agvDirection": 0,
			"directionAgv": 0,
			"directionAgv2": 0,
			"directionShelf": 0,
			"pathType": 0,
			"rpmShelf": 0,
			"workStationCode": 0,
			"directionShelf2": 0,
			"position": 0,
			"effectivePath": 0,
			"hasAction": 0,
			"pathParam": "",
			"agvDirection2": 0
		}
	],
	"startMarkerId": "",
	"endMarkerId": "",
	"agvDirection": 0,
	"directionAgv": 0,
	"directionAgv2": 0,
	"directionShelf": 0,
	"pathType": 0,
	"rpmShelf": 0,
	"workStationCode": 0,
	"directionShelf2": 0,
	"position": 0,
	"effectivePath": 0,
	"hasAction": 0,
	"pathParam": {
		"safety_scanner_region": 0,
		"safety": 0,
		"max_translation_speed": 0,
		"max_rotate_speed": 0,
		"P": 0,
		"D": 0,
		"translation_acc": 0,
		"rotate_acc": 0,
		"createTime": "",
		"updateTime": "",
		"extend_bit": "",
		"extend_string": "",
		"features_requested": 0
	},
	"agvDirection2": 0
}
```


# 路径规划调试


## 获取地图路径权重


**接口地址**:`/api/v3/pathPlanTest/DirectEdgeWeight`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|DirectEdgeWeight|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|acode||string||
|bcode||string||
|weight||number(double)|number(double)|
|weightAuto||number(double)|number(double)|
|weightFixed||number(double)|number(double)|
|weightUser||number(double)|number(double)|


**响应示例**:
```javascript
[
	{
		"acode": "",
		"bcode": "",
		"weight": 0,
		"weightAuto": 0,
		"weightFixed": 0,
		"weightUser": 0
	}
]
```


## 获取所有激活的marker code


**接口地址**:`/api/v3/pathPlanTest/GetAllMarker`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 获取AGV在路径中的定位数据


**接口地址**:`/api/v3/pathPlanTest/GetLocationInDirectEdge`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 地图阻塞路径


**接口地址**:`/api/v3/pathPlanTest/JamSidePaths`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|DirectEdgeWeight|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|acode||string||
|bcode||string||
|weight||number(double)|number(double)|
|weightAuto||number(double)|number(double)|
|weightFixed||number(double)|number(double)|
|weightUser||number(double)|number(double)|


**响应示例**:
```javascript
[
	{
		"acode": "",
		"bcode": "",
		"weight": 0,
		"weightAuto": 0,
		"weightFixed": 0,
		"weightUser": 0
	}
]
```


## 重置地图路径权重


**接口地址**:`/api/v3/pathPlanTest/ResetDirectEdgeWeight`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 获取AGV的规划路径


**接口地址**:`/api/v3/pathPlanTest/agvPlannedSidePaths`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|TempSidePath|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endMarkerCode||string||
|sidePathId||string||
|startMarkerCode||string||
|t0||number(double)|number(double)|
|t1||number(double)|number(double)|


**响应示例**:
```javascript
[
	{
		"endMarkerCode": "",
		"sidePathId": "",
		"startMarkerCode": "",
		"t0": 0,
		"t1": 0
	}
]
```


# 边路径


## 列表


**接口地址**:`/api/v3/sidePaths`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|agvMapName|标记点ID|query|true|string||
|isDraft|是否查询草稿文件数据|query|true|boolean||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|SidePath|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|pathParam|路径参数|PathParam|PathParam|
|&emsp;&emsp;safety_scanner_region|雷达避障区域 0、默认区域|integer(int32)||
|&emsp;&emsp;safety|避障 1、打开避障  2、关闭避障|integer(int32)||
|&emsp;&emsp;max_translation_speed|最大平移速度 >0 m/s|number(double)||
|&emsp;&emsp;max_rotate_speed|最大旋转速度 rad/s >0|number(double)||
|&emsp;&emsp;P|平移加速比例控制系数 >0|number(double)||
|&emsp;&emsp;D|平移加速微分控制系数 >0|number(double)||
|&emsp;&emsp;translation_acc|平移加（减）速度 m/s2 >0|number(double)||
|&emsp;&emsp;rotate_acc|旋转加（减）速度 rad/s2 >0|number(double)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|修改时间|string(date-time)||
|&emsp;&emsp;extend_bit|拓展布尔|string||
|&emsp;&emsp;extend_string|拓展字符串|string||
|&emsp;&emsp;features_requested|融合特征 1、开启 0、关闭|integer(int32)||
|safetyScannerRegion||integer(int32)|integer(int32)|
|weightRatio|路径权重系数|number(double)|number(double)|
|agvMapName|地图ID|string||
|pathId|路径ID|string||
|startMarkerId|开始标记点|string||
|endMarkerId|结束标记点|string||
|startControl|开始点的控制点xy坐标|string||
|endControl|结束点的控制点xy坐标|string||
|length|长度|number(double)|number(double)|
|lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）|integer(int32)|integer(int32)|
|agvDirection|agv方向: 0、双向 1、正向 2、反向|integer(int32)|integer(int32)|
|usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|autoDoorId|自动门ID|string||
|directionAgv|AGV要朝向的角度（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|directionAgv2|AGV要朝向的角度2（地图坐标系下）（预留，暂不使用）  -180 ~ 180|number(double)|number(double)|
|pathType|路径类型: 0、普通路径 1、二维码对接路径 2、脱离对接路径|integer(int32)|integer(int32)|
|directionShelf|货架要朝向的角度1（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|workStationCode|工位编码|integer(int32)|integer(int32)|
|directionShelf2|货架要朝向的角度2（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|position|位置，1、起始点 2、结束点|integer(int32)|integer(int32)|
|effectivePath|生效路径 1、全部路径 2、第一段路径|integer(int32)|integer(int32)|
|rpmShelf|uint, 货架旋转速度，单位，转/每分钟|integer(int32)|integer(int32)|
|firstPath|是否是首段路径 1、是 0、否|integer(int32)|integer(int32)|
|accurateStop|是否启用末端精定位: 0不启用 1启用，默认是不启用|integer(int32)|integer(int32)|
|hasAction|是否有动作,1、有 0、没有|integer(int32)|integer(int32)|
|agvDirection2|agv方向2: -180 ~ 180|integer(int32)|integer(int32)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"pathParam": {
			"safety_scanner_region": 0,
			"safety": 0,
			"max_translation_speed": 0,
			"max_rotate_speed": 0,
			"P": 0,
			"D": 0,
			"translation_acc": 0,
			"rotate_acc": 0,
			"createTime": "",
			"updateTime": "",
			"extend_bit": "",
			"extend_string": "",
			"features_requested": 0
		},
		"safetyScannerRegion": 0,
		"weightRatio": 0,
		"agvMapName": "",
		"pathId": "",
		"startMarkerId": "",
		"endMarkerId": "",
		"startControl": "",
		"endControl": "",
		"length": 0,
		"lineType": 0,
		"agvDirection": 0,
		"usageStatus": "",
		"autoDoorId": "",
		"directionAgv": 0,
		"directionAgv2": 0,
		"pathType": 0,
		"directionShelf": 0,
		"workStationCode": 0,
		"directionShelf2": 0,
		"position": 0,
		"effectivePath": 0,
		"rpmShelf": 0,
		"firstPath": 0,
		"accurateStop": 0,
		"hasAction": 0,
		"agvDirection2": 0
	}
]
```


## 根据pathId查询


**接口地址**:`/api/v3/sidePaths/{agvMapName}/selectByPathId`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|agvMapName|标记点ID|path|true|string||
|isDraft|是否查询草稿文件数据|query|true|boolean||
|pathId|标记点ID|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|SidePath|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|pathParam|路径参数|PathParam|PathParam|
|&emsp;&emsp;safety_scanner_region|雷达避障区域 0、默认区域|integer(int32)||
|&emsp;&emsp;safety|避障 1、打开避障  2、关闭避障|integer(int32)||
|&emsp;&emsp;max_translation_speed|最大平移速度 >0 m/s|number(double)||
|&emsp;&emsp;max_rotate_speed|最大旋转速度 rad/s >0|number(double)||
|&emsp;&emsp;P|平移加速比例控制系数 >0|number(double)||
|&emsp;&emsp;D|平移加速微分控制系数 >0|number(double)||
|&emsp;&emsp;translation_acc|平移加（减）速度 m/s2 >0|number(double)||
|&emsp;&emsp;rotate_acc|旋转加（减）速度 rad/s2 >0|number(double)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|修改时间|string(date-time)||
|&emsp;&emsp;extend_bit|拓展布尔|string||
|&emsp;&emsp;extend_string|拓展字符串|string||
|&emsp;&emsp;features_requested|融合特征 1、开启 0、关闭|integer(int32)||
|safetyScannerRegion||integer(int32)|integer(int32)|
|weightRatio|路径权重系数|number(double)|number(double)|
|agvMapName|地图ID|string||
|pathId|路径ID|string||
|startMarkerId|开始标记点|string||
|endMarkerId|结束标记点|string||
|startControl|开始点的控制点xy坐标|string||
|endControl|结束点的控制点xy坐标|string||
|length|长度|number(double)|number(double)|
|lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）|integer(int32)|integer(int32)|
|agvDirection|agv方向: 0、双向 1、正向 2、反向|integer(int32)|integer(int32)|
|usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|autoDoorId|自动门ID|string||
|directionAgv|AGV要朝向的角度（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|directionAgv2|AGV要朝向的角度2（地图坐标系下）（预留，暂不使用）  -180 ~ 180|number(double)|number(double)|
|pathType|路径类型: 0、普通路径 1、二维码对接路径 2、脱离对接路径|integer(int32)|integer(int32)|
|directionShelf|货架要朝向的角度1（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|workStationCode|工位编码|integer(int32)|integer(int32)|
|directionShelf2|货架要朝向的角度2（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|position|位置，1、起始点 2、结束点|integer(int32)|integer(int32)|
|effectivePath|生效路径 1、全部路径 2、第一段路径|integer(int32)|integer(int32)|
|rpmShelf|uint, 货架旋转速度，单位，转/每分钟|integer(int32)|integer(int32)|
|firstPath|是否是首段路径 1、是 0、否|integer(int32)|integer(int32)|
|accurateStop|是否启用末端精定位: 0不启用 1启用，默认是不启用|integer(int32)|integer(int32)|
|hasAction|是否有动作,1、有 0、没有|integer(int32)|integer(int32)|
|agvDirection2|agv方向2: -180 ~ 180|integer(int32)|integer(int32)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"pathParam": {
			"safety_scanner_region": 0,
			"safety": 0,
			"max_translation_speed": 0,
			"max_rotate_speed": 0,
			"P": 0,
			"D": 0,
			"translation_acc": 0,
			"rotate_acc": 0,
			"createTime": "",
			"updateTime": "",
			"extend_bit": "",
			"extend_string": "",
			"features_requested": 0
		},
		"safetyScannerRegion": 0,
		"weightRatio": 0,
		"agvMapName": "",
		"pathId": "",
		"startMarkerId": "",
		"endMarkerId": "",
		"startControl": "",
		"endControl": "",
		"length": 0,
		"lineType": 0,
		"agvDirection": 0,
		"usageStatus": "",
		"autoDoorId": "",
		"directionAgv": 0,
		"directionAgv2": 0,
		"pathType": 0,
		"directionShelf": 0,
		"workStationCode": 0,
		"directionShelf2": 0,
		"position": 0,
		"effectivePath": 0,
		"rpmShelf": 0,
		"firstPath": 0,
		"accurateStop": 0,
		"hasAction": 0,
		"agvDirection2": 0
	}
]
```


## 详情


**接口地址**:`/api/v3/sidePaths/{agvMapName}/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|agvMapName|标记点ID|path|true|string||
|id|标记点ID|path|true|string||
|isDraft|是否查询草稿文件数据|query|true|boolean||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|SidePath|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|pathParam|路径参数|PathParam|PathParam|
|&emsp;&emsp;safety_scanner_region|雷达避障区域 0、默认区域|integer(int32)||
|&emsp;&emsp;safety|避障 1、打开避障  2、关闭避障|integer(int32)||
|&emsp;&emsp;max_translation_speed|最大平移速度 >0 m/s|number(double)||
|&emsp;&emsp;max_rotate_speed|最大旋转速度 rad/s >0|number(double)||
|&emsp;&emsp;P|平移加速比例控制系数 >0|number(double)||
|&emsp;&emsp;D|平移加速微分控制系数 >0|number(double)||
|&emsp;&emsp;translation_acc|平移加（减）速度 m/s2 >0|number(double)||
|&emsp;&emsp;rotate_acc|旋转加（减）速度 rad/s2 >0|number(double)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|修改时间|string(date-time)||
|&emsp;&emsp;extend_bit|拓展布尔|string||
|&emsp;&emsp;extend_string|拓展字符串|string||
|&emsp;&emsp;features_requested|融合特征 1、开启 0、关闭|integer(int32)||
|safetyScannerRegion||integer(int32)|integer(int32)|
|weightRatio|路径权重系数|number(double)|number(double)|
|agvMapName|地图ID|string||
|pathId|路径ID|string||
|startMarkerId|开始标记点|string||
|endMarkerId|结束标记点|string||
|startControl|开始点的控制点xy坐标|string||
|endControl|结束点的控制点xy坐标|string||
|length|长度|number(double)|number(double)|
|lineType|线类型 1、直线 2、曲线（只要不为1,目前都默认为曲线）|integer(int32)|integer(int32)|
|agvDirection|agv方向: 0、双向 1、正向 2、反向|integer(int32)|integer(int32)|
|usageStatus|使用状态 ENABLE:启用  DISABLE:禁用|string||
|autoDoorId|自动门ID|string||
|directionAgv|AGV要朝向的角度（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|directionAgv2|AGV要朝向的角度2（地图坐标系下）（预留，暂不使用）  -180 ~ 180|number(double)|number(double)|
|pathType|路径类型: 0、普通路径 1、二维码对接路径 2、脱离对接路径|integer(int32)|integer(int32)|
|directionShelf|货架要朝向的角度1（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|workStationCode|工位编码|integer(int32)|integer(int32)|
|directionShelf2|货架要朝向的角度2（地图坐标系下）  -180 ~ 180|number(double)|number(double)|
|position|位置，1、起始点 2、结束点|integer(int32)|integer(int32)|
|effectivePath|生效路径 1、全部路径 2、第一段路径|integer(int32)|integer(int32)|
|rpmShelf|uint, 货架旋转速度，单位，转/每分钟|integer(int32)|integer(int32)|
|firstPath|是否是首段路径 1、是 0、否|integer(int32)|integer(int32)|
|accurateStop|是否启用末端精定位: 0不启用 1启用，默认是不启用|integer(int32)|integer(int32)|
|hasAction|是否有动作,1、有 0、没有|integer(int32)|integer(int32)|
|agvDirection2|agv方向2: -180 ~ 180|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"id": "",
	"pathParam": {
		"safety_scanner_region": 0,
		"safety": 0,
		"max_translation_speed": 0,
		"max_rotate_speed": 0,
		"P": 0,
		"D": 0,
		"translation_acc": 0,
		"rotate_acc": 0,
		"createTime": "",
		"updateTime": "",
		"extend_bit": "",
		"extend_string": "",
		"features_requested": 0
	},
	"safetyScannerRegion": 0,
	"weightRatio": 0,
	"agvMapName": "",
	"pathId": "",
	"startMarkerId": "",
	"endMarkerId": "",
	"startControl": "",
	"endControl": "",
	"length": 0,
	"lineType": 0,
	"agvDirection": 0,
	"usageStatus": "",
	"autoDoorId": "",
	"directionAgv": 0,
	"directionAgv2": 0,
	"pathType": 0,
	"directionShelf": 0,
	"workStationCode": 0,
	"directionShelf2": 0,
	"position": 0,
	"effectivePath": 0,
	"rpmShelf": 0,
	"firstPath": 0,
	"accurateStop": 0,
	"hasAction": 0,
	"agvDirection2": 0
}
```


# 通过markId 获取路径顺序


## 通过站点获取站点路径优先级,有设置起始点


**接口地址**:`/api/v3/bestWayWitchMarkId/getBestWay`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:


**请求示例**:


```javascript
[
	""
]
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|set|set|body|true|array|string|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 通过站点获取站点路径优先级,不设置起始点


**接口地址**:`/api/v3/bestWayWitchMarkId/getBestWayNoStart`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:


**请求示例**:


```javascript
[
	""
]
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|set|set|body|true|array|string|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 音频文件(audioFile)


## 下载音频文件(文件流格式)


**接口地址**:`/api/v3/audioFile/downAudio`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`*/*`


**接口描述**:根据路径获取对应的音频文件


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|url|音频文件url|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 预设任务


## 列表


**接口地址**:`/api/v3/missions`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Mission|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|code|预设任务编码|string||
|name|名称|string||
|description|描述|string||
|sequence|优先级,1:低，2：普通，3：高，4：最高. 默认是2|integer(int32)|integer(int32)|
|interrupt|是否可中断,True:任务可以被更高优级的新任务中断，False:必须执行完成后才能执行其他的任务。|boolean||
|version|预设任务版本|integer(int32)|integer(int32)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"code": "",
		"name": "自动运输任务",
		"description": "自动运输任务",
		"sequence": 2,
		"interrupt": false,
		"version": 0,
		"createTime": "",
		"updateTime": ""
	}
]
```


## 创建


**接口地址**:`/api/v3/missions`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"code": "",
	"name": "自动运输任务",
	"description": "自动运输任务",
	"sequence": 2,
	"interrupt": false,
	"version": 0,
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|mission|预设任务|body|true|Mission|Mission|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;code|预设任务编码||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;sequence|优先级,1:低，2：普通，3：高，4：最高. 默认是2||false|integer(int32)||
|&emsp;&emsp;interrupt|是否可中断,True:任务可以被更高优级的新任务中断，False:必须执行完成后才能执行其他的任务。||false|boolean||
|&emsp;&emsp;version|预设任务版本||false|integer(int32)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|Mission|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|code|预设任务编码|string||
|name|名称|string||
|description|描述|string||
|sequence|优先级,1:低，2：普通，3：高，4：最高. 默认是2|integer(int32)|integer(int32)|
|interrupt|是否可中断,True:任务可以被更高优级的新任务中断，False:必须执行完成后才能执行其他的任务。|boolean||
|version|预设任务版本|integer(int32)|integer(int32)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"code": "",
	"name": "自动运输任务",
	"description": "自动运输任务",
	"sequence": 2,
	"interrupt": false,
	"version": 0,
	"createTime": "",
	"updateTime": ""
}
```


## 分页查询


**接口地址**:`/api/v3/missions/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«Mission»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|Mission|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;code|预设任务编码|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;sequence|优先级,1:低，2：普通，3：高，4：最高. 默认是2|integer(int32)||
|&emsp;&emsp;interrupt|是否可中断,True:任务可以被更高优级的新任务中断，False:必须执行完成后才能执行其他的任务。|boolean||
|&emsp;&emsp;version|预设任务版本|integer(int32)||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"code": "",
			"name": "自动运输任务",
			"description": "自动运输任务",
			"sequence": 2,
			"interrupt": false,
			"version": 0,
			"createTime": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/missions/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|预设任务ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Mission|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|code|预设任务编码|string||
|name|名称|string||
|description|描述|string||
|sequence|优先级,1:低，2：普通，3：高，4：最高. 默认是2|integer(int32)|integer(int32)|
|interrupt|是否可中断,True:任务可以被更高优级的新任务中断，False:必须执行完成后才能执行其他的任务。|boolean||
|version|预设任务版本|integer(int32)|integer(int32)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"code": "",
	"name": "自动运输任务",
	"description": "自动运输任务",
	"sequence": 2,
	"interrupt": false,
	"version": 0,
	"createTime": "",
	"updateTime": ""
}
```


## 更新


**接口地址**:`/api/v3/missions/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:根据ID更新预设任务信息


**请求示例**:


```javascript
{
	"id": "",
	"code": "",
	"name": "自动运输任务",
	"description": "自动运输任务",
	"sequence": 2,
	"interrupt": false,
	"version": 0,
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|预设任务ID|path|true|string||
|mission|预设任务|body|true|Mission|Mission|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;code|预设任务编码||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;sequence|优先级,1:低，2：普通，3：高，4：最高. 默认是2||false|integer(int32)||
|&emsp;&emsp;interrupt|是否可中断,True:任务可以被更高优级的新任务中断，False:必须执行完成后才能执行其他的任务。||false|boolean||
|&emsp;&emsp;version|预设任务版本||false|integer(int32)||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Mission|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|code|预设任务编码|string||
|name|名称|string||
|description|描述|string||
|sequence|优先级,1:低，2：普通，3：高，4：最高. 默认是2|integer(int32)|integer(int32)|
|interrupt|是否可中断,True:任务可以被更高优级的新任务中断，False:必须执行完成后才能执行其他的任务。|boolean||
|version|预设任务版本|integer(int32)|integer(int32)|
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"code": "",
	"name": "自动运输任务",
	"description": "自动运输任务",
	"sequence": 2,
	"interrupt": false,
	"version": 0,
	"createTime": "",
	"updateTime": ""
}
```


## 删除


**接口地址**:`/api/v3/missions/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:根据ID删除预设任务信息


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|预设任务ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 根据预设任务ID查询预设任务动作列表


**接口地址**:`/api/v3/missions/{id}/missionActions`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|预设任务ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionAction|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|预设任务ID|string||
|name|名称|string||
|actionType|类型|string||
|preAction|上一个动作|string||
|nextAction|下一个动作|string||
|description|描述|string||
|parentActionId|父类动作Id|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|
|childType|子动作类型 1、IF 2、ELSE 3、WHILE|string||


**响应示例**:
```javascript
[
	{
		"id": "",
		"missionId": "",
		"name": "",
		"actionType": "",
		"preAction": "",
		"nextAction": "",
		"description": "",
		"parentActionId": "",
		"createTime": "",
		"updateTime": "",
		"childType": ""
	}
]
```


## 根据预设任务ID查询预设任务全局变量


**接口地址**:`/api/v3/missions/{id}/missionGlobalVariables`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|工作ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionGlobalVariable|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|预设任务ID|string||
|variableKey|变量键|string||
|variableValue|变量值|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"missionId": "",
		"variableKey": "",
		"variableValue": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


# 预设任务全局变量


## 列表


**接口地址**:`/api/v3/missionGlobalVariables`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionGlobalVariable|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|预设任务ID|string||
|variableKey|变量键|string||
|variableValue|变量值|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"missionId": "",
		"variableKey": "",
		"variableValue": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


## 创建


**接口地址**:`/api/v3/missionGlobalVariables`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"missionId": "",
	"variableKey": "",
	"variableValue": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|missionGlobalVariable|预设任务全局变量|body|true|MissionGlobalVariable|MissionGlobalVariable|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;missionId|预设任务ID||false|string||
|&emsp;&emsp;variableKey|变量键||false|string||
|&emsp;&emsp;variableValue|变量值||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|MissionGlobalVariable|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|预设任务ID|string||
|variableKey|变量键|string||
|variableValue|变量值|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"missionId": "",
	"variableKey": "",
	"variableValue": "",
	"createTime": "",
	"updateTime": ""
}
```


## 分页查询


**接口地址**:`/api/v3/missionGlobalVariables/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«MissionGlobalVariable»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|MissionGlobalVariable|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;missionId|预设任务ID|string||
|&emsp;&emsp;variableKey|变量键|string||
|&emsp;&emsp;variableValue|变量值|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"missionId": "",
			"variableKey": "",
			"variableValue": "",
			"createTime": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/missionGlobalVariables/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|预设任务全局变量ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionGlobalVariable|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|预设任务ID|string||
|variableKey|变量键|string||
|variableValue|变量值|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"missionId": "",
	"variableKey": "",
	"variableValue": "",
	"createTime": "",
	"updateTime": ""
}
```


## 更新


**接口地址**:`/api/v3/missionGlobalVariables/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"missionId": "",
	"variableKey": "",
	"variableValue": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|预设任务全局变量ID|path|true|string||
|missionGlobalVariable|预设任务全局变量|body|true|MissionGlobalVariable|MissionGlobalVariable|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;missionId|预设任务ID||false|string||
|&emsp;&emsp;variableKey|变量键||false|string||
|&emsp;&emsp;variableValue|变量值||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionGlobalVariable|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|预设任务ID|string||
|variableKey|变量键|string||
|variableValue|变量值|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"missionId": "",
	"variableKey": "",
	"variableValue": "",
	"createTime": "",
	"updateTime": ""
}
```


## 删除


**接口地址**:`/api/v3/missionGlobalVariables/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|预设任务全局变量ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 预设任务链


## 列表


**接口地址**:`/api/v3/missionChains`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionChain|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|missionIds|预设任务ID列表, 多个ID以逗号隔开|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"name": "",
		"missionIds": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


## 创建


**接口地址**:`/api/v3/missionChains`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"name": "",
	"missionIds": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|missionChain|预设任务链|body|true|MissionChain|MissionChain|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;missionIds|预设任务ID列表, 多个ID以逗号隔开||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|MissionChain|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|missionIds|预设任务ID列表, 多个ID以逗号隔开|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"missionIds": "",
	"createTime": "",
	"updateTime": ""
}
```


## 分页查询


**接口地址**:`/api/v3/missionChains/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«MissionChain»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|MissionChain|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;missionIds|预设任务ID列表, 多个ID以逗号隔开|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"name": "",
			"missionIds": "",
			"createTime": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/missionChains/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|预设任务链ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionChain|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|missionIds|预设任务ID列表, 多个ID以逗号隔开|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"missionIds": "",
	"createTime": "",
	"updateTime": ""
}
```


## 更新


**接口地址**:`/api/v3/missionChains/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"name": "",
	"missionIds": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|预设任务链ID|path|true|string||
|missionChain|预设任务链|body|true|MissionChain|MissionChain|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;missionIds|预设任务ID列表, 多个ID以逗号隔开||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionChain|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|name|名称|string||
|missionIds|预设任务ID列表, 多个ID以逗号隔开|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"name": "",
	"missionIds": "",
	"createTime": "",
	"updateTime": ""
}
```


## 删除


**接口地址**:`/api/v3/missionChains/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|预设任务链ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


# 预设动作


## 列表


**接口地址**:`/api/v3/missionActions`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionAction|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|预设任务ID|string||
|name|名称|string||
|actionType|类型|string||
|preAction|上一个动作|string||
|nextAction|下一个动作|string||
|description|描述|string||
|parentActionId|父类动作Id|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|
|childType|子动作类型 1、IF 2、ELSE 3、WHILE|string||


**响应示例**:
```javascript
[
	{
		"id": "",
		"missionId": "",
		"name": "",
		"actionType": "",
		"preAction": "",
		"nextAction": "",
		"description": "",
		"parentActionId": "",
		"createTime": "",
		"updateTime": "",
		"childType": ""
	}
]
```


## 创建


**接口地址**:`/api/v3/missionActions`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"missionId": "",
	"name": "",
	"actionType": "",
	"preAction": "",
	"nextAction": "",
	"description": "",
	"parentActionId": "",
	"createTime": "",
	"updateTime": "",
	"childType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|missionAction|预设动作|body|true|MissionAction|MissionAction|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;missionId|预设任务ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;actionType|类型||false|string||
|&emsp;&emsp;preAction|上一个动作||false|string||
|&emsp;&emsp;nextAction|下一个动作||false|string||
|&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;parentActionId|父类动作Id||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|&emsp;&emsp;childType|子动作类型 1、IF 2、ELSE 3、WHILE||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|MissionAction|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|预设任务ID|string||
|name|名称|string||
|actionType|类型|string||
|preAction|上一个动作|string||
|nextAction|下一个动作|string||
|description|描述|string||
|parentActionId|父类动作Id|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|
|childType|子动作类型 1、IF 2、ELSE 3、WHILE|string||


**响应示例**:
```javascript
{
	"id": "",
	"missionId": "",
	"name": "",
	"actionType": "",
	"preAction": "",
	"nextAction": "",
	"description": "",
	"parentActionId": "",
	"createTime": "",
	"updateTime": "",
	"childType": ""
}
```


## 批量更新


**接口地址**:`/api/v3/missionActions`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"missionId": "",
	"name": "",
	"actionType": "",
	"preAction": "",
	"nextAction": "",
	"description": "",
	"parentActionId": "",
	"createTime": "",
	"updateTime": "",
	"childType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|missionActions|预设动作|body|true|MissionAction|MissionAction|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;missionId|预设任务ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;actionType|类型||false|string||
|&emsp;&emsp;preAction|上一个动作||false|string||
|&emsp;&emsp;nextAction|下一个动作||false|string||
|&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;parentActionId|父类动作Id||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|&emsp;&emsp;childType|子动作类型 1、IF 2、ELSE 3、WHILE||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionAction|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|预设任务ID|string||
|name|名称|string||
|actionType|类型|string||
|preAction|上一个动作|string||
|nextAction|下一个动作|string||
|description|描述|string||
|parentActionId|父类动作Id|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|
|childType|子动作类型 1、IF 2、ELSE 3、WHILE|string||


**响应示例**:
```javascript
[
	{
		"id": "",
		"missionId": "",
		"name": "",
		"actionType": "",
		"preAction": "",
		"nextAction": "",
		"description": "",
		"parentActionId": "",
		"createTime": "",
		"updateTime": "",
		"childType": ""
	}
]
```


## 分页查询


**接口地址**:`/api/v3/missionActions/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«MissionAction»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|MissionAction|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;missionId|预设任务ID|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;actionType|类型|string||
|&emsp;&emsp;preAction|上一个动作|string||
|&emsp;&emsp;nextAction|下一个动作|string||
|&emsp;&emsp;description|描述|string||
|&emsp;&emsp;parentActionId|父类动作Id|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|&emsp;&emsp;childType|子动作类型 1、IF 2、ELSE 3、WHILE|string||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"missionId": "",
			"name": "",
			"actionType": "",
			"preAction": "",
			"nextAction": "",
			"description": "",
			"parentActionId": "",
			"createTime": "",
			"updateTime": "",
			"childType": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/missionActions/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|预设动作ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionAction|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|预设任务ID|string||
|name|名称|string||
|actionType|类型|string||
|preAction|上一个动作|string||
|nextAction|下一个动作|string||
|description|描述|string||
|parentActionId|父类动作Id|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|
|childType|子动作类型 1、IF 2、ELSE 3、WHILE|string||


**响应示例**:
```javascript
{
	"id": "",
	"missionId": "",
	"name": "",
	"actionType": "",
	"preAction": "",
	"nextAction": "",
	"description": "",
	"parentActionId": "",
	"createTime": "",
	"updateTime": "",
	"childType": ""
}
```


## 更新


**接口地址**:`/api/v3/missionActions/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"missionId": "",
	"name": "",
	"actionType": "",
	"preAction": "",
	"nextAction": "",
	"description": "",
	"parentActionId": "",
	"createTime": "",
	"updateTime": "",
	"childType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|预设动作ID|path|true|string||
|missionAction|预设动作|body|true|MissionAction|MissionAction|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;missionId|预设任务ID||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;actionType|类型||false|string||
|&emsp;&emsp;preAction|上一个动作||false|string||
|&emsp;&emsp;nextAction|下一个动作||false|string||
|&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;parentActionId|父类动作Id||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||
|&emsp;&emsp;childType|子动作类型 1、IF 2、ELSE 3、WHILE||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionAction|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionId|预设任务ID|string||
|name|名称|string||
|actionType|类型|string||
|preAction|上一个动作|string||
|nextAction|下一个动作|string||
|description|描述|string||
|parentActionId|父类动作Id|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|
|childType|子动作类型 1、IF 2、ELSE 3、WHILE|string||


**响应示例**:
```javascript
{
	"id": "",
	"missionId": "",
	"name": "",
	"actionType": "",
	"preAction": "",
	"nextAction": "",
	"description": "",
	"parentActionId": "",
	"createTime": "",
	"updateTime": "",
	"childType": ""
}
```


## 删除


**接口地址**:`/api/v3/missionActions/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|预设动作ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 根据预设动作ID查询参数列表


**接口地址**:`/api/v3/missionActions/{id}/missionActionParameters`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|动作ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionActionParameter|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionActionId|预设动作ID|string||
|parameterKey|参数Key|string||
|parameterValue|参数值|string||
|parameterValueType|参数值类型 String,Integer,Double,Long|string||
|parameterType|参数类型  NORMAL_PARAMETER:正常参数，RUNTIME_PARAMETER:动行时参数|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"missionActionId": "",
		"parameterKey": "",
		"parameterValue": "",
		"parameterValueType": "",
		"parameterType": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


# 预设动作参数


## 列表


**接口地址**:`/api/v3/missionActionParameters`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionActionParameter|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionActionId|预设动作ID|string||
|parameterKey|参数Key|string||
|parameterValue|参数值|string||
|parameterValueType|参数值类型 String,Integer,Double,Long|string||
|parameterType|参数类型  NORMAL_PARAMETER:正常参数，RUNTIME_PARAMETER:动行时参数|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
[
	{
		"id": "",
		"missionActionId": "",
		"parameterKey": "",
		"parameterValue": "",
		"parameterValueType": "",
		"parameterType": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


## 创建


**接口地址**:`/api/v3/missionActionParameters`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
{
	"id": "",
	"missionActionId": "",
	"parameterKey": "",
	"parameterValue": "",
	"parameterValueType": "",
	"parameterType": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|missionActionParameter|预设任务参数|body|true|MissionActionParameter|MissionActionParameter|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;missionActionId|预设动作ID||false|string||
|&emsp;&emsp;parameterKey|参数Key||false|string||
|&emsp;&emsp;parameterValue|参数值||false|string||
|&emsp;&emsp;parameterValueType|参数值类型 String,Integer,Double,Long||false|string||
|&emsp;&emsp;parameterType|参数类型  NORMAL_PARAMETER:正常参数，RUNTIME_PARAMETER:动行时参数||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created|MissionActionParameter|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionActionId|预设动作ID|string||
|parameterKey|参数Key|string||
|parameterValue|参数值|string||
|parameterValueType|参数值类型 String,Integer,Double,Long|string||
|parameterType|参数类型  NORMAL_PARAMETER:正常参数，RUNTIME_PARAMETER:动行时参数|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"missionActionId": "",
	"parameterKey": "",
	"parameterValue": "",
	"parameterValueType": "",
	"parameterType": "",
	"createTime": "",
	"updateTime": ""
}
```


## 批量创建


**接口地址**:`/api/v3/missionActionParameters/batch`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
[
	{
		"id": "",
		"missionActionId": "",
		"parameterKey": "",
		"parameterValue": "",
		"parameterValueType": "",
		"parameterType": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|missionActionParameters|预设任务参数|body|true|array|MissionActionParameter|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;missionActionId|预设动作ID||false|string||
|&emsp;&emsp;parameterKey|参数Key||false|string||
|&emsp;&emsp;parameterValue|参数值||false|string||
|&emsp;&emsp;parameterValueType|参数值类型 String,Integer,Double,Long||false|string||
|&emsp;&emsp;parameterType|参数类型  NORMAL_PARAMETER:正常参数，RUNTIME_PARAMETER:动行时参数||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 批量更新


**接口地址**:`/api/v3/missionActionParameters/batch`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:


**请求示例**:


```javascript
[
	{
		"id": "",
		"missionActionId": "",
		"parameterKey": "",
		"parameterValue": "",
		"parameterValueType": "",
		"parameterType": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|missionActionParameters|预设任务参数|body|true|array|MissionActionParameter|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;missionActionId|预设动作ID||false|string||
|&emsp;&emsp;parameterKey|参数Key||false|string||
|&emsp;&emsp;parameterValue|参数值||false|string||
|&emsp;&emsp;parameterValueType|参数值类型 String,Integer,Double,Long||false|string||
|&emsp;&emsp;parameterType|参数类型  NORMAL_PARAMETER:正常参数，RUNTIME_PARAMETER:动行时参数||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 删除预设动作参数列表


**接口地址**:`/api/v3/missionActionParameters/deleteBatch`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:根据ID删除预设动作参数列表


**请求示例**:


```javascript
[
	{
		"id": "",
		"missionActionId": "",
		"parameterKey": "",
		"parameterValue": "",
		"parameterValueType": "",
		"parameterType": "",
		"createTime": "",
		"updateTime": ""
	}
]
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|missionActionParameters|预设任务参数|body|true|array|MissionActionParameter|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;missionActionId|预设动作ID||false|string||
|&emsp;&emsp;parameterKey|参数Key||false|string||
|&emsp;&emsp;parameterValue|参数值||false|string||
|&emsp;&emsp;parameterValueType|参数值类型 String,Integer,Double,Long||false|string||
|&emsp;&emsp;parameterType|参数类型  NORMAL_PARAMETER:正常参数，RUNTIME_PARAMETER:动行时参数||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 分页查询


**接口地址**:`/api/v3/missionActionParameters/page`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNum|页数|query|true|string||
|pageSize|数量|query|true|string||
|sort|排序|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PageInfo«MissionActionParameter»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|endRow||integer(int32)|integer(int32)|
|firstPage||integer(int32)|integer(int32)|
|hasNextPage||boolean||
|hasPreviousPage||boolean||
|isFirstPage||boolean||
|isLastPage||boolean||
|lastPage||integer(int32)|integer(int32)|
|list||array|MissionActionParameter|
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;missionActionId|预设动作ID|string||
|&emsp;&emsp;parameterKey|参数Key|string||
|&emsp;&emsp;parameterValue|参数值|string||
|&emsp;&emsp;parameterValueType|参数值类型 String,Integer,Double,Long|string||
|&emsp;&emsp;parameterType|参数类型  NORMAL_PARAMETER:正常参数，RUNTIME_PARAMETER:动行时参数|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|navigateFirstPage||integer(int32)|integer(int32)|
|navigateLastPage||integer(int32)|integer(int32)|
|navigatePages||integer(int32)|integer(int32)|
|navigatepageNums||array||
|nextPage||integer(int32)|integer(int32)|
|pageNum||integer(int32)|integer(int32)|
|pageSize||integer(int32)|integer(int32)|
|pages||integer(int32)|integer(int32)|
|prePage||integer(int32)|integer(int32)|
|size||integer(int32)|integer(int32)|
|startRow||integer(int32)|integer(int32)|
|total||integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"endRow": 0,
	"firstPage": 0,
	"hasNextPage": true,
	"hasPreviousPage": true,
	"isFirstPage": true,
	"isLastPage": true,
	"lastPage": 0,
	"list": [
		{
			"id": "",
			"missionActionId": "",
			"parameterKey": "",
			"parameterValue": "",
			"parameterValueType": "",
			"parameterType": "",
			"createTime": "",
			"updateTime": ""
		}
	],
	"navigateFirstPage": 0,
	"navigateLastPage": 0,
	"navigatePages": 0,
	"navigatepageNums": [],
	"nextPage": 0,
	"pageNum": 0,
	"pageSize": 0,
	"pages": 0,
	"prePage": 0,
	"size": 0,
	"startRow": 0,
	"total": 0
}
```


## 详情


**接口地址**:`/api/v3/missionActionParameters/{id}`


**请求方式**:`GET`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|预设动作参数ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionActionParameter|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionActionId|预设动作ID|string||
|parameterKey|参数Key|string||
|parameterValue|参数值|string||
|parameterValueType|参数值类型 String,Integer,Double,Long|string||
|parameterType|参数类型  NORMAL_PARAMETER:正常参数，RUNTIME_PARAMETER:动行时参数|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"missionActionId": "",
	"parameterKey": "",
	"parameterValue": "",
	"parameterValueType": "",
	"parameterType": "",
	"createTime": "",
	"updateTime": ""
}
```


## 更新


**接口地址**:`/api/v3/missionActionParameters/{id}`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`application/json`


**接口描述**:根据ID更新动作参数信息


**请求示例**:


```javascript
{
	"id": "",
	"missionActionId": "",
	"parameterKey": "",
	"parameterValue": "",
	"parameterValueType": "",
	"parameterType": "",
	"createTime": "",
	"updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|预设动作参数ID|path|true|string||
|missionActionParameter|预设任务参数|body|true|MissionActionParameter|MissionActionParameter|
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;missionActionId|预设动作ID||false|string||
|&emsp;&emsp;parameterKey|参数Key||false|string||
|&emsp;&emsp;parameterValue|参数值||false|string||
|&emsp;&emsp;parameterValueType|参数值类型 String,Integer,Double,Long||false|string||
|&emsp;&emsp;parameterType|参数类型  NORMAL_PARAMETER:正常参数，RUNTIME_PARAMETER:动行时参数||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MissionActionParameter|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|id|ID|string||
|missionActionId|预设动作ID|string||
|parameterKey|参数Key|string||
|parameterValue|参数值|string||
|parameterValueType|参数值类型 String,Integer,Double,Long|string||
|parameterType|参数类型  NORMAL_PARAMETER:正常参数，RUNTIME_PARAMETER:动行时参数|string||
|createTime|创建时间|string(date-time)|string(date-time)|
|updateTime|更新时间|string(date-time)|string(date-time)|


**响应示例**:
```javascript
{
	"id": "",
	"missionActionId": "",
	"parameterKey": "",
	"parameterValue": "",
	"parameterValueType": "",
	"parameterType": "",
	"createTime": "",
	"updateTime": ""
}
```


## 删除


**接口地址**:`/api/v3/missionActionParameters/{id}`


**请求方式**:`DELETE`


**请求数据类型**:`*`


**响应数据类型**:`application/json`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | in    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|预设动作参数ID|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


暂无


**响应示例**:
```javascript

```