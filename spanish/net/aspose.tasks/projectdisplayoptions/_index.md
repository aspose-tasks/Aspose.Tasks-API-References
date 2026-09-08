---
title: "Clase ProjectDisplayOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.ProjectDisplayOptions. Representa las opciones de visualización para una instancia de proyecto"
type: docs
weight: 1450
url: /es/net/aspose.tasks/projectdisplayoptions/
---
## ProjectDisplayOptions class

Representa las opciones de visualización para una instancia de proyecto.

```csharp
public class ProjectDisplayOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ProjectDisplayOptions](projectdisplayoptions/)() | Inicializa una nueva instancia de la clase `ProjectDisplayOptions`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AddSpaceBeforeLabel](../../aspose.tasks/projectdisplayoptions/addspacebeforelabel/) { get; set; } | Obtiene o establece un valor que indica si se debe agregar un espacio antes del valor numérico y la abreviatura de tiempo (1 wk en lugar de 1wk). |
| [DayLabel](../../aspose.tasks/projectdisplayoptions/daylabel/) { get; set; } | Obtiene o establece cómo se muestra la etiqueta del día. |
| [HourLabel](../../aspose.tasks/projectdisplayoptions/hourlabel/) { get; set; } | Obtiene o establece cómo se muestra la etiqueta de la hora. |
| [MinuteLabel](../../aspose.tasks/projectdisplayoptions/minutelabel/) { get; set; } | Obtiene o establece cómo se muestra la etiqueta del minuto. |
| [MonthLabel](../../aspose.tasks/projectdisplayoptions/monthlabel/) { get; set; } | Obtiene o establece cómo se muestra la etiqueta del mes. |
| [ShowProjectSummaryTask](../../aspose.tasks/projectdisplayoptions/showprojectsummarytask/) { get; set; } | Obtiene o establece un valor que indica si se debe mostrar información resumida de todo un proyecto en una sola fila con su propia barra de tarea resumen en la parte superior de la vista de diagrama de Gantt. |
| [ShowTaskScheduleSuggestions](../../aspose.tasks/projectdisplayoptions/showtaskschedulesuggestions/) { get; set; } | Obtiene o establece un valor que indica si se deben mostrar sugerencias cuando Project identifica un posible conflicto de programación con una tarea programada manualmente. Esta opción está disponible para la versión Project 2010 y posteriores. |
| [ShowTaskScheduleWarnings](../../aspose.tasks/projectdisplayoptions/showtaskschedulewarnings/) { get; set; } | Obtiene o establece un valor que indica si se deben mostrar advertencias cuando Project identifica un posible conflicto de programación con una tarea programada manualmente. Esta opción está disponible para la versión Project 2010 y posteriores. |
| [UnderlineHyperlinks](../../aspose.tasks/projectdisplayoptions/underlinehyperlinks/) { get; set; } | Obtiene o establece un valor que indica si se deben subrayar los hipervínculos. |
| [WeekLabel](../../aspose.tasks/projectdisplayoptions/weeklabel/) { get; set; } | Obtiene o establece cómo se muestra la etiqueta de la semana. |
| [YearLabel](../../aspose.tasks/projectdisplayoptions/yearlabel/) { get; set; } | Obtiene o establece cómo se muestra la etiqueta del año. |

## Ejemplos

Muestra cómo usar las opciones de visualización del proyecto.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Establece un valor que indica si se deben mostrar advertencias cuando Project identifica un posible conflicto de programación con una tarea programada manualmente.
// Esta opción está disponible para la versión Project 2010 y posteriores.
project.DisplayOptions.ShowTaskScheduleWarnings = false;

// un valor que indica si se debe agregar un espacio antes del valor numérico y la abreviatura de tiempo (1 wk en lugar de 1wk)
project.DisplayOptions.AddSpaceBeforeLabel = true;

// establece cómo se muestra la etiqueta de minuto
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.Min;

// establece cómo se muestra la etiqueta de hora
project.DisplayOptions.HourLabel = HourLabelDisplay.Hr;

// establece cómo se muestra la etiqueta del día
project.DisplayOptions.DayLabel = DayLabelDisplay.Dy;

// establece cómo se muestra la etiqueta de la semana
project.DisplayOptions.WeekLabel = WeekLabelDisplay.Week;

// establecer cómo se muestra la etiqueta del mes
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mon;

// establece cómo se muestra la etiqueta del año
project.DisplayOptions.YearLabel = YearLabelDisplay.Year;

// establece un valor que indica si se debe mostrar información resumida de todo el proyecto en una sola fila con su propia barra de tarea resumida en la parte superior de la vista del diagrama de Gantt.
project.DisplayOptions.ShowProjectSummaryTask = true;

// establece un valor que indica si se deben mostrar sugerencias cuando Project identifica un posible conflicto de programación con una tarea programada manualmente.
project.DisplayOptions.ShowTaskScheduleSuggestions = true;

// establece un valor que indica si se deben subrayar los hipervínculos.
project.DisplayOptions.UnderlineHyperlinks = true;

project.Save(OutDir + "WorkWithProjectDisplayOptions.mpp", SaveFileFormat.Mpp);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


