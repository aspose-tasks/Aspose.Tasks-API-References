---
title: "类 GlobalizationSettings"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.GlobalizationSettings 类。表示项目的全球化设置"
type: docs
weight: 720
url: /zh/net/aspose.tasks/globalizationsettings/
---
## GlobalizationSettings class

表示项目的全球化设置。

```csharp
public class GlobalizationSettings
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| virtual [FalseLiteral](../../aspose.tasks/globalizationsettings/falseliteral/) { get; } | 获取在公式中使用的布尔值“false”文字的字符串。 |
| virtual [FormulaDateNA](../../aspose.tasks/globalizationsettings/formuladatena/) { get; } | 获取在日期字段的公式中使用的 "NA"（空值）文字。 |
| virtual [TrueLiteral](../../aspose.tasks/globalizationsettings/trueliteral/) { get; } | 获取在公式中使用的布尔值 'true' 字面量的字符串。 |

## 备注

推荐的做法是在整个项目中使用与区域设置无关的字面量或格式。但是，如果项目使用特定区域设置的字面量，则可以使用此类来帮助公式计算引擎解析这些字面量。

## 示例

展示如何设置项目的语言特定设置。

```csharp
var project = new Project();

var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number");
attribute.Formula = "IIf(ProjDateValue('n.a.')=[Date1];100;200)";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// 创建扩展属性
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

var attributeDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "Date");

task.ExtendedAttributes.Add(attributeDate.CreateExtendedAttribute(DateTime.MinValue));

Console.WriteLine(extendedAttribute.NumericValue);

project.GlobalizationSettings = new MyGlobalizationSettings();

Console.WriteLine(extendedAttribute.NumericValue);
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


