---
title: "Prj.SaveVersion"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. La versione di Microsoft Office Project da cui è stato salvato un file di progetto"
type: docs
weight: 620
url: /it/net/aspose.tasks/prj/saveversion/
---
## Prj.SaveVersion field

La versione di Microsoft Office Project da cui è stato salvato un file di progetto.

```csharp
public static readonly Key<int, PrjKey> SaveVersion;
```

## Esempi

Mostra come verificare la versione di salvataggio del progetto e la data di salvataggio.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// Visualizza versione del progetto
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


