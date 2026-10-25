---
title: "Interfaz IVbaModule"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Interfaz Aspose.Tasks.IVbaModule. Representa un módulo con código VBA"
type: docs
weight: 880
url: /es/net/aspose.tasks/ivbamodule/
---
## IVbaModule interface

Representa un módulo con código VBA.

```csharp
public interface IVbaModule
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Attributes](../../aspose.tasks/ivbamodule/attributes/) { get; } | Obtiene una colección de [`VbaModuleAttributeCollection`](../vbamoduleattributecollection/) |
| [Name](../../aspose.tasks/ivbamodule/name/) { get; } | Obtiene el nombre del módulo VBA |
| [SourceCode](../../aspose.tasks/ivbamodule/sourcecode/) { get; } | Obtiene el código fuente del módulo VBA |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


