---
title: "Clase PrimaveraXmlSaveOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Saving.PrimaveraXmlSaveOptions. Permite especificar opciones adicionales al guardar el proyecto en formato XML de Primavera"
type: docs
weight: 2160
url: /es/net/aspose.tasks.saving/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions class

Permite especificar opciones adicionales al guardar el proyecto en formato XML de Primavera.

```csharp
public class PrimaveraXmlSaveOptions : SimpleSaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PrimaveraXmlSaveOptions](primaveraxmlsaveoptions/)() | Inicializa una nueva instancia de la clase `PrimaveraXmlSaveOptions`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Obtiene o establece el formato en el que se guardará el documento si se utiliza este objeto de opciones de guardado. |
| [SaveRootTask](../../aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/) { get; set; } | Obtiene o establece un valor que indica si guardar una tarea raíz o no. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/) { get; set; } | Obtiene o establece un valor que indica si se deben omitir las asignaciones de recursos a tareas resumidas durante la exportación. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Obtiene o establece el comparador para ordenar tareas en el diagrama de Gantt y en el diagrama de hoja de tareas. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Obtiene o establece la condición que se utiliza para filtrar las tareas renderizadas en los diagramas de Gantt, hoja de tareas y uso de tareas. |

## Ejemplos

Muestra cómo exportar al archivo XML de Primavera.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### Ver también

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


