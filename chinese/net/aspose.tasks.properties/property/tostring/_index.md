---
title: "Property.ToString"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Property 方法。返回属性值的字符串形式"
type: docs
weight: 30
url: /zh/net/aspose.tasks.properties/property/tostring/
---
## Property.ToString method

以字符串形式返回属性值。

```csharp
public override string ToString()
```

### 返回值

字符串值。

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

* class [Property](../)
* namespace [Aspose.Tasks.Properties](../../property/)
* assembly [Aspose.Tasks](../../../)


