---
title: "VbaProject.HelpFile"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà VbaProject. Ottiene il nome del file di aiuto"
type: docs
weight: 40
url: /it/net/aspose.tasks/vbaproject/helpfile/
---
## VbaProject.HelpFile property

Ottiene il nome del file di aiuto

```csharp
public string HelpFile { get; }
```

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

* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


