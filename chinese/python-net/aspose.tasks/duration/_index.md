---
title: "Duration"
second_title: "适用于 Python via .NET 的 Aspose.Tasks API 参考"
description: 
type: docs
weight: 260
url: /zh/python-net/aspose.tasks/duration/
---

## Duration class

表示项目中的持续时间。

Duration 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| Duration() | 初始化 Duration 类的新实例 |
## 属性
| 名称 | 描述 |
| :- | :- |
| time_span | 获取此 Duration 对象的 [time_span](/tasks/python-net/aspose.tasks/duration/) 实例。 |
| time_unit | 获取此对象的时间单位类型。 |
| is_estimated | 获取指示时间单位是否为估计的值。 |
| is_elapsed | 获取指示时间单位是否已过去的值。 |
## Methods
| 名称 | 描述 |
| :- | :- |
| add(d) | 将指定的持续时间添加到此持续时间。 |
| add(val) | 将指定的 double 值添加到此持续时间。 |
| subtract(d) | 从此持续时间实例中减去指定的持续时间。 |
| subtract(val) | 从此持续时间实例中减去指定的 double 值。 |
| parse(p, value) | 将指定的字符串转换为 [Duration](/tasks/python-net/aspose.tasks/duration/) 结构的实例。 |
| parse_time_span(value) | 解析格式为 "PT--H--M--S--" 的持续时间字符串。 |
| to_double() | 将 Duration 对象转换为 float 值。 |
| convert(time_unit_type) | 将 Duration 对象转换为具有指定时间单位的另一个持续时间。 |
| equals(other) | 返回一个值，指示此实例是否等于指定的对象。 |

### 另见

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

