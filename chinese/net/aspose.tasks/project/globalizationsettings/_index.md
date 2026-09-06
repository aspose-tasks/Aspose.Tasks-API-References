---
title: "Project.GlobalizationSettings"
second_title: "Aspose.Tasks for .NET API 参考"
description: "项目属性。获取或设置项目的全局化语言特定设置"
type: docs
weight: 460
url: /zh/net/aspose.tasks/project/globalizationsettings/
---
## Project.GlobalizationSettings property

获取或设置项目的全球化（特定语言）设置。

```csharp
public GlobalizationSettings GlobalizationSettings { get; set; }
```

## 备注

推荐的做法是整个项目使用与区域性无关的文字或格式。但是，如果项目使用特定区域性的文字，可以使用此类来帮助计算引擎解析这些文字。

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

* class [GlobalizationSettings](../../globalizationsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


