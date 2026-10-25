---
title: "BuiltInProjectPropertyCollection.Title"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "BuiltInProjectPropertyCollection özelliği. Bir projenin başlığını alır veya ayarlar"
type: docs
weight: 100
url: /tr/net/aspose.tasks.properties/builtinprojectpropertycollection/title/
---
## BuiltInProjectPropertyCollection.Title property

Bir projenin başlığını alır veya ayarlar.

```csharp
public string Title { get; set; }
```

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

* class [BuiltInProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../builtinprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


