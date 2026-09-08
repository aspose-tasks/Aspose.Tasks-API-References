---
title: "VbaModuleCollection.ToList"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método VbaModuleCollection. Convierte el objeto de colección en una lista de objetos VbaModule"
type: docs
weight: 100
url: /es/net/aspose.tasks/vbamodulecollection/tolist/
---
## VbaModuleCollection.ToList method

Convierte el objeto de colección en una lista de objetos [`VbaModule`](../../vbamodule/).

```csharp
public List<VbaModule> ToList()
```

### Valor devuelto

Lista de objetos.

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


