---
title: "BuiltInProjectPropertyCollection.IsReadOnly"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "BuiltInProjectPropertyCollection özelliği. Bu koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer döndürür, aksi takdirde false"
type: docs
weight: 60
url: /tr/net/aspose.tasks.properties/builtinprojectpropertycollection/isreadonly/
---
## BuiltInProjectPropertyCollection.IsReadOnly property

Bu koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer alır; aksi takdirde false.

```csharp
public override bool IsReadOnly { get; }
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


