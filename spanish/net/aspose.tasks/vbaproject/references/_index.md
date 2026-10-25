---
title: "VbaProject.References"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad VbaProject. Obtiene una colección de VbaReferenceCollection"
type: docs
weight: 70
url: /es/net/aspose.tasks/vbaproject/references/
---
## VbaProject.References property

Obtiene una colección de [`VbaReferenceCollection`](../../vbareferencecollection/)

```csharp
public VbaReferenceCollection References { get; }
```

## Ejemplos

Muestra cómo leer la información de referencias del proyecto VBA.

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

* class [VbaReferenceCollection](../../vbareferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


