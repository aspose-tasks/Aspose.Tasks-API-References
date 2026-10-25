---
title: "Resource.Delete"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método del recurso. Elimina un recurso y sus asignaciones del proyecto"
type: docs
weight: 810
url: /es/net/aspose.tasks/resource/delete/
---
## Resource.Delete method

Elimina un recurso y sus asignaciones del proyecto.

```csharp
public void Delete()
```

## Ejemplos

Muestra cómo eliminar un recurso.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource = project.Resources.GetById(1);

Console.WriteLine("Number of resources (before): " + project.Resources.Count);

// eliminar el recurso
resource.Delete();

Console.WriteLine("Number of resources (after): " + project.Resources.Count);
```

### Ver también

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


