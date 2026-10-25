---
title: "Class PrimaveraSaveOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.Saving.PrimaveraSaveOptions class. Permite especificar opciones adicionales al guardar el proyecto en formato Primavera XER"
type: docs
weight: 2150
url: /es/net/aspose.tasks.saving/primaverasaveoptions/
---
## PrimaveraSaveOptions class

Permite especificar opciones adicionales al guardar el proyecto en formato Primavera XER.

```csharp
public class PrimaveraSaveOptions : SimpleSaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PrimaveraSaveOptions](primaverasaveoptions/)() | Inicializa una nueva instancia de la clase `PrimaveraSaveOptions`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ActivityIdIncrement](../../aspose.tasks.saving/primaverasaveoptions/activityidincrement/) { get; set; } | Obtiene o establece el incremento utilizado al renumerar los IDs de actividad. |
| [ActivityIdPrefix](../../aspose.tasks.saving/primaverasaveoptions/activityidprefix/) { get; set; } | Obtiene o establece el prefijo utilizado al renumerar los IDs de actividad. |
| [ActivityIdSuffix](../../aspose.tasks.saving/primaverasaveoptions/activityidsuffix/) { get; set; } | Obtiene o establece el sufijo utilizado al renumerar los IDs de actividad. |
| [RenumberActivityIds](../../aspose.tasks.saving/primaverasaveoptions/renumberactivityids/) { get; set; } | Obtiene o establece un valor que indica si es necesario renumerar los IDs de actividad. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Obtiene o establece el formato en el que se guardará el documento si se utiliza este objeto de opciones de guardado. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaverasaveoptions/skipsummaryassignments/) { get; set; } | Obtiene o establece un valor que indica si se deben omitir las asignaciones de recursos a tareas resumidas durante la exportación. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Obtiene o establece el comparador para ordenar tareas en el diagrama de Gantt y en el diagrama de hoja de tareas. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Obtiene o establece la condición que se utiliza para filtrar las tareas renderizadas en los diagramas de Gantt, hoja de tareas y uso de tareas. |

## Ejemplos

Muestra cómo trabajar con &lt;see cref=\"Aspose.Tasks.Saving.PrimaveraSaveOptions\" /&gt;.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// crear opciones de guardado Primavera y afinarlas
var options = new PrimaveraSaveOptions
                  {
                      // definir prefijo y sufijo de una actividad
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // controlar la renumeración de actividades
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### Ver también

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


