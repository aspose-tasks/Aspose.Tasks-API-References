---
title: "Prj.LastSaved"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. La data in cui un progetto è stato salvato l'ultima volta. Salvato in formato UTC nei file mpp. Tipo DateTime."
type: docs
weight: 440
url: /it/net/aspose.tasks/prj/lastsaved/
---
## Prj.LastSaved field

La data in cui un progetto è stato salvato l'ultima volta. Salvata in formato UTC nei file mpp. Tipo DateTime.

```csharp
public static readonly Key<DateTime, PrjKey> LastSaved;
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


