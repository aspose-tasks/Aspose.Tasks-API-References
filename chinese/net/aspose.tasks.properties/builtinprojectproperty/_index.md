---
title: "类 BuiltInProjectProperty"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Properties.BuiltInProjectProperty 类。表示一个内置属性"
type: docs
weight: 1520
url: /zh/net/aspose.tasks.properties/builtinprojectproperty/
---
## BuiltInProjectProperty class

表示内置属性。

```csharp
public sealed class BuiltInProjectProperty : Property
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | 获取属性的名称。 |
| [Value](../../aspose.tasks.properties/builtinprojectproperty/value/) { get; set; } | 获取或设置属性的值。（2 个属性） |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | 以字符串形式返回属性值。 |

## 示例

展示如何读取项目内置属性。

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Author: " + project.BuiltInProps.Author);
Console.WriteLine("Category: " + project.BuiltInProps.Category);
Console.WriteLine("Comments: " + project.BuiltInProps.Comments);
Console.WriteLine("Company: " + project.BuiltInProps.Company);
Console.WriteLine("HyperlinkBase: " + project.BuiltInProps.HyperlinkBase);
Console.WriteLine("IsReadOnly: " + project.BuiltInProps.IsReadOnly);
Console.WriteLine("Keywords: " + project.BuiltInProps.Keywords);
Console.WriteLine("Manager: " + project.BuiltInProps.Manager);
Console.WriteLine("Subject: " + project.BuiltInProps.Subject);
Console.WriteLine("Title: " + project.BuiltInProps.Title);
Console.WriteLine();

// 遍历内置属性集合
foreach (Property property in project.BuiltInProps)
{
    Console.WriteLine("Name: " + property.Name);
    Console.WriteLine("Value: " + property.Value);
    Console.WriteLine("Prop As String: " + property.ToString());
    Console.WriteLine();
}
```

### 另见

* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


