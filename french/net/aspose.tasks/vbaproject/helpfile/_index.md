---
title: "VbaProject.HelpFile"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété VbaProject. Obtient le nom d'un fichier d'aide"
type: docs
weight: 40
url: /fr/net/aspose.tasks/vbaproject/helpfile/
---
## VbaProject.HelpFile property

Obtient le nom du fichier d'aide

```csharp
public string HelpFile { get; }
```

## Exemples

Montre comment lire les propriétés du projet VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("VbaProject.Name " + project.VbaProject.Name);
Console.WriteLine("VbaProject.Description " + project.VbaProject.Description);
Console.WriteLine("VbaProject.CompilationArguments" + project.VbaProject.CompilationArguments);
Console.WriteLine("VbaProject.HelpContextId" + project.VbaProject.HelpContextId);
Console.WriteLine("VbaProject.HelpFile" + project.VbaProject.HelpFile);
```

### Voir aussi

* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


