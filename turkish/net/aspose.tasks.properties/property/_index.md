---
title: "Sınıf Property"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Properties.Property sınıfı. Bir özelliğin temel sınıfını temsil eder"
type: docs
weight: 1580
url: /tr/net/aspose.tasks.properties/property/
---
## Property class

Bir özelliğin temel sınıfını temsil eder.

```csharp
public abstract class Property
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | Özelliğin adını alır. |
| [Value](../../aspose.tasks.properties/property/value/) { get; set; } | Özelliğin değerini alır veya ayarlar. |

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

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


