---
title: "Prj.Revision"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. Het aantal keren dat een project is opgeslagen"
type: docs
weight: 610
url: /nl/net/aspose.tasks/prj/revision/
---
## Prj.Revision field

Het aantal keren dat een project is opgeslagen.

```csharp
public static readonly Key<int, PrjKey> Revision;
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


