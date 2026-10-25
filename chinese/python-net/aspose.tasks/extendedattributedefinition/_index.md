---
title: "ExtendedAttributeDefinition"
second_title: "适用于 Python via .NET 的 Aspose.Tasks API 参考"
description: 
type: docs
weight: 310
url: /zh/python-net/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

表示与项目关联的扩展属性定义。

ExtendedAttributeDefinition 类型公开以下成员：
## 属性
| 名称 | 描述 |
| :- | :- |
| field_id | 获取或设置对应于自定义字段的项目 ID。<br/>            使用来自 [ExtendedAttributeTask](/tasks/python-net/aspose.tasks/extendedattributetask/) 类的常量的字符串表示来指定 [field_id](/tasks/python-net/aspose.tasks/extendedattributedefinition/) 属性。 |
| field_name | 获取自定义字段的名称。 |
| cf_type | 获取自定义字段的类型。 |
| guid | 获取或设置自定义字段的 Guid。 |
| element_type | 获取或设置扩展属性与<br/>            任务、资源或分配关联。 |
| max_multi_values | 获取或设置在选择列表中可以设置的最大值数量。 |
| user_def | 获取或设置一个值，用于指示自定义字段是否由用户定义。 |
| alias | 获取或设置自定义字段的别名。 |
| secondary_pid | 获取或设置自定义字段的次要 PID。 |
| auto_roll_down | 获取或设置一个值，指示是否启用了自动向下滚动到分配。 |
| default_guid | 获取或设置默认查找表条目的 Guid。 |
| lookup_uid | 获取与自定义字段关联的查找表的 Guid。 |
| phonetics_alias | 获取或设置自定义字段别名的拼音发音。 |
| rollup_type | 获取或设置汇总的计算方式。 |
| calculation_type | 获取或设置自定义属性值的计算类型。 |
| summary_rows_calculation_type | 获取或设置汇总行中自定义属性值的计算类型。 |
| formula | 获取或设置 Microsoft Project 用于填充自定义任务字段的公式。 |
| graphical_indicator | 获取或设置与扩展属性关联的图形指示器信息。<br/>            适用于 MPP 格式。 |
| restrict_values | 获取或设置一个值，指示自定义字段值是否受限于 [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/) 中的值。 |
| valuelist_sort_order | 获取或设置值列表的排序方式。取值为：0=降序，1=升序。 |
| append_new_values | 获取或设置一个值，指示添加到项目的新值是否会自动添加到列表中。 |
| default | 获取或设置列表中的默认值。 |
| value_list | 获取 List<Value> ValueList。 |
| secondary_guid | 获取或设置扩展属性的次要 guid。 |
| parent_project | 获取 [ExtendedAttributeDefinition](/tasks/python-net/aspose.tasks/extendedattributedefinition/) 实例的父项目。 |
## Methods
| 名称 | 描述 |
| :- | :- |
| create_extended_attribute() | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值。 |
| create_extended_attribute(text_value) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并使用指定的文本值。 |
| create_extended_attribute(numeric_value) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并使用指定的数值。 |
| create_extended_attribute(date_time_value) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并使用指定的日期值。 |
| create_extended_attribute(duration_value) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并使用指定的持续时间值。 |
| create_extended_attribute(flag_value) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并使用指定的标志值。 |
| create_extended_attribute(lookup_value) | 创建与指定的 [Value](/tasks/python-net/aspose.tasks/value/) 项关联的新扩展属性。 |
| create_task_definition(custom_field_type, field_id, alias) | 工厂方法用于创建一个简单的扩展属性定义，Microsoft Project 将其显示为 “None”。<br/>            它的 [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) 等于 [NONE](/tasks/python-net/aspose.tasks/calculationtype/)，且只能在任务中使用。<br/>            您需要指定 |
| create_task_definition(field_id, alias) | 工厂方法用于创建一个简单的扩展属性定义，Microsoft Project 将其显示为 “None”。<br/>            它的 [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) 等于 [NONE](/tasks/python-net/aspose.tasks/calculationtype/)，且只能在任务中使用。<br/>            您需要指定 |
| create_resource_definition(custom_field_type, field_id, alias) | 工厂方法用于创建一个简单的扩展属性定义，Microsoft Project 将其显示为 “None”。<br/>            它的 [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) 等于 [NONE](/tasks/python-net/aspose.tasks/calculationtype/)，且只能在资源中使用。<br/>            您需要指定 |
| create_resource_definition(field_id, alias) | 工厂方法用于创建一个简单的扩展属性定义，Microsoft Project 将其显示为 “None”。<br/>            它的 [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) 等于 [NONE](/tasks/python-net/aspose.tasks/calculationtype/)，且只能在资源中使用。<br/>            您需要指定 |
| create_lookup_task_definition(field_id, alias) | 工厂方法用于创建带查找的扩展属性定义。<br/>            它的 [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) 等于 [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/)，且只能在任务中使用。<br/>            您需要指定 |
| create_lookup_task_definition(custom_field_type, field_id, alias) | 工厂方法用于创建带查找的扩展属性定义。<br/>            它的 [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) 等于 [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/)，且只能在任务中使用。<br/>            您需要指定 |
| create_lookup_resource_definition(field_id, alias) | 工厂方法用于创建带查找的扩展属性定义。<br/>            它的 [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) 等于 [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/)，且只能在资源中使用。<br/>            您需要指定 |
| create_lookup_resource_definition(custom_field_type, field_id, alias) | 工厂方法用于创建带查找的扩展属性定义。<br/>            它的 [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) 等于 [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/)，且只能在资源中使用。<br/>            您需要指定 |
| add_lookup_value(value) | 向内部查找列表添加一个值。这是对 [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/) 进行操作的首选方式。 |
| remove_lookup_value(value) | 从内部查找列表中移除一个值。这是对 [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/) 进行操作的首选方式。 |

### 另见

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

