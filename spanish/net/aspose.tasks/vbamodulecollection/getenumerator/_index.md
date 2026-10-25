---
title: "VbaModuleCollection.GetEnumerator"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método VbaModuleCollection."
type: docs
weight: 80
url: /es/net/aspose.tasks/vbamodulecollection/getenumerator/
---
## VbaModuleCollection.GetEnumerator method

```csharp
public IEnumerator<VbaModule> GetEnumerator()
```

## Ejemplos

Muestra cómo iterar sobre los módulos VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var vbaProject = project.VbaProject;

Console.WriteLine("Total Modules Count: " + vbaProject.Modules.Count);
foreach (VbaModule module in vbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Module Type: " + module.Type);
    Console.WriteLine("Source Code: " + module.SourceCode);
    Console.WriteLine();
}
```

### Ver también

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


