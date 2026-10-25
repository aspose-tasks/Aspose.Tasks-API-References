---
title: "Clase VbaModuleAttribute"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.VbaModuleAttribute. El atributo del objeto VbaModule"
type: docs
weight: 2820
url: /es/net/aspose.tasks/vbamoduleattribute/
---
## VbaModuleAttribute class

El atributo del objeto [`VbaModule`](../vbamodule/)

```csharp
public sealed class VbaModuleAttribute : IEquatable<VbaModuleAttribute>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Key](../../aspose.tasks/vbamoduleattribute/key/) { get; } | Obtiene la clave del atributo del módulo VBA. |
| [Value](../../aspose.tasks/vbamoduleattribute/value/) { get; } | Obtiene el valor del atributo del módulo VBA. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals_1)(object) | Devuelve un valor que indica si esta instancia es igual al objeto `VbaModuleAttribute` especificado. |
| [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals)(VbaModuleAttribute) | Devuelve un valor que indica si esta instancia es igual al objeto `VbaModuleAttribute` especificado. |
| override [GetHashCode](../../aspose.tasks/vbamoduleattribute/gethashcode/)() | Devuelve un valor de código hash para este `VbaModuleAttribute`. |

## Ejemplos

Muestra cómo trabajar con atributos de módulo VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("  VB Name: " + attribute.Key);
        Console.WriteLine("  Module: " + attribute.Value);
    }
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


