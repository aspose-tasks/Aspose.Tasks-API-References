---
title: "IVbaModule.Name"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad IVbaModule. Obtiene el nombre del módulo VBA"
type: docs
weight: 20
url: /es/net/aspose.tasks/ivbamodule/name/
---
## IVbaModule.Name property

Obtiene el nombre del módulo VBA

```csharp
public string Name { get; }
```

## Ejemplos

Muestra cómo leer los módulos del proyecto VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

### Ver también

* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


