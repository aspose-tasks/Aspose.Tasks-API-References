---
title: "Project.BuiltInProps"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. Projenin yerleşik özellikler koleksiyonunu alır"
type: docs
weight: 100
url: /tr/net/aspose.tasks/project/builtinprops/
---
## Project.BuiltInProps property

Projenin yerleşik özellikler koleksiyonunu alır.

```csharp
public BuiltInProjectPropertyCollection BuiltInProps { get; }
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

* class [BuiltInProjectPropertyCollection](../../../aspose.tasks.properties/builtinprojectpropertycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


