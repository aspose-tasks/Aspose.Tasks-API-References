---
title: "Kelas BuiltInProjectProperty"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Properties.BuiltInProjectProperty. Mewakili properti bawaan"
type: docs
weight: 1520
url: /id/net/aspose.tasks.properties/builtinprojectproperty/
---
## BuiltInProjectProperty class

Mewakili properti bawaan.

```csharp
public sealed class BuiltInProjectProperty : Property
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | Mendapatkan nama properti. |
| [Value](../../aspose.tasks.properties/builtinprojectproperty/value/) { get; set; } | Mendapatkan atau mengatur nilai properti. (2 properti) |

## Metode

| Nama | Deskripsi |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | Mengembalikan nilai properti sebagai string. |

## Contoh

Menampilkan cara membaca properti bawaan proyek.

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

// iterasi atas koleksi properti bawaan
foreach (Property property in project.BuiltInProps)
{
    Console.WriteLine("Name: " + property.Name);
    Console.WriteLine("Value: " + property.Value);
    Console.WriteLine("Prop As String: " + property.ToString());
    Console.WriteLine();
}
```

### Lihat Juga

* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


