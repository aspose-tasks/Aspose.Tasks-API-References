---
title: "Enum BarItemType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.Visualization.BarItemType enum. Tipo de elemento para cambiar el estilo de una barra."
type: docs
weight: 2940
url: /es/net/aspose.tasks.visualization/baritemtype/
---
## BarItemType enumeration

Tipo de elemento para cambiar un estilo de barra.

```csharp
public enum BarItemType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Task | `0` | Indica el tipo de elemento de barra de tarea. |
| Summary | `1` | Indica el tipo de elemento de barra de resumen. |
| ProjectSummary | `2` | Indica el tipo de elemento de barra de resumen del proyecto. |
| ManualTask | `3` | Indica el tipo de elemento de barra de tarea manual. |
| InactiveTask | `4` | Indica el tipo de elemento de barra de tarea inactiva. |
| CriticalTask | `5` | Indica el tipo de elemento de barra de tarea crítica. |
| Milestone | `6` | Indica el tipo de elemento de barra de tarea de hito. |
| ManualSummary | `7` | Indica el tipo de elemento de barra de resumen manual. |
| Split | `8` | Indica el tipo de elemento de barra dividida. |
| ExternalTasks | `9` | Indica el tipo de elemento de barra de tareas externas. |
| ExternalMilestone | `10` | Indica el tipo de elemento de barra de hito externo. |
| Deadline | `11` | Indica el tipo de elemento de barra de fecha límite. |
| Progress | `12` | Indica el tipo de elemento de barra de progreso. |
| StartOnly | `13` | Indica el tipo de elemento de barra solo de inicio. |
| FinishOnly | `14` | Indica el tipo de elemento de barra solo de finalización. |
| DurationOnly | `15` | Indica el tipo de elemento de barra solo de duración. |
| InactiveMilestone | `16` | Indica el tipo de elemento de barra de hito inactivo. |
| InactiveSummary | `17` | Indica el tipo de elemento de barra de resumen inactivo. |
| SummaryRollup | `18` | Tipo de elemento de barra de resumen acumulado. |

## Ejemplos

Muestra cómo personalizar las barras de tareas usando &lt;see cref=\"Aspose.Tasks.Visualization.BarStyle\" /&gt;s.

```csharp
var project = new Project();

var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

var task3 = project.RootTask.Children.Add("Task 3");
var rsc1 = project.Resources.Add("Resource 1");
var rsc2 = project.Resources.Add("Resource 2");
var rsc3 = project.Resources.Add("Resource 3");

project.ResourceAssignments.Add(task1, rsc1);
project.ResourceAssignments.Add(task2, rsc2);
project.ResourceAssignments.Add(task3, rsc3);

SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.ThirdsOfMonths
};

var style = new BarStyle
                {
                    ItemType = BarItemType.CriticalTask,
                    LeftBarTextConverter = delegate(Task t)
                    {
                        return string.Format("This task (ID = {0}) is on critical path", t.Get(Tsk.Id));
                    }
                };

var style2 = new BarStyle { BarColor = Color.DarkOrchid, ItemType = BarItemType.Task };

options.BarStyles = new List<BarStyle> { style, style2 };

project.Save(OutDir + "CustomizeTextWithTaskBars_out.pdf", options);
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


