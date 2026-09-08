---
title: "Clase VbaModule"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.VbaModule. Representa un módulo VBA"
type: docs
weight: 2810
url: /es/net/aspose.tasks/vbamodule/
---
## VbaModule class

Representa un módulo VBA.

```csharp
public sealed class VbaModule
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Attributes](../../aspose.tasks/vbamodule/attributes/) { get; } | Obtiene una colección de los atributos del módulo. |
| [Name](../../aspose.tasks/vbamodule/name/) { get; set; } | Obtiene el nombre del módulo VBA |
| [SourceCode](../../aspose.tasks/vbamodule/sourcecode/) { get; set; } | Obtiene o establece el código fuente del módulo VBA |
| [Type](../../aspose.tasks/vbamodule/type/) { get; } | Obtiene el tipo del módulo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [CreateClassModule](../../aspose.tasks/vbamodule/createclassmodule/)(string) | Crea una instancia de `VbaModule` con el tipo VbaModuleType.ClassModule. |
| static [CreateProceduralModule](../../aspose.tasks/vbamodule/createproceduralmodule/)(string) | Crea una instancia de `VbaModule` con el tipo VbaModuleType.ProceduralModule. |

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


