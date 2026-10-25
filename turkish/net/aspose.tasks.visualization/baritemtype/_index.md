---
title: "Enum BarItemType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.BarItemType enum. Bir çubuk stilini değiştirmek için öğe türü"
type: docs
weight: 2940
url: /tr/net/aspose.tasks.visualization/baritemtype/
---
## BarItemType enumeration

Bir çubuk stilini değiştirmek için öğe türü.

```csharp
public enum BarItemType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Task | `0` | Görev çubuğu öğesi türünü gösterir. |
| Summary | `1` | Özet çubuğu öğesi türünü gösterir. |
| ProjectSummary | `2` | Proje özeti çubuğu öğesi türünü gösterir. |
| ManualTask | `3` | Manuel görev çubuğu öğesi türünü gösterir. |
| InactiveTask | `4` | Pasif görev çubuğu öğesi türünü gösterir. |
| CriticalTask | `5` | Kritik görev çubuğu öğesi türünü gösterir. |
| Milestone | `6` | Kilometre taşı görev çubuğu öğesi türünü gösterir. |
| ManualSummary | `7` | Manuel özet çubuğu öğesi türünü gösterir. |
| Split | `8` | Bölünmüş çubuk öğesi türünü gösterir. |
| ExternalTasks | `9` | Harici görevler çubuğu öğesi türünü gösterir. |
| ExternalMilestone | `10` | Harici kilometre taşı çubuk öğesi türünü belirtir. |
| Deadline | `11` | Son tarih çubuk öğesi türünü belirtir. |
| Progress | `12` | İlerleme çubuk öğesi türünü belirtir. |
| StartOnly | `13` | Yalnızca başlangıç çubuk öğesi türünü belirtir. |
| FinishOnly | `14` | Yalnızca bitiş çubuk öğesi türünü belirtir. |
| DurationOnly | `15` | Yalnızca süre çubuk öğesi türünü belirtir. |
| InactiveMilestone | `16` | Etkin olmayan kilometre taşı çubuk öğesi türünü belirtir. |
| InactiveSummary | `17` | Etkin olmayan özet çubuk öğesi türünü belirtir. |
| SummaryRollup | `18` | Özet toplama çubuk öğesi türü. |

## Örnekler

Görev çubuklarını özelleştirmenin nasıl yapılacağını &lt;see cref=\"Aspose.Tasks.Visualization.BarStyle\" /&gt; kullanarak gösterir.

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

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


