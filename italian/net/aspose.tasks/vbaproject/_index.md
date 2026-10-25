---
title: "Classe VbaProject"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.VbaProject. Rappresenta VbaProject"
type: docs
weight: 2860
url: /it/net/aspose.tasks/vbaproject/
---
## VbaProject class

Rappresenta `VbaProject`.

```csharp
public class VbaProject
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CompilationArguments](../../aspose.tasks/vbaproject/compilationarguments/) { get; } | Ottiene gli argomenti di compilazione condizionale |
| [Description](../../aspose.tasks/vbaproject/description/) { get; } | Ottiene una descrizione del progetto. |
| [HelpContextId](../../aspose.tasks/vbaproject/helpcontextid/) { get; } | Ottiene l'ID del contesto di aiuto del progetto |
| [HelpFile](../../aspose.tasks/vbaproject/helpfile/) { get; } | Ottiene il nome del file di aiuto |
| [Modules](../../aspose.tasks/vbaproject/modules/) { get; } | Ottiene una raccolta di [`VbaModuleCollection`](../vbamodulecollection/) |
| [Name](../../aspose.tasks/vbaproject/name/) { get; } | Ottiene il nome del progetto |
| [References](../../aspose.tasks/vbaproject/references/) { get; } | Ottiene una raccolta di [`VbaReferenceCollection`](../vbareferencecollection/) |

## Esempi

Mostra come leggere le proprietà del progetto VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("VbaProject.Name " + project.VbaProject.Name);
Console.WriteLine("VbaProject.Description " + project.VbaProject.Description);
Console.WriteLine("VbaProject.CompilationArguments" + project.VbaProject.CompilationArguments);
Console.WriteLine("VbaProject.HelpContextId" + project.VbaProject.HelpContextId);
Console.WriteLine("VbaProject.HelpFile" + project.VbaProject.HelpFile);
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


