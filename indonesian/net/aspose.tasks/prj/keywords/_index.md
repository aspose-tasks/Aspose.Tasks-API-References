---
title: "Prj.Keywords"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Prj field. Kata kunci proyek"
type: docs
weight: 410
url: /id/net/aspose.tasks/prj/keywords/
---
## Prj.Keywords field

Kata kunci proyek.

```csharp
public static readonly Key<string, PrjKey> Keywords;
```

## Contoh

Menampilkan cara mengatur informasi meta proyek.

```csharp
var project = new Project(DataDir + "WriteProjectInfo.mpp");

// Atur informasi proyek
project.Set(Prj.Author, "Author");
project.Set(Prj.LastAuthor, "Last Author");
project.Set(Prj.Revision, 15);
project.Set(Prj.Keywords, "MSP Aspose");
project.Set(Prj.Comments, "Comments");

Console.WriteLine(project.Get(Prj.Author));
Console.WriteLine(project.Get(Prj.LastAuthor));
Console.WriteLine(project.Get(Prj.Revision));
Console.WriteLine(project.Get(Prj.Keywords));
Console.WriteLine(project.Get(Prj.Comments));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


