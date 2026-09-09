---
title: "Prj.Revision"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Bir projenin kaç kez kaydedildiği"
type: docs
weight: 610
url: /tr/net/aspose.tasks/prj/revision/
---
## Prj.Revision field

Bir projenin kaç kez kaydedildiği.

```csharp
public static readonly Key<int, PrjKey> Revision;
```

## Örnekler

Proje meta bilgilerini nasıl ayarlayacağınızı gösterir.

```csharp
var project = new Project(DataDir + "WriteProjectInfo.mpp");

// Proje bilgilerini ayarla
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

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


