---
title: "OutlineCodeDefinitionCollection.Item"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti OutlineCodeDefinitionCollection. Mengembalikan atau mengatur elemen pada indeks yang ditentukan"
type: docs
weight: 30
url: /id/net/aspose.tasks/outlinecodedefinitioncollection/item/
---
## OutlineCodeDefinitionCollection indexer

Mengembalikan atau mengatur elemen pada indeks yang ditentukan.

```csharp
public OutlineCodeDefinition this[int index] { get; set; }
```

| Parameter | Deskripsi |
| --- | --- |
| index | Indeks berbasis nol dari elemen yang akan diambil atau diatur. |

### Nilai Kembali

elemen pada indeks yang ditentukan.

## Contoh

Menampilkan cara bekerja dengan koleksi definisi kode outline.

```csharp
var project = new Project(DataDir + "OutlineCodes.mpp");

Console.WriteLine("Count of outline code definitions: " + project.OutlineCodes.Count);
foreach (var outlineCode in project.OutlineCodes)
{
    Console.WriteLine("Field Name: " + outlineCode.FieldName);
    Console.WriteLine("Alias: " + outlineCode.Alias);
    Console.WriteLine();
}

// tambahkan definisi kode outline khusus
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };

var outlineCodeDefinition2 = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString("D"), Alias = "My Outline Code 2" };

if (!project.OutlineCodes.IsReadOnly)
{
    project.OutlineCodes.Add(outlineCodeDefinition);

    // menyisipkan definisi kode outline pada posisi
    project.OutlineCodes.Insert(0, outlineCodeDefinition2);
}

// temukan indeks definisi kode outline
var index = project.OutlineCodes.IndexOf(outlineCodeDefinition);

// sunting definisi kode outline
project.OutlineCodes[index].Alias = "New Alias";

// ...
// bekerja dengan definisi kode outline
// ...

// hapus definisi kode outline
if (project.OutlineCodes.Contains(outlineCodeDefinition))
{
    project.OutlineCodes.Remove(outlineCodeDefinition);
}

// hapus definisi kode outline berdasarkan indeks
project.OutlineCodes.RemoveAt(0);

var otherProject = new Project(DataDir + "Blank2010.mpp");

// hapus definisi kode outline
otherProject.OutlineCodes.Clear();

// salin definisi kode outline
var outlineCodeDefinitions = new OutlineCodeDefinition[project.OutlineCodes.Count];
project.OutlineCodes.CopyTo(outlineCodeDefinitions, 0);

foreach (var definition in outlineCodeDefinitions)
{
    otherProject.OutlineCodes.Add(definition);
}

// ...
// bekerja dengan definisi kode outline
// ...

// hapus definisi kode outline satu per satu
List<OutlineCodeDefinition> definitions = otherProject.OutlineCodes.ToList();
foreach (var definition in definitions)
{
    otherProject.OutlineCodes.Remove(definition);
}
```

### Lihat Juga

* class [OutlineCodeDefinition](../../outlinecodedefinition/)
* class [OutlineCodeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../outlinecodedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


