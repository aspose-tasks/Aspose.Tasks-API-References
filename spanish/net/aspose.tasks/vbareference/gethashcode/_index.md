---
title: "VbaReference.GetHashCode"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método VbaReference. Devuelve un valor de código hash para este VbaReference"
type: docs
weight: 50
url: /es/net/aspose.tasks/vbareference/gethashcode/
---
## VbaReference.GetHashCode method

Devuelve un valor de código hash para este [`VbaReference`](../).

```csharp
public override int GetHashCode()
```

### Valor devuelto

Devuelve un valor de código hash para este objeto.

## Ejemplos

Muestra cómo obtener un código hash de una referencia VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// El código hash de una referencia es el código hash del GUID interno de la referencia.
Console.WriteLine("VBA reference Hash Code: {0}", reference1.GetHashCode());
Console.WriteLine("VBA reference Hash Code: {0}", reference2.GetHashCode());
```

### Ver también

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


