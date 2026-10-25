---
title: "Clase MPPSaveOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Saving.MPPSaveOptions. Permite especificar opciones adicionales al guardar los datos del proyecto en MPP"
type: docs
weight: 2050
url: /es/net/aspose.tasks.saving/mppsaveoptions/
---
## MPPSaveOptions class

Permite especificar opciones adicionales al guardar datos del proyecto en MPP.

```csharp
public class MPPSaveOptions : SimpleSaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [MPPSaveOptions](mppsaveoptions/)() | Inicializa una nueva instancia de la clase `MPPSaveOptions`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ClearVba](../../aspose.tasks.saving/mppsaveoptions/clearvba/) { get; set; } | Obtiene o establece un valor que indica si se deben eliminar los datos de macros VBA existentes al guardar un proyecto en formato MPP. |
| [ProtectionPassword](../../aspose.tasks.saving/mppsaveoptions/protectionpassword/) { get; set; } | Obtiene o establece una contraseña que se utiliza para proteger el archivo MPP resultante. Actualmente se admite para los formatos de MS Project 2010 y posteriores. Un valor nulo indica que el archivo del proyecto no está protegido. |
| [RemoveInvalidAssignments](../../aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/) { get; set; } | Obtiene o establece un valor que indica si se deben eliminar asignaciones de recursos no válidas al guardar en MPP. MS Project crea una asignación de recursos vacía para cada tarea. Establezca este indicador en true para eliminarlas al guardar. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Obtiene o establece el formato en el que se guardará el documento si se utiliza este objeto de opciones de guardado. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Obtiene o establece el comparador para ordenar tareas en el diagrama de Gantt y en el diagrama de hoja de tareas. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Obtiene o establece la condición que se utiliza para filtrar las tareas renderizadas en los diagramas de Gantt, hoja de tareas y uso de tareas. |
| [WriteFilters](../../aspose.tasks.saving/mppsaveoptions/writefilters/) { get; set; } | Obtiene o establece un valor que indica si se deben escribir los datos de filtros al guardar un proyecto en formato MPP. Los datos de filtros incluyen las colecciones Project.TaskFilters y Project.ResourceFilters. |
| [WriteGroups](../../aspose.tasks.saving/mppsaveoptions/writegroups/) { get; set; } | Obtiene o establece un valor que indica si se deben escribir los datos de grupos al guardar un proyecto en formato MPP. Los datos de grupos incluyen las colecciones Project.TaskGroups y Project.ResourceGroups. |
| [WriteVba](../../aspose.tasks.saving/mppsaveoptions/writevba/) { get; set; } | Obtiene o establece un valor que indica si se deben actualizar los datos de macros VBA existentes en el archivo MPP. Actualmente se admite la escritura de VbaModule.SourceCode. |
| [WriteViewData](../../aspose.tasks.saving/mppsaveoptions/writeviewdata/) { get; set; } | Obtiene o establece un valor que indica si se deben escribir los datos de vista al guardar un proyecto en formato MPP. Los datos de vista incluyen las colecciones Project.Views, Filters y Tables. |

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


