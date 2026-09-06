---
title: "ExtendedAttribute.TextValue"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ExtendedAttribute 属性。获取或设置 Text 类型属性的值。"
type: docs
weight: 80
url: /zh/net/aspose.tasks/extendedattribute/textvalue/
---
## ExtendedAttribute.TextValue property

获取或设置 'Text' 类型属性的值。

```csharp
public string TextValue { get; set; }
```

### 异常

| 异常 | 条件 |
| --- | --- |
| InvalidOperationException | 如果 [`AttributeDefinition`](../attributedefinition/) 属性未初始化，或当前属性不是文本属性，则抛出异常。 |

## 示例

展示如何添加使用 MS Project 日期/时间公式的扩展属性。

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");

var numberDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, null);
project.ExtendedAttributes.Add(numberDefinition);

var numberAttribute = numberDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(numberAttribute);

// 设置 ProjDateDiff 公式并打印扩展属性值。
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/18/2015\")";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/25/2015\")";
Console.WriteLine(numberAttribute.NumericValue);

var dateDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, null);
project.ExtendedAttributes.Add(dateDefinition);
var dateAttribute = dateDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(dateAttribute);

var durationDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration4, "Custom duration field");
project.ExtendedAttributes.Add(durationDefinition);
var durationAttribute = durationDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(durationAttribute);

var textDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text5, "Custom text field");
project.ExtendedAttributes.Add(textDefinition);
var textAttribute = textDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(textAttribute);

// 设置 ProjDateSub 公式并打印扩展属性值。
dateDefinition.Formula = "ProjDateSub(\"3/19/2015\", \"1d\")";
Console.WriteLine(dateAttribute.DateValue);

// 我们可以将 ProjDurConv 公式设置为持续时间值属性以及文本值属性。
// 将 ProjDurConv 公式设置为持续时间值的扩展属性并打印其值。
durationDefinition.Formula = "ProjDurConv([Duration], pjHours)";
Console.WriteLine(durationAttribute.DurationValue);

// 将 ProjDurConv 公式设置为文本值的扩展属性并打印其值。
textDefinition.Formula = "ProjDurConv([Duration], pjWeeks)";
Console.WriteLine(textAttribute.TextValue);

// 设置 Second 公式并打印扩展属性值。
numberDefinition.Formula = "Second(\"4/21/2015 2:53:41 AM\")";
Console.WriteLine(numberAttribute.NumericValue);

// 设置 Weekday 公式并打印扩展属性值。
numberDefinition.Formula = "Weekday(\"24/3/2015\", 1)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 2)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 3)";
Console.WriteLine(numberAttribute.NumericValue);
```

### 另见

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


