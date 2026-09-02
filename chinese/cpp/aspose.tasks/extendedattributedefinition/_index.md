---
title: "Aspose::Tasks::ExtendedAttributeDefinition 类"
linktitle: "ExtendedAttributeDefinition"
articleTitle: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks for C++"
description: "表示与项目关联的扩展属性定义。"
type: docs
weight: 10
url: /zh/cpp/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

表示与项目关联的扩展属性定义。

## 方法

| 表示 ResourceAssignment 对象的属性。 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| [AddLookupValue](./addlookupvalue/) | 向内部查找列表添加一个值。这是对 ValueList 进行操作的首选方式。 |
| [CreateExtendedAttribute (7 overloads)](./createextendedattribute/) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值。 |
| [CreateLookupResourceDefinition (2 overloads)](./createlookupresourcedefinition/) | 工厂方法，用于创建带查找的扩展属性定义。其 CalculationType 等于 Tasks::CalculationType::Lookup，并且只能在 Resources 中使用。调用此方法时需要指定 customFieldType、fieldId 和 alias。 |
| [CreateLookupTaskDefinition (2 overloads)](./createlookuptaskdefinition/) | 工厂方法，用于创建带查找的扩展属性定义。其 CalculationType 等于 Tasks::CalculationType::Lookup，并且只能在 Tasks 中使用。调用此方法时需要指定 customFieldType、fieldId 和 alias。 |
| [CreateResourceDefinition (2 overloads)](./createresourcedefinition/) | 工厂方法，用于创建简单的扩展属性定义，Microsoft Project 将其显示为 “None”。其 CalculationType 等于 Tasks::CalculationType::None，并且只能在 Resource 中使用。调用此方法时需要指定 customFieldType、fieldId 和 alias。 |
| [CreateTaskDefinition (2 overloads)](./createtaskdefinition/) | 工厂方法，用于创建简单的扩展属性定义，Microsoft Project 将其显示为 “None”。其 CalculationType 等于 Tasks::CalculationType::None，并且只能在 Tasks 中使用。调用此方法时需要指定 customFieldType、fieldId 和 alias。 |
| [Equals](./equals/) | 返回一个标志，指示此实例是否等于指定的对象。 |
| [get_Alias](./get_alias/) | 获取自定义字段的别名。 |
| [get_AppendNewValues](./get_appendnewvalues/) | 获取一个值，指示添加到项目的新值是否会自动添加到列表中。 |
| [get_AutoRollDown](./get_autorolldown/) | 获取一个值，指示是否启用了自动向分配下放。 |
| [get_CalculationType](./get_calculationtype/) | 获取自定义属性值的计算类型。 |
| [get_CfType](./get_cftype/) | 获取自定义字段的类型。 |
| [get_Default](./get_default/) | 获取列表中的默认值。 |
| [get_DefaultGuid](./get_defaultguid/) | 获取默认查找表条目的 Guid。 |
| [get_ElementType](./get_elementtype/) | 获取扩展属性是否与任务、资源或分配关联。 |
| [get_FieldId](./get_fieldid/) | 获取对应于自定义字段的项目 ID。使用 Aspose::Tasks::ExtendedAttributeTask 类中常量的字符串表示来指定 FieldId 属性。 |
| [get_FieldName](./get_fieldname/) | 获取自定义字段的名称。 |
| [get_Formula](./get_formula/) | 获取 Microsoft Project 用于填充自定义任务字段的公式。 |
| [get_GraphicalIndicator](./get_graphicalindicator/) | 获取与扩展属性关联的图形指示器信息。适用于 MPP 格式。 |
| [get_Guid](./get_guid/) | 获取自定义字段的 Guid。 |
| [get_LookupUid](./get_lookupuid/) | 获取与自定义字段关联的查找表的 Guid。 |
| [get_MaxMultiValues](./get_maxmultivalues/) | 获取在选择列表中可以设置的最大值数量。 |
| [get_ParentProject](./get_parentproject/) | 获取 ExtendedAttributeDefinition 实例的父项目。 |
| [get_PhoneticsAlias](./get_phoneticsalias/) | 获取自定义字段别名的音标发音。 |
| [get_RestrictValues](./get_restrictvalues/) | 获取一个值，指示自定义字段的值是否受限于 ValueList 中的值。 |
| [get_RollupType](./get_rolluptype/) | 获取汇总的计算方式。 |
| [get_SecondaryGuid](./get_secondaryguid/) | 获取扩展属性的次要 guid。 |
| [get_SecondaryPid](./get_secondarypid/) | 获取自定义字段的次要 PID。 |
| [get_SummaryRowsCalculationType](./get_summaryrowscalculationtype/) | 获取汇总行中自定义属性值的计算类型。 |
| [get_UserDef](./get_userdef/) | 获取一个值，指示自定义字段是否为用户定义。 |
| [get_ValueList](./get_valuelist/) | 获取 List< Value > ValueList。 |
| [get_ValuelistSortOrder](./get_valuelistsortorder/) | 获取值列表的排序方式。值为：0=降序，1=升序。 |
| [GetHashCode](./gethashcode/) | 返回 ExtendedAttributeDefinition 类实例的哈希码。 |
| [RemoveLookupValue](./removelookupvalue/) | 从内部查找列表中移除一个值。这是对 ValueList 进行操作的首选方式。 |
| [set_Alias](./set_alias/) | 设置自定义字段的别名。 |
| [set_AppendNewValues](./set_appendnewvalues/) | 设置一个值，指示是否将新添加到项目的值自动加入列表。 |
| [set_AutoRollDown](./set_autorolldown/) | 设置一个值，指示是否启用对任务分配的自动向下滚动。 |
| [set_CalculationType](./set_calculationtype/) | 设置自定义属性值的计算类型。 |
| [set_Default](./set_default/) | 设置列表中的默认值。 |
| [set_DefaultGuid](./set_defaultguid/) | 设置默认查找表条目的 Guid。 |
| [set_ElementType](./set_elementtype/) | 设置扩展属性与任务、资源或分配关联。 |
| [set_FieldId](./set_fieldid/) | 设置对应于自定义字段的项目 ID。使用来自 Aspose::Tasks::ExtendedAttributeTask 类的常量的字符串表示来指定 FieldId 属性。 |
| [set_Formula](./set_formula/) | 设置 Microsoft Project 用于填充自定义任务字段的公式。 |
| [set_GraphicalIndicator](./set_graphicalindicator/) | 设置与扩展属性关联的图形指示器信息。适用于 MPP 格式。 |
| [set_Guid](./set_guid/) | 设置自定义字段的 Guid。 |
| [set_MaxMultiValues](./set_maxmultivalues/) | 设置在下拉列表中可以设置的最大值数量。 |
| [set_PhoneticsAlias](./set_phoneticsalias/) | 设置自定义字段别名的拼音发音。 |
| [set_RestrictValues](./set_restrictvalues/) | 设置一个值，指示自定义字段值是否受限于 ValueList 中的值。 |
| [set_RollupType](./set_rolluptype/) | 设置汇总的计算方式。 |
| [set_SecondaryGuid](./set_secondaryguid/) | 设置扩展属性的次要 guid。 |
| [set_SecondaryPid](./set_secondarypid/) | 设置自定义字段的次要 PID。 |
| [set_SummaryRowsCalculationType](./set_summaryrowscalculationtype/) | 设置汇总行中自定义属性值的计算类型。 |
| [set_UserDef](./set_userdef/) | 设置一个值，指示自定义字段是否为用户定义。 |
| [set_ValuelistSortOrder](./set_valuelistsortorder/) | 设置值列表的排序方式。取值为：0=降序，1=升序。 |

