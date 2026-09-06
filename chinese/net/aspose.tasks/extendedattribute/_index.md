---
title: "类 ExtendedAttribute"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ExtendedAttribute 类。表示扩展属性"
type: docs
weight: 520
url: /zh/net/aspose.tasks/extendedattribute/
---
## ExtendedAttribute class

表示扩展属性。

```csharp
public class ExtendedAttribute
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [AttributeDefinition](../../aspose.tasks/extendedattribute/attributedefinition/) { get; } | 获取属性定义。 |
| [DateValue](../../aspose.tasks/extendedattribute/datevalue/) { get; set; } | 获取或设置日期类型属性的值（Date、Start、Finish）。 |
| [DurationValue](../../aspose.tasks/extendedattribute/durationvalue/) { get; set; } | 获取或设置 'Duration' 类型属性的值。 |
| [FieldId](../../aspose.tasks/extendedattribute/fieldid/) { get; } | 获取字段的 ID。 |
| [FlagValue](../../aspose.tasks/extendedattribute/flagvalue/) { get; set; } | 获取或设置一个值，以指示是否为 'Flag' 类型的属性设置了标志。 |
| [IsErrorValue](../../aspose.tasks/extendedattribute/iserrorvalue/) { get; } | 获取扩展属性值的计算是否出现错误。 |
| [NumericValue](../../aspose.tasks/extendedattribute/numericvalue/) { get; set; } | 获取或设置数值类型属性的值（Cost、Number）。 |
| [TextValue](../../aspose.tasks/extendedattribute/textvalue/) { get; set; } | 获取或设置 'Text' 类型属性的值。 |
| [ValueGuid](../../aspose.tasks/extendedattribute/valueguid/) { get; } | 获取查找值的 GUID。 |
| [ValueReadOnly](../../aspose.tasks/extendedattribute/valuereadonly/) { get; } | 获取一个值，以指示此 `ExtendedAttribute` 实例的值是否为只读。如果在此对象的 [`ExtendedAttributeDefinition`](../extendedattributedefinition/) 中定义了公式或汇总，则返回 true。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [ToString](../../aspose.tasks/extendedattribute/tostring/)() | 返回扩展属性的简短字符串表示。 |

## 备注

当前支持从 MSP Xml 2003/2007 和 mpp 2003 读取的所有类型的扩展属性。对于 MSP mpp 2007，支持读取所有扩展属性，除持续时间和标志外。

## 示例

展示如何添加自定义字段，其值使用用户指定的公式计算。

```csharp
var project = new Project();

// 创建新的任务扩展属性定义
var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, "Cost ratio");

// 向属性添加公式。
attribute.Formula = "[Cost] / [Actual Cost]";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// 创建扩展属性
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

// 我们为扩展属性设置了 Formula，因此它是只读的（该值使用公式计算）。
// 输出是 "Value is read only"
Console.WriteLine(extendedAttribute.ValueReadOnly ? "Value is read only" : "Value is not read only");

// 您可以尝试设置只读字段的值，但它不会生效。
extendedAttribute.NumericValue = -1000000M;

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost),
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());

task.Set(Tsk.Cost, 100m);
task.Set(Tsk.ActualCost, 120m);

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost), 
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


