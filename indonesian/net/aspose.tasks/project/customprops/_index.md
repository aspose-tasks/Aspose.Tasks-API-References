---
title: "Project.CustomProps"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Project. Mendapatkan koleksi properti khusus proyek"
type: docs
weight: 260
url: /id/net/aspose.tasks/project/customprops/
---
## Project.CustomProps property

Menampilkan koleksi properti khusus proyek.

```csharp
public CustomProjectPropertyCollection CustomProps { get; }
```

## Contoh

Menampilkan cara membaca properti meta proyek (API usang).

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

// properti khusus tersedia melalui koleksi bertipe
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}

// Properti bawaan tersedia secara langsung
Console.WriteLine(project.BuiltInProps.Author);
Console.WriteLine(project.BuiltInProps.Title);

// atau sebagai item dari koleksi properti bawaan
foreach (var property in project.BuiltInProps)
{
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}
```

### Lihat Juga

* class [CustomProjectPropertyCollection](../../../aspose.tasks.properties/customprojectpropertycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


