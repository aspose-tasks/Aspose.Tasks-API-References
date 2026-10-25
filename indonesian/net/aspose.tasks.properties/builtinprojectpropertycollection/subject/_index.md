---
title: "BuiltInProjectPropertyCollection.Subject"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "BuiltInProjectPropertyCollection property. Mendapatkan atau mengatur subjek proyek"
type: docs
weight: 90
url: /id/net/aspose.tasks.properties/builtinprojectpropertycollection/subject/
---
## BuiltInProjectPropertyCollection.Subject property

Mendapatkan atau mengatur subjek proyek.

```csharp
public string Subject { get; set; }
```

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

* class [BuiltInProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../builtinprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


