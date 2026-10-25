---
title: "Property.Value"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Property özelliği. Özelliğin bir değerini alır veya ayarlar."
type: docs
weight: 20
url: /tr/net/aspose.tasks.properties/property/value/
---
## Property.Value property

Özelliğin değerini alır veya ayarlar.

```csharp
public object Value { get; set; }
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

* class [Property](../)
* namespace [Aspose.Tasks.Properties](../../property/)
* assembly [Aspose.Tasks](../../../)


