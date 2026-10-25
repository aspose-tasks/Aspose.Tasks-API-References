---
title: "Enum BarItemType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Visualization.BarItemType enum. Tipo di elemento per cambiare lo stile di una barra"
type: docs
weight: 2940
url: /it/net/aspose.tasks.visualization/baritemtype/
---
## BarItemType enumeration

Tipo di elemento per cui modificare lo stile di una barra.

```csharp
public enum BarItemType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Task | `0` | Indica il tipo di elemento barra per attività. |
| Summary | `1` | Indica il tipo di elemento barra per riepilogo. |
| ProjectSummary | `2` | Indica il tipo di elemento barra per riepilogo del progetto. |
| ManualTask | `3` | Indica il tipo di elemento barra per attività manuale. |
| InactiveTask | `4` | Indica il tipo di elemento barra per attività inattiva. |
| CriticalTask | `5` | Indica il tipo di elemento barra per attività critica. |
| Milestone | `6` | Indica il tipo di elemento barra per attività milestone. |
| ManualSummary | `7` | Indica il tipo di elemento barra per riepilogo manuale. |
| Split | `8` | Indica il tipo di elemento barra per divisione. |
| ExternalTasks | `9` | Indica il tipo di elemento barra per attività esterne. |
| ExternalMilestone | `10` | Indica il tipo di elemento barra per traguardo esterno. |
| Deadline | `11` | Indica il tipo di elemento barra per scadenza. |
| Progress | `12` | Indica il tipo di elemento barra per avanzamento. |
| StartOnly | `13` | Indica il tipo di elemento barra solo di inizio. |
| FinishOnly | `14` | Indica il tipo di elemento barra solo di fine. |
| DurationOnly | `15` | Indica il tipo di elemento barra solo di durata. |
| InactiveMilestone | `16` | Indica il tipo di elemento barra per traguardo inattivo. |
| InactiveSummary | `17` | Indica il tipo di elemento barra per riepilogo inattivo. |
| SummaryRollup | `18` | Tipo di elemento barra per riepilogo aggregato. |

## Esempi

Mostra come personalizzare le barre delle attività utilizzando &lt;see cref="Aspose.Tasks.Visualization.BarStyle" /&gt;s.

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

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


