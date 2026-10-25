---
title: "Enum BarItemType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.BarItemType enum. Itemtype om een balkstijl te wijzigen."
type: docs
weight: 2940
url: /nl/net/aspose.tasks.visualization/baritemtype/
---
## BarItemType enumeration

Itemtype om een balkstijl voor te wijzigen.

```csharp
public enum BarItemType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Task | `0` | Geeft taakbalkitemtype aan. |
| Summary | `1` | Geeft samenvattingsbalkitemtype aan. |
| ProjectSummary | `2` | Geeft project samenvattingsbalkitemtype aan. |
| ManualTask | `3` | Geeft handmatig taakbalkitemtype aan. |
| InactiveTask | `4` | Geeft inactief taakbalkitemtype aan. |
| CriticalTask | `5` | Geeft kritisch taakbalkitemtype aan. |
| Milestone | `6` | Geeft mijlpaal taakbalkitemtype aan. |
| ManualSummary | `7` | Geeft handmatig samenvattingsbalkitemtype aan. |
| Split | `8` | Geeft gesplitst balkitemtype aan. |
| ExternalTasks | `9` | Geeft externe taken balkitemtype aan. |
| ExternalMilestone | `10` | Geeft het type externe mijlpaalbalkitem aan. |
| Deadline | `11` | Geeft het type deadlinebalkitem aan. |
| Progress | `12` | Geeft het type voortgangsbalkitem aan. |
| StartOnly | `13` | Geeft het type alleen-startbalkitem aan. |
| FinishOnly | `14` | Geeft het type alleen-eindbalkitem aan. |
| DurationOnly | `15` | Geeft het type alleen-duurbalkitem aan. |
| InactiveMilestone | `16` | Geeft het type inactieve mijlpaalbalkitem aan. |
| InactiveSummary | `17` | Geeft het type inactieve samenvattingsbalkitem aan. |
| SummaryRollup | `18` | Samenvattingsrollupbalkitemtype. |

## Voorbeelden

Toont hoe taakbalken aan te passen met behulp van &lt;see cref=\"Aspose.Tasks.Visualization.BarStyle\" /&gt;s.

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

### Zie ook

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


