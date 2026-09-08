---
title: "MPPSaveOptions.WriteViewData"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad MPPSaveOptions. Obtiene o establece un valor que indica si se deben escribir datos de vista al guardar un proyecto en formato MPP. Los datos de vista incluyen las colecciones Project.Views Filters y Tables."
type: docs
weight: 80
url: /es/net/aspose.tasks.saving/mppsaveoptions/writeviewdata/
---
## MPPSaveOptions.WriteViewData property

Obtiene o establece un valor que indica si se deben escribir los datos de vista al guardar un proyecto en formato MPP. Los datos de vista incluyen las colecciones Project.Views, Filters y Tables.

```csharp
public bool WriteViewData { get; set; }
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


