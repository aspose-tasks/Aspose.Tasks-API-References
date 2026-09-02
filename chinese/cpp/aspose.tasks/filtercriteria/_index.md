---
title: "Aspose::Tasks::FilterCriteria 类"
linktitle: "FilterCriteria"
articleTitle: "FilterCriteria"
second_title: "Aspose.Tasks for C++"
description: "定义任务或资源必须满足的标准，以便在 MSP 视图中显示。"
type: docs
weight: 10
url: /zh/cpp/aspose.tasks/filtercriteria/
---

## FilterCriteria class

定义任务或资源必须满足的标准，以便在 MSP 视图中显示。

## 方法

| 表示 ResourceAssignment 对象的属性。 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| [get_CriteriaRows](./get_criteriarows/) | 获取子 FilterCriteria 行的列表。如果过滤器包含多个条件行，则 And 运算符的效果是必须同时满足两行的条件，任务或资源才能作为此过滤器的结果显示。Or 运算符的效果是只需满足其中一行的条件即可。 |
| [get_Field](./get_field/) | 获取要更改的字段。 |
| [get_Operation](./get_operation/) | 获取使用 FieldName、Test 和 Value 建立的准则，该准则与过滤器中的其他准则相关。 |
| [get_Test](./get_test/) | 获取在 FieldName 与 Value 之间进行的比较类型，该类型作为过滤器的选择准则。FilterComparisonType |
| [get_Values](./get_values/) | 获取用于与由 FieldName 指定的字段值进行比较的对象值。 |
| [IsFieldValue](./isfieldvalue/) | 获取 FilterCriteria 的右侧值是否为字段引用，而非常量值。 |
| [set_Field](./set_field/) | 设置要更改的字段。 |
| [set_Operation](./set_operation/) | 设置使用 FieldName、Test 和 Value 建立的准则，使其与过滤器中的其他准则相关。 |
| [set_Test](./set_test/) | 设置在 FieldName 与 Value 之间进行的比较类型，该类型作为过滤器的选择准则。FilterComparisonType |
| [SetValueField](./setvaluefield/) | 设置其值将与由 FieldName 指定的字段值进行比较的字段。 |
| [ToString](./tostring/) | 返回 FilterCriteria 类实例的字符串表示形式。 |

