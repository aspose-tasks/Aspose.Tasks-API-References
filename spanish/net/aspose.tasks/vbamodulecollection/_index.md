---
title: "Clase VbaModuleCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.VbaModuleCollection. Representa una colección de objetos VbaModule"
type: docs
weight: 2840
url: /es/net/aspose.tasks/vbamodulecollection/
---
## VbaModuleCollection class

Representa una colección de [`VbaModule`](../vbamodule/) objetos.

```csharp
public class VbaModuleCollection : ICollection<VbaModule>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/vbamodulecollection/count/) { get; } |  |
| [IsReadOnly](../../aspose.tasks/vbamodulecollection/isreadonly/) { get; } |  |
| [Item](../../aspose.tasks/vbamodulecollection/item/) { get; } | Obtiene el módulo en el índice especificado. (2 indexadores) |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/vbamodulecollection/add/)(VbaModule) |  |
| [Clear](../../aspose.tasks/vbamodulecollection/clear/)() |  |
| [Contains](../../aspose.tasks/vbamodulecollection/contains/)(VbaModule) |  |
| [CopyTo](../../aspose.tasks/vbamodulecollection/copyto/)(VbaModule[], int) |  |
| [GetEnumerator](../../aspose.tasks/vbamodulecollection/getenumerator/)() |  |
| [Remove](../../aspose.tasks/vbamodulecollection/remove/)(VbaModule) |  |
| [ToList](../../aspose.tasks/vbamodulecollection/tolist/)() | Convierte el objeto de colección en una lista de [`VbaModule`](../vbamodule/) objetos. |

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

* class [VbaModule](../vbamodule/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


