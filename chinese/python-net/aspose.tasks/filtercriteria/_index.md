---
title: "FilterCriteria"
second_title: "适用于 Python via .NET 的 Aspose.Tasks API 参考"
description: 
type: docs
weight: 350
url: /zh/python-net/aspose.tasks/filtercriteria/
---

## FilterCriteria class

定义任务或资源必须满足的标准，以便在 MSP 视图中显示。

FilterCriteria 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| FilterCriteria() | 初始化 FilterCriteria 类的新实例 |
## 属性
| 名称 | 描述 |
| :- | :- |
| 操作 | 获取或设置使用 FieldName、Test 和 Value 建立的准则，该准则与过滤器中的其他准则相关。 |
| field | 获取或设置一个 [field](/tasks/python-net/aspose.tasks/filtercriteria/) 进行更改。 |
| test | 获取或设置在 FieldName 和 Value 之间进行的比较类型，该类型作为过滤器的选择准则。<br/>            [FilterComparisonType](/tasks/python-net/aspose.tasks/filtercomparisontype/) |
| values | 获取用于与由 FieldName 指定的字段值进行比较的对象值。 |
| criteria_rows | 获取子 [FilterCriteria](/tasks/python-net/aspose.tasks/filtercriteria/) 行的列表。<br/>            如果过滤器包含多个准则行，则 And 运算符的作用是必须满足两行的准则，任务或资源才会作为此过滤器的结果显示。<br/>            Or 运算符的作用是必须满足其中一行的准则。 |
## Methods
| 名称 | 描述 |
| :- | :- |
| is_field_value() | 获取 FilterCriteria 的右侧值是否为字段引用，而非常量值。 |
| set_value_field(value) | 设置其值将与由 FieldName 指定的字段值进行比较的字段。 |

### 另见

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

