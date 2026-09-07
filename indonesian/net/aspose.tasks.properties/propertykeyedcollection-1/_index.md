---
title: "Kelas PropertyKeyedCollectionT"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Properties.PropertyKeyedCollection1T. Kelas dasar dari koleksi properti"
type: docs
weight: 1600
url: /id/net/aspose.tasks.properties/propertykeyedcollection-1/
---
## PropertyKeyedCollection&lt;T&gt; class

Kelas dasar dari kumpulan properti.

```csharp
public abstract class PropertyKeyedCollection<T> : PropertyCollection<T>, ICollection<T>
    where T : Property
```

| Parameter | Deskripsi |
| --- | --- |
| T | Tipe properti. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } | Mendapatkan jumlah properti dalam koleksi. |
| abstract [IsReadOnly](../../aspose.tasks.properties/propertykeyedcollection-1/isreadonly/) { get; } | Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca; jika tidak, false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } | Mendapatkan Properti yang terkait dengan kunci yang ditentukan. |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } | Mendapatkan koleksi semua nama properti. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(T) | Membuat properti khusus baru. |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) | Menentukan apakah [`PropertyCollection`](../propertycollection-1/) berisi properti dengan nama yang ditentukan. |

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

* class [PropertyCollection&lt;T&gt;](../propertycollection-1/)
* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


