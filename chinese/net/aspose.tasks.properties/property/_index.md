---
title: "类 Property"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Properties.Property 类。表示属性的基类"
type: docs
weight: 1580
url: /zh/net/aspose.tasks.properties/property/
---
## Property class

表示属性的基类。

```csharp
public abstract class Property
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | 获取属性的名称。 |
| [Value](../../aspose.tasks.properties/property/value/) { get; set; } | 获取或设置属性的值。 |

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

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


