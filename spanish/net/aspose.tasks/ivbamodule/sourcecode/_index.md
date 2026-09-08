---
title: "IVbaModule.SourceCode"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad IVbaModule. Obtiene el código fuente del módulo VBA"
type: docs
weight: 30
url: /es/net/aspose.tasks/ivbamodule/sourcecode/
---
## IVbaModule.SourceCode property

Obtiene el código fuente del módulo VBA

```csharp
public string SourceCode { get; }
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


