---
title: "ResourceAssignment.GetHashCode"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ResourceAssignment. Devuelve un valor de código hash para la instancia de la clase ResourceAssignment"
type: docs
weight: 710
url: /es/net/aspose.tasks/resourceassignment/gethashcode/
---
## ResourceAssignment.GetHashCode method

Devuelve un valor de código hash para la instancia de la clase [`ResourceAssignment`](../).

```csharp
public override int GetHashCode()
```

### Valor devuelto

devuelve un valor de código hash para este objeto.

## Ejemplos

Muestra cómo obtener un código hash de una asignación de recurso.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(2);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(3);

// imprimir códigos hash de la asignación
Console.WriteLine("Resource Assignment 1 Hash Code: {0}", resourceAssignment1.GetHashCode());
Console.WriteLine("Resource Assignment 2 Hash Code: {0}", resourceAssignment2.GetHashCode());
```

### Ver también

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


