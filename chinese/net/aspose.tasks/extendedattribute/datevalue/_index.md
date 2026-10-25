---
title: "ExtendedAttribute.DateValue"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ExtendedAttribute 属性。获取或设置日期类型（Date、Start、Finish）属性的值。"
type: docs
weight: 20
url: /zh/net/aspose.tasks/extendedattribute/datevalue/
---
## ExtendedAttribute.DateValue property

获取或设置日期类型属性的值（Date、Start、Finish）。

```csharp
public DateTime DateValue { get; set; }
```

### 异常

| 异常 | 条件 |
| --- | --- |
| InvalidOperationException | 如果 [`AttributeDefinition`](../attributedefinition/) 属性未初始化或当前属性不是日期属性，则抛出异常。 |

## 示例

展示如何更改扩展属性的属性定义。

```csharp
var project = new Project();

// 创建新的任务扩展属性定义
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, string.Empty);

// 向属性添加公式。
definition.Alias = "Difference between Cost and Actual Cost";
definition.Formula = "[Cost]-[Actual Cost]";

project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
task.Set(Tsk.Deadline, new DateTime(2020, 4, 22, 17, 0, 0));
task.Set(Tsk.Cost, 20);
task.Set(Tsk.ActualCost, 13);

// 创建扩展属性
var extendedAttribute = definition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

Console.WriteLine("Before change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.NumericValue);

// 创建一个新的日期扩展属性定义。
var newDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Date, ExtendedAttributeTask.Date1, string.Empty);

// 向属性添加公式。
newDefinition.Alias = "Days from finish to deadline";
newDefinition.Formula = "[Deadline] - [Finish]";
project.ExtendedAttributes.Add(newDefinition);

extendedAttribute = newDefinition.CreateExtendedAttribute();

Console.WriteLine();
Console.WriteLine("After change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.DateValue.Day);
```

### 另见

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


