---
title: "TimephasedData"
second_title: "适用于 Python via .NET 的 Aspose.Tasks API 参考"
description: 
type: docs
weight: 1270
url: /zh/python-net/aspose.tasks/timephaseddata/
---

## TimephasedData class

表示时间分段数据。

TimephasedData 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| TimephasedData() | 初始化 [TimephasedData](/tasks/python-net/aspose.tasks/timephaseddata/) 类的新实例。 |
## 属性
| 名称 | 描述 |
| :- | :- |
| value_to_units | 获取表示此对象基于单位的时间分段数据的字符串值的 float 实例。 |
| uid | 获取或设置时间分段数据的唯一标识符。 |
| 开始 | 获取或设置时间分段数据期间的开始日期。 |
| finish | 获取或设置时间分段数据期间的结束日期。 |
| unit | 获取或设置时间分段数据期间的时间单位。 |
| timephased_data_type | 获取或设置时间分段数据的类型。 |
| value | 获取或设置时间分段数据期间的每单位时间的值。 |
| value_to_duration | 获取表示此对象字符串值的 datatime 实例。 |
| value_to_cost | 获取表示此对象字符串值的 float 实例。 |
## Methods
| 名称 | 描述 |
| :- | :- |
| create_cost_timephased(uid, start, finish, value, time_unit, type) |  |
| create_cost_timephased(uid, start, finish, value, type) |  |
| create_work_timephased(uid, start, finish, value, time_unit, type) | 创建并初始化一个新的 [TimephasedData](/tasks/python-net/aspose.tasks/timephaseddata/) 类实例，用于基于工作的时间分段数据。 |
| create_unit_timephased(uid, start, finish, units, type) | 创建并初始化一个新的 [TimephasedData](/tasks/python-net/aspose.tasks/timephaseddata/) 类实例，用于材料资源分配的基于单位的时间分段数据。 |

### 另见

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

