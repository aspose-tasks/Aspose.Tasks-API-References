---
title: "Kelas BuiltInProjectPropertyCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Properties.BuiltInProjectPropertyCollection. Mewakili koleksi properti proyek bawaan"
type: docs
weight: 1530
url: /id/net/aspose.tasks.properties/builtinprojectpropertycollection/
---
## BuiltInProjectPropertyCollection class

Mewakili kumpulan properti proyek bawaan.

```csharp
public sealed class BuiltInProjectPropertyCollection : 
    PropertyKeyedCollection<BuiltInProjectProperty>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Author](../../aspose.tasks.properties/builtinprojectpropertycollection/author/) { get; set; } | Mendapatkan atau mengatur penulis proyek. |
| [Category](../../aspose.tasks.properties/builtinprojectpropertycollection/category/) { get; set; } | Mendapatkan atau mengatur kategori proyek. |
| [Comments](../../aspose.tasks.properties/builtinprojectpropertycollection/comments/) { get; set; } | Mendapatkan atau mengatur komentar proyek. |
| [Company](../../aspose.tasks.properties/builtinprojectpropertycollection/company/) { get; set; } | Mendapatkan atau mengatur perusahaan proyek. |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } |  |
| [HyperlinkBase](../../aspose.tasks.properties/builtinprojectpropertycollection/hyperlinkbase/) { get; set; } | Mendapatkan atau mengatur dasar hyperlink proyek. |
| override [IsReadOnly](../../aspose.tasks.properties/builtinprojectpropertycollection/isreadonly/) { get; } | Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca; jika tidak, false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } |  |
| [Keywords](../../aspose.tasks.properties/builtinprojectpropertycollection/keywords/) { get; set; } | Mendapatkan atau mengatur kata kunci proyek. |
| [Manager](../../aspose.tasks.properties/builtinprojectpropertycollection/manager/) { get; set; } | Mendapatkan atau mengatur manajer proyek. |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } |  |
| [Subject](../../aspose.tasks.properties/builtinprojectpropertycollection/subject/) { get; set; } | Mendapatkan atau mengatur subjek proyek. |
| [Title](../../aspose.tasks.properties/builtinprojectpropertycollection/title/) { get; set; } | Mendapatkan atau mengatur judul proyek. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(BuiltInProjectProperty) |  |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) |  |

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

* class [PropertyKeyedCollection&lt;T&gt;](../propertykeyedcollection-1/)
* class [BuiltInProjectProperty](../builtinprojectproperty/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


