---
title: "类 ExtendedAttributeDefinition"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ExtendedAttributeDefinition 类。表示与项目关联的扩展属性定义。"
type: docs
weight: 540
url: /zh/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

表示与项目关联的扩展属性定义。

```csharp
public class ExtendedAttributeDefinition
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias/) { get; set; } | 获取或设置自定义字段的别名。 |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues/) { get; set; } | 获取或设置一个值，指示是否将添加到项目的新值自动加入列表。 |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown/) { get; set; } | 获取或设置一个值，指示是否启用自动向分配下放。 |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype/) { get; set; } | 获取或设置自定义属性值的计算类型。 |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype/) { get; } | 获取自定义字段的类型。 |
| [Default](../../aspose.tasks/extendedattributedefinition/default/) { get; set; } | 获取或设置列表中的默认值。 |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid/) { get; set; } | 获取或设置默认查找表条目的 Guid。 |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype/) { get; set; } | 获取或设置扩展属性是否关联到任务、资源或分配。 |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid/) { get; set; } | 获取或设置对应于自定义字段的项目 ID。使用来自 [`ExtendedAttributeTask`](../extendedattributetask/) 类的常量的字符串表示来指定 [`FieldId`](./fieldid/) 属性。 |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname/) { get; } | 获取自定义字段的名称。 |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula/) { get; set; } | 获取或设置 Microsoft Project 用于填充自定义任务字段的公式。 |
| [GraphicalIndicator](../../aspose.tasks/extendedattributedefinition/graphicalindicator/) { get; set; } | 获取或设置与扩展属性关联的图形指示器信息。适用于 MPP 格式。 |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid/) { get; set; } | 获取或设置自定义字段的 Guid。 |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid/) { get; } | 获取与自定义字段关联的查找表的 Guid。 |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues/) { get; set; } | 获取或设置在选择列表中可以设置的最大值数量。 |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject/) { get; } | 获取 `ExtendedAttributeDefinition` 实例的父项目。 |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias/) { get; set; } | 获取或设置自定义字段别名的拼音发音。 |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues/) { get; set; } | 获取或设置一个值，指示自定义字段的值是否受限于 [`ValueList`](./valuelist/) 中的值。 |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype/) { get; set; } | 获取或设置汇总的计算方式。 |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid/) { get; set; } | 获取或设置扩展属性的次要 guid。 |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid/) { get; set; } | 获取或设置自定义字段的次要 PID。 |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/) { get; set; } | 获取或设置汇总行中自定义属性值的计算类型。 |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef/) { get; set; } | 获取或设置一个值，指示自定义字段是否为用户定义。 |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist/) { get; } | 获取 List&lt;Value&gt; ValueList。 |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder/) { get; set; } | 获取或设置值列表的排序方式。取值为：0=降序，1=升序。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | 工厂方法，用于创建带查找的扩展属性定义。其 [`CalculationType`](./calculationtype/) 等于 Lookup，仅可在资源中使用。调用此方法时必须指定 *fieldId* 和 *alias*。字段类型根据字段 ID 推断。 |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | 工厂方法，用于创建带查找的扩展属性定义。其 [`CalculationType`](./calculationtype/) 等于 Lookup，仅可在资源中使用。调用此方法时必须指定 *customFieldType*、*fieldId* 和 *alias*。 |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | 工厂方法，用于创建带查找的扩展属性定义。其 [`CalculationType`](./calculationtype/) 等于 Lookup，仅可在任务中使用。调用此方法时必须指定 *fieldId* 和 *alias*。字段类型根据字段 ID 推断。 |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | 工厂方法，用于创建带查找的扩展属性定义。其 [`CalculationType`](./calculationtype/) 等于 Lookup，仅可在任务中使用。调用此方法时必须指定 *customFieldType*、*fieldId* 和 *alias*。 |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition_1)(ExtendedAttributeResource, string) | 工厂方法，用于创建简单的扩展属性定义，Microsoft Project 将其显示为 “None”。其 [`CalculationType`](./calculationtype/) 等于 None，仅可在资源中使用。调用此方法时必须指定 *fieldId* 和 *alias*。字段类型根据字段 ID 推断。 |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | 工厂方法，用于创建简单的扩展属性定义，Microsoft Project 将其显示为 “None”。其 [`CalculationType`](./calculationtype/) 等于 None，仅可在资源中使用。调用此方法时必须指定 *customFieldType*、*fieldId* 和 *alias*。 |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition_1)(ExtendedAttributeTask, string) | 工厂方法，用于创建简单的扩展属性定义，Microsoft Project 将其显示为 “None”。其 [`CalculationType`](./calculationtype/) 等于 None，仅可在任务中使用。调用此方法时必须指定 *fieldId* 和 *alias*。字段类型根据字段 ID 推断。 |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | 工厂方法，用于创建简单的扩展属性定义，Microsoft Project 将其显示为 “None”。其 [`CalculationType`](./calculationtype/) 等于 None，仅可在任务中使用。调用此方法时必须指定 *customFieldType*、*fieldId* 和 *alias*。 |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue/)(Value) | 向内部查找列表添加一个值。这是操作 [`ValueList`](./valuelist/) 的首选方式。 |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute)() | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值。 |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_3)(bool) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并且具有指定的标志值。 |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_4)(DateTime) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并且具有指定的日期值。 |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_5)(decimal) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并且具有指定的数值。 |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_1)(Duration) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并且具有指定的持续时间值。 |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_6)(string) | 创建一个新的扩展属性，其字段 ID 等于此对象的字段 ID 值，并且具有指定的文本值。 |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_2)(Value) | 创建与指定的[`Value`](../value/)项链接的新扩展属性。 |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals/)(object) | 返回一个标志，指示此实例是否等于指定的对象。 |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode/)() | 返回 `ExtendedAttributeDefinition` 类实例的哈希码。 |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue/)(Value) | 从内部查找列表中移除一个值。这是对[`ValueList`](./valuelist/)进行操作的首选方式。 |

## 示例

展示如何在扩展属性中使用常用数学函数。

```csharp
public static void EvaluateChoose()
{
    var project = CreateTestProjectWithCustomField();

    // 设置公式
    project.ExtendedAttributes[0].Formula = "Choose(3, \"This is a\", \"right\", \"choice\")";

    // 打印扩展属性值
    var task = project.RootTask.Children.GetById(1);
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
}

public static void EvaluateIsNumeric()
{
    string[] numericFormulas =
        {
            "IsNumeric('AAA')", @"IsNUmeric(1)", "IsNumeric(1<0)", "IsNumeric(\"1.1\")", "IsNumeric(Choose((2 + Sgn(2^-3)), 123, \"one two three\"))"
        };

    var project = CreateTestProjectWithCustomField();

    foreach (var numericFormula in numericFormulas)
    {
        // 设置公式
        project.ExtendedAttributes[0].Formula = numericFormula;

        // 打印扩展属性值
        var task = project.RootTask.Children.GetById(1);
        Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    }
}

public static void EvaluateSwitch()
{
    var project = CreateTestProjectWithCustomField();

    // 设置公式
    project.ExtendedAttributes[0].Formula = "Switch( 0 < 1, \"0 is lesser than 1\", 0 > 1, \"0 is greater than 1\")";

    // 打印扩展属性值
    var task = project.RootTask.Children.GetById(1);
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
}

public static Project CreateTestProjectWithCustomField()
{
    var project = new Project();
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Custom Field");
    project.ExtendedAttributes.Add(definition);

    var task = project.RootTask.Children.Add("Task");

    var attribute = definition.CreateExtendedAttribute();
    task.ExtendedAttributes.Add(attribute);
    return project;
}
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


