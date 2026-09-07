---
title: "Enum BarItemType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.BarItemType enum. Τύπος στοιχείου για την αλλαγή του στυλ μιας μπάρας"
type: docs
weight: 2940
url: /el/net/aspose.tasks.visualization/baritemtype/
---
## BarItemType enumeration

Τύπος στοιχείου για αλλαγή του στυλ μπάρας.

```csharp
public enum BarItemType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Task | `0` | Υποδεικνύει Task bar item type. |
| Summary | `1` | Υποδεικνύει Summary bar item type. |
| ProjectSummary | `2` | Υποδεικνύει Project summary bar item type. |
| ManualTask | `3` | Υποδεικνύει Manual task bar item type. |
| InactiveTask | `4` | Υποδεικνύει Inactive task bar item type. |
| CriticalTask | `5` | Υποδεικνύει Critical task bar item type. |
| Milestone | `6` | Υποδεικνύει Milestone task bar item type. |
| ManualSummary | `7` | Υποδεικνύει Manual summary bar item type. |
| Split | `8` | Υποδεικνύει Split bar item type. |
| ExternalTasks | `9` | Υποδεικνύει External tasks bar item type. |
| ExternalMilestone | `10` | Δείχνει τύπο στοιχείου γραμμής εξωτερικού ορόσημου. |
| Deadline | `11` | Δείχνει τύπο στοιχείου γραμμής προθεσμίας. |
| Progress | `12` | Δείχνει τύπο στοιχείου γραμμής προόδου. |
| StartOnly | `13` | Δείχνει τύπο στοιχείου γραμμής μόνο έναρξης. |
| FinishOnly | `14` | Δείχνει τύπο στοιχείου γραμμής μόνο λήξης. |
| DurationOnly | `15` | Δείχνει τύπο στοιχείου γραμμής μόνο διάρκειας. |
| InactiveMilestone | `16` | Δείχνει τύπο στοιχείου γραμμής ανενεργού ορόσημου. |
| InactiveSummary | `17` | Δείχνει τύπο στοιχείου γραμμής ανενεργής σύνοψης. |
| SummaryRollup | `18` | Τύπος στοιχείου γραμμής συγκεντρωτικής σύνοψης. |

## Παραδείγματα

Δείχνει πώς να προσαρμόσετε τις γραμμές εργασιών χρησιμοποιώντας &lt;see cref=\"Aspose.Tasks.Visualization.BarStyle\" /&gt;s.

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

### Δείτε επίσης

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


