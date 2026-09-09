---
title: "Sınıf BuiltInProjectProperty"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Properties.BuiltInProjectProperty sınıfı. Yerleşik bir özelliği temsil eder."
type: docs
weight: 1520
url: /tr/net/aspose.tasks.properties/builtinprojectproperty/
---
## BuiltInProjectProperty class

Yerleşik bir özelliği temsil eder.

```csharp
public sealed class BuiltInProjectProperty : Property
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | Özelliğin adını alır. |
| [Value](../../aspose.tasks.properties/builtinprojectproperty/value/) { get; set; } | Özelliğin değerini alır veya ayarlar. (2 özellik) |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | Özellik değerini dize olarak döndürür. |

## Örnekler

Proje yerleşik özelliklerini nasıl okuyacağınızı gösterir.

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

// yerleşik özellik koleksiyonunda yineleme yap
foreach (Property property in project.BuiltInProps)
{
    Console.WriteLine("Name: " + property.Name);
    Console.WriteLine("Value: " + property.Value);
    Console.WriteLine("Prop As String: " + property.ToString());
    Console.WriteLine();
}
```

### Ayrıca Bakınız

* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


