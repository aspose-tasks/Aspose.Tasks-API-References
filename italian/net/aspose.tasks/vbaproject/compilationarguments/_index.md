---
title: "VbaProject.CompilationArguments"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "VbaProject property. Ottiene gli argomenti di compilazione condizionali"
type: docs
weight: 10
url: /it/net/aspose.tasks/vbaproject/compilationarguments/
---
## VbaProject.CompilationArguments property

Ottiene gli argomenti di compilazione condizionale

```csharp
public string CompilationArguments { get; }
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


