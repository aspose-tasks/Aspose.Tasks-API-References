---
title: "ExtendedAttribute.IsErrorValue"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ExtendedAttribute 属性。获取扩展属性值的计算是否导致错误。"
type: docs
weight: 60
url: /zh/net/aspose.tasks/extendedattribute/iserrorvalue/
---
## ExtendedAttribute.IsErrorValue property

获取扩展属性值的计算是否出现错误。

```csharp
public bool IsErrorValue { get; }
```

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

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


