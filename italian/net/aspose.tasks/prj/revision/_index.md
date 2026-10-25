---
title: "Prj.Revision"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Il numero di volte in cui un progetto è stato salvato"
type: docs
weight: 610
url: /it/net/aspose.tasks/prj/revision/
---
## Prj.Revision field

Il numero di volte in cui un progetto è stato salvato.

```csharp
public static readonly Key<int, PrjKey> Revision;
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


