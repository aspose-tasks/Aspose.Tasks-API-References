---
title: "Prj.Keywords"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Parole chiave del progetto"
type: docs
weight: 410
url: /it/net/aspose.tasks/prj/keywords/
---
## Prj.Keywords field

Parole chiave del progetto.

```csharp
public static readonly Key<string, PrjKey> Keywords;
```

## Esempi

Mostra come impostare le meta‑informazioni del progetto.

```csharp
var project = new Project(DataDir + "WriteProjectInfo.mpp");

// Imposta le informazioni del progetto
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

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


