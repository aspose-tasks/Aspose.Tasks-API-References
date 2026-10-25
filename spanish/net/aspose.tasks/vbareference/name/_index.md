---
title: "VbaReference.Name"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad VbaReference. Obtiene o establece el nombre de la referencia VBA"
type: docs
weight: 30
url: /es/net/aspose.tasks/vbareference/name/
---
## VbaReference.Name property

Obtiene o establece el nombre de la referencia VBA.

```csharp
public string Name { get; set; }
```

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

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


