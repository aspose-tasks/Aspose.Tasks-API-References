---
title: Enum BarItemType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.BarItemType enum. Item type to change a bar style for
type: docs
weight: 2920
url: /net/aspose.tasks.visualization/baritemtype/
---
## BarItemType enumeration

Item type to change a bar style for.

```csharp
public enum BarItemType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Task | `0` | Indicates Task bar item type. |
| Summary | `1` | Indicates Summary bar item type. |
| ProjectSummary | `2` | Indicates Project summary bar item type. |
| ManualTask | `3` | Indicates Manual task bar item type. |
| InactiveTask | `4` | Indicates Inactive task bar item type. |
| CriticalTask | `5` | Indicates Critical task bar item type. |
| Milestone | `6` | Indicates Milestone task bar item type. |
| ManualSummary | `7` | Indicates Manual summary bar item type. |
| Split | `8` | Indicates Split bar item type. |
| ExternalTasks | `9` | Indicates External tasks bar item type. |
| ExternalMilestone | `10` | Indicates External milestone bar item type. |
| Deadline | `11` | Indicates Deadline bar item type. |
| Progress | `12` | Indicates Progress bar item type. |
| StartOnly | `13` | Indicates Start-only bar item type. |
| FinishOnly | `14` | Indicates Finish-only bar item type. |
| DurationOnly | `15` | Indicates Duration-only bar item type. |
| InactiveMilestone | `16` | Indicates Inactive milestone bar item type. |
| InactiveSummary | `17` | Indicates Inactive summary bar item type. |
| SummaryRollup | `18` | Summary rollup bar item type. |

## Examples

Shows how to customize task bars by using &lt;see cref="Aspose.Tasks.Visualization.BarStyle" /&gt;s.

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

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


