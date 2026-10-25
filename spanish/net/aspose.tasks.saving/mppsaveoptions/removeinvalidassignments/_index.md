---
title: "MPPSaveOptions.RemoveInvalidAssignments"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad MPPSaveOptions. Obtiene o establece un valor que indica si se deben eliminar asignaciones de recursos inválidas al guardar en MPP. MS Project crea una asignación de recurso vacía para cada tarea. Establezca este indicador en true para eliminarlas al guardar."
type: docs
weight: 40
url: /es/net/aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/
---
## MPPSaveOptions.RemoveInvalidAssignments property

Obtiene o establece un valor que indica si se deben eliminar asignaciones de recursos no válidas al guardar en MPP. MS Project crea una asignación de recursos vacía para cada tarea. Establezca este indicador en true para eliminarlas al guardar.

```csharp
public bool RemoveInvalidAssignments { get; set; }
```

## Ejemplos

Muestra cómo guardar el proyecto en un flujo como un archivo MPP.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

    // crear opciones de guardado
    SimpleSaveOptions options = new MPPSaveOptions
    {
        // establece un valor que indica si se deben eliminar asignaciones de recursos no válidas al guardar en MPP
        RemoveInvalidAssignments = true
    };

    // guardar MPP con opciones
    project.Save(stream, options);
}
```

### Ver también

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


