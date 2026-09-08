---
title: "VbaReference.LibIdentifier"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad VbaReference. Obtiene el identificador de la biblioteca"
type: docs
weight: 20
url: /es/net/aspose.tasks/vbareference/libidentifier/
---
## VbaReference.LibIdentifier property

Obtiene el identificador de la biblioteca.

```csharp
public string LibIdentifier { get; }
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


