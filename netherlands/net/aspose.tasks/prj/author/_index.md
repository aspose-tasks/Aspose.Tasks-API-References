---
title: "Prj.Author"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. De auteur van een project."
type: docs
weight: 40
url: /nl/net/aspose.tasks/prj/author/
---
## Prj.Author field

De auteur van een project.

```csharp
public static readonly Key<string, PrjKey> Author;
```

## Voorbeelden

Toont hoe projectmeta-informatie in te stellen.

```csharp
var project = new Project(DataDir + "WriteProjectInfo.mpp");

// Stel projectinformatie in
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

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


