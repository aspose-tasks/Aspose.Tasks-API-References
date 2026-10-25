---
title: "Перечисление BarItemType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.Visualization.BarItemType. Тип элемента для изменения стиля полосы"
type: docs
weight: 2940
url: /ru/net/aspose.tasks.visualization/baritemtype/
---
## BarItemType enumeration

Тип элемента, для которого изменяется стиль полосы.

```csharp
public enum BarItemType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Task | `0` | Указывает тип элемента полосы задачи. |
| Summary | `1` | Указывает тип элемента полосы сводки. |
| ProjectSummary | `2` | Указывает тип элемента полосы сводки проекта. |
| ManualTask | `3` | Указывает тип элемента полосы ручной задачи. |
| InactiveTask | `4` | Указывает тип элемента полосы неактивной задачи. |
| CriticalTask | `5` | Указывает тип элемента полосы критической задачи. |
| Milestone | `6` | Указывает тип элемента полосы веховой задачи. |
| ManualSummary | `7` | Указывает тип элемента полосы ручной сводки. |
| Split | `8` | Указывает тип элемента полосы разделения. |
| ExternalTasks | `9` | Указывает тип элемента полосы внешних задач. |
| ExternalMilestone | `10` | Указывает тип элемента внешней контрольной точки. |
| Deadline | `11` | Указывает тип элемента срока. |
| Progress | `12` | Указывает тип элемента прогресса. |
| StartOnly | `13` | Указывает тип элемента только начала. |
| FinishOnly | `14` | Указывает тип элемента только завершения. |
| DurationOnly | `15` | Указывает тип элемента только длительности. |
| InactiveMilestone | `16` | Указывает тип неактивной контрольной точки. |
| InactiveSummary | `17` | Указывает тип неактивного сводного элемента. |
| SummaryRollup | `18` | Тип элемента сводного объединения. |

## Примеры

Показывает, как настроить полосы задач, используя &lt;see cref=\"Aspose.Tasks.Visualization.BarStyle\" /&gt;s.

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

### См. также

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


