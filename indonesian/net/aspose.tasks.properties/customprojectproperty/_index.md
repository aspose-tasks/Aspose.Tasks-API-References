---
title: "Kelas CustomProjectProperty"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Properties.CustomProjectProperty. Mewakili properti khusus"
type: docs
weight: 1540
url: /id/net/aspose.tasks.properties/customprojectproperty/
---
## CustomProjectProperty class

Mewakili properti khusus.

```csharp
public sealed class CustomProjectProperty : Property
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | Mendapatkan nama properti. |
| [Type](../../aspose.tasks.properties/customprojectproperty/type/) { get; } | Mendapatkan tipe properti. |
| [Value](../../aspose.tasks.properties/property/value/) { get; set; } | Mendapatkan atau mengatur nilai properti. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | Mengembalikan nilai properti sebagai string. |

## Contoh

Menampilkan cara bekerja dengan koleksi properti proyek khusus.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// mari tambahkan properti khusus baru
// koleksi mendukung tipe Boolean, DateTime, Double, String
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// properti khusus tersedia melalui koleksi bertipe
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// dapatkan nilai properti khusus
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// iterasi atas nama-nama properti khusus
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// seseorang dapat menghapus nilai dengan kunci string
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// atau seseorang dapat menghapus koleksi sepenuhnya
project.CustomProps.Clear();
```

### Lihat Juga

* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


