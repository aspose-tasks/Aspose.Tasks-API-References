---
title: "Clase VbaReference"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.VbaReference. Representa una referencia del VbaProject"
type: docs
weight: 2870
url: /es/net/aspose.tasks/vbareference/
---
## VbaReference class

Representa una referencia del [`VbaProject`](../vbaproject/).

```csharp
public sealed class VbaReference : IEquatable<VbaReference>
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [VbaReference](vbareference/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [LibIdentifier](../../aspose.tasks/vbareference/libidentifier/) { get; } | Obtiene el identificador de la biblioteca. |
| [Name](../../aspose.tasks/vbareference/name/) { get; set; } | Obtiene o establece el nombre de la referencia VBA. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.tasks/vbareference/equals/#equals_1)(object) | Devuelve un valor que indica si esta instancia es igual al objeto `VbaReference` especificado. |
| [Equals](../../aspose.tasks/vbareference/equals/#equals)(VbaReference) | Devuelve un valor que indica si esta instancia es igual al objeto `VbaReference` especificado. |
| override [GetHashCode](../../aspose.tasks/vbareference/gethashcode/)() | Devuelve un valor de código hash para este `VbaReference`. |

## Ejemplos

Muestra cómo leer referencias VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


