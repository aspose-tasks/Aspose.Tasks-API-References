---
title: "Struktur GenericPropertyTKey"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Struktur Aspose.Tasks.Properties.GenericProperty1TKey. Mewakili properti kontainer"
type: docs
weight: 1570
url: /id/net/aspose.tasks.properties/genericproperty-1/
---
## GenericProperty&lt;TKey&gt; structure

Mewakili properti kontainer.

```csharp
public struct GenericProperty<TKey>
    where TKey : struct
```

| Parameter | Deskripsi |
| --- | --- |
| TKey | Tipe nilai properti. |

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [GenericProperty](genericproperty/)(string) | Menginisialisasi instance baru dari struktur `GenericProperty`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Name](../../aspose.tasks.properties/genericproperty-1/name/) { get; } | Mendapatkan nama properti. |
| [Value](../../aspose.tasks.properties/genericproperty-1/value/) { get; } | Mendapatkan nilai properti. |

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

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


