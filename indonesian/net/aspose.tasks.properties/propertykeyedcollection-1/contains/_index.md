---
title: "PropertyKeyedCollection1.Contains"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode PropertyKeyedCollection. Menentukan apakah PropertyCollection berisi properti dengan nama yang ditentukan"
type: docs
weight: 60
url: /id/net/aspose.tasks.properties/propertykeyedcollection-1/contains/
---
## PropertyKeyedCollection&lt;T&gt;.Contains method

Menentukan apakah [`PropertyCollection`](../../propertycollection-1/) berisi properti dengan nama yang ditentukan.

```csharp
public bool Contains(string name)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | String | Nama sebuah properti |

### Nilai Kembali

true jika [`PropertyCollection`](../../propertycollection-1/) berisi properti dengan nama yang ditentukan; jika tidak, false.

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

* class [PropertyKeyedCollection&lt;T&gt;](../)
* namespace [Aspose.Tasks.Properties](../../propertykeyedcollection-1/)
* assembly [Aspose.Tasks](../../../)


