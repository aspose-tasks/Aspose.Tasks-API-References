---
title: "Project.CustomProps"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. Projenin özel özellikler koleksiyonunu alır"
type: docs
weight: 260
url: /tr/net/aspose.tasks/project/customprops/
---
## Project.CustomProps property

Projenin özel özellikler koleksiyonunu alır.

```csharp
public CustomProjectPropertyCollection CustomProps { get; }
```

## Örnekler

Proje meta özelliklerini nasıl okuyacağını gösterir (eski API).

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

// Özel özellikler tiplenmiş koleksiyon aracılığıyla kullanılabilir.
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}

// Yerleşik özellikler doğrudan kullanılabilir
Console.WriteLine(project.BuiltInProps.Author);
Console.WriteLine(project.BuiltInProps.Title);

// veya yerleşik özellik koleksiyonunun bir öğesi olarak
foreach (var property in project.BuiltInProps)
{
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}
```

### Ayrıca Bakınız

* class [CustomProjectPropertyCollection](../../../aspose.tasks.properties/customprojectpropertycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


