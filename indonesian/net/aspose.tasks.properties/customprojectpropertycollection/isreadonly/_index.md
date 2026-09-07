---
title: "CustomProjectPropertyCollection.IsReadOnly"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti CustomProjectPropertyCollection. Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca; jika tidak, false"
type: docs
weight: 20
url: /id/net/aspose.tasks.properties/customprojectpropertycollection/isreadonly/
---
## CustomProjectPropertyCollection.IsReadOnly property

Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca; jika tidak, false.

```csharp
public override bool IsReadOnly { get; }
```

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

* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


