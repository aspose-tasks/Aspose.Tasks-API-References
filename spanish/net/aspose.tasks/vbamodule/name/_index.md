---
title: "VbaModule.Name"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad VbaModule. Obtiene un nombre del módulo VBA"
type: docs
weight: 40
url: /es/net/aspose.tasks/vbamodule/name/
---
## VbaModule.Name property

Obtiene el nombre del módulo VBA

```csharp
public string Name { get; set; }
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

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


