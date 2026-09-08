---
title: "Project.RemoveInvalidResourceAssignments"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método del proyecto. Elimina asignaciones de recursos no válidas de la lista de asignaciones de recursos del proyecto"
type: docs
weight: 1170
url: /es/net/aspose.tasks/project/removeinvalidresourceassignments/
---
## Project.RemoveInvalidResourceAssignments method

Elimina asignaciones de recursos inválidas de la lista de asignaciones de recursos del proyecto.

```csharp
public void RemoveInvalidResourceAssignments()
```

## Observaciones

MS Project crea una asignación de recurso vacía para cada tarea. Llama al método para eliminarlas.

## Ejemplos

Muestra cómo eliminar asignaciones no válidas.

```csharp
var project = new Project(DataDir + "InvalidResourceAssignments.mpp");
var invalid = 0;

// ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
foreach (var ra in project.ResourceAssignments)
{
    if (ra.Get(Asn.Resource) == null)
    {
        invalid++;
    }
}

Console.WriteLine("Count of invalid assignments (before): " + invalid);

// eliminar asignaciones no válidas
project.RemoveInvalidResourceAssignments();

Console.WriteLine("Count of invalid assignments (after): " + invalid);
```

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


