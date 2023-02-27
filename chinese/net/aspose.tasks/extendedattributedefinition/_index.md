---
title: Class ExtendedAttributeDefinition
second_title: Aspose.Tasks for .NET API 参考
description: Aspose.Tasks.ExtendedAttributeDefinition 班级. 表示与项目关联的扩展属性定义
type: docs
weight: 540
url: /zh/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

表示与项目关联的扩展属性定义。

```csharp
public class ExtendedAttributeDefinition
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias/) { get; set; } | 获取或设置自定义字段的别名。 |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues/) { get; set; } | 获取或设置一个值，该值指示添加到项目的新值是否自动添加到列表中。 |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown/) { get; set; } | 获取或设置一个值，该值指示是否启用自动向下滚动到分配。 |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype/) { get; set; } | 获取或设置自定义属性值的计算类型。 |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype/) { get; } | 获取自定义字段的类型。 |
| [Default](../../aspose.tasks/extendedattributedefinition/default/) { get; set; } | 获取或设置列表中的默认值。 |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid/) { get; set; } | 获取或设置默认查找表条目的 Guid。 |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype/) { get; set; } | 获取或设置扩展属性关联 任务、资源或分配。 |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid/) { get; set; } | 获取或设置对应自定义字段的项目id。 使用常量的字符串表示来自[`ExtendedAttributeTask`](../extendedattributetask/)要指定的类[`FieldId`](./fieldid/)财产. |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname/) { get; } | 获取自定义字段的名称。 |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula/) { get; set; } | 获取或设置 Microsoft Project 用于填充自定义任务字段的公式。 |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid/) { get; set; } | 获取或设置自定义字段的 Guid。 |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid/) { get; } | 获取与自定义字段关联的查找表的 Guid。 |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues/) { get; set; } | 获取或设置您可以在选择列表中设置的最大值数。 |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject/) { get; } | 获取父项目`ExtendedAttributeDefinition`实例. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias/) { get; set; } | 获取或设置自定义字段别名的拼音 |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues/) { get; set; } | 获取或设置一个值，该值指示自定义字段值是否限制为[`ValueList`](./valuelist/). |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype/) { get; set; } | 获取或设置汇总的计算方式。 |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid/) { get; set; } | 获取或设置扩展属性的辅助 guid。 |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid/) { get; set; } | 获取或设置自定义字段的辅助 PID。 |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/) { get; set; } | 获取或设置汇总行的自定义属性值的计算类型。 |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef/) { get; set; } | 获取或设置一个值，该值指示自定义字段是否为用户定义。 |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist/) { get; } | 获取 List&lt;Value&gt; ValueList. |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder/) { get; set; } | 获取或设置值列表的排序方式。值为：0=降序，1=升序。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | 使用查找创建扩展属性定义的工厂方法。 它有[`CalculationType`](./calculationtype/)等于Lookup并且只能在资源中使用。 您需要指定*fieldId*和*alias*当调用这个方法时。 字段类型是从字段id推断出来的。 |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | 使用查找创建扩展属性定义的工厂方法。 它有[`CalculationType`](./calculationtype/)等于Lookup并且只能在资源中使用。 您需要指定*customFieldType*,*fieldId*和*alias*调用此方法时. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | 使用查找创建扩展属性定义的工厂方法。 它有[`CalculationType`](./calculationtype/)等于Lookup并且只能在任务中使用。 您需要指定*fieldId*和*alias*当调用这个方法时。 字段类型是从字段id推断出来的。 |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | 使用查找创建扩展属性定义的工厂方法。 它有[`CalculationType`](./calculationtype/)等于Lookup并且只能在任务中使用。 您需要指定*customFieldType*,*fieldId*和*alias*调用此方法时. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition_1)(ExtendedAttributeResource, string) | 创建简单扩展属性定义的工厂方法，Microsoft Project 显示为“无”。 它具有[`CalculationType`](./calculationtype/)等于None并且只能在资源中使用。 您需要指定*fieldId*和*alias*当调用这个方法时。 字段类型是从字段id推断出来的。 |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | 创建简单扩展属性定义的工厂方法，Microsoft Project 显示为“无”。 它具有[`CalculationType`](./calculationtype/)等于None并且只能在资源中使用。 您需要指定*customFieldType*,*fieldId*和*alias*调用此方法时. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition_1)(ExtendedAttributeTask, string) | 创建简单扩展属性定义的工厂方法，Microsoft Project 显示为“无”。 它具有[`CalculationType`](./calculationtype/)等于None并且只能在任务中使用。 您需要指定*fieldId*和*alias*调用这个方法时。 字段类型是从字段id推断出来的。 |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | 创建简单扩展属性定义的工厂方法，Microsoft Project 显示为“无”。 它具有[`CalculationType`](./calculationtype/)等于None并且只能在任务中使用。 您需要指定*customFieldType*,*fieldId*和*alias*调用此方法时. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue/)(Value) | 向内部查找列表添加一个值。这是使用[`ValueList`](./valuelist/). |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute)() | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值。 |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_3)(bool) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值和指定的标志值。 |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_4)(DateTime) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值和指定的日期值。 |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_5)(decimal) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值和指定的数值。 |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_1)(Duration) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值和指定的持续时间值。 |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_6)(string) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值和指定的文本值。 |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_2)(Value) | 创建与指定链接的新扩展属性[`Value`](../value/)项目. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals/)(object) | 返回一个标志，指示此实例是否等于指定对象。 |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode/)() | 返回实例的哈希码`ExtendedAttributeDefinition`类. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue/)(Value) | 从内部查找列表中删除一个值。这是使用[`ValueList`](./valuelist/). |

### 也可以看看

* 命名空间 [Aspose.Tasks](../../aspose.tasks/)
* 部件 [Aspose.Tasks](../../)


