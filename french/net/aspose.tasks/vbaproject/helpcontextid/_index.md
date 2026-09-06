---
title: "VbaProject.HelpContextId"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "VbaProject propriété. Obtient un identifiant d'aide contextuelle du projet"
type: docs
weight: 30
url: /fr/net/aspose.tasks/vbaproject/helpcontextid/
---
## VbaProject.HelpContextId property

Obtient l'identifiant de contexte d'aide du projet

```csharp
public int HelpContextId { get; }
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


