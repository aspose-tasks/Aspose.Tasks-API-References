---
title: Enum GanttBarShowFor
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.GanttBarShowFor enum. Represents categories of tasks used when customizing Bar Styles of Gantt chart
type: docs
weight: 3010
url: /net/aspose.tasks.visualization/ganttbarshowfor/
---
## GanttBarShowFor enumeration

Represents categories of tasks used when customizing Bar Styles of Gantt chart.

```csharp
public enum GanttBarShowFor
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Normal | `0` | Normal category. |
| Milestone | `1` | Milestone category. |
| Summary | `2` | Summary category. |
| Critical | `3` | Critical category. |
| Noncritical | `4` | Noncritical category. |
| Marked | `5` | Marked category. |
| Finished | `6` | Finished category. |
| InProgress | `7` | InProgress category. |
| NotFinished | `8` | Not Finished category. |
| NotStarted | `9` | Not Started category. |
| StartedLate | `10` | Started Late. |
| FinishedLate | `11` | Finished Late category. |
| StartedEarly | `12` | Started Early category. |
| FinishedEarly | `13` | Finished Early category. |
| StartedOnTime | `14` | Started On Time category. |
| FinishedOnTime | `15` | Finished On Time category. |
| Flag1 | `16` | Flag1 category. |
| Flag2 | `17` | Flag2 category. |
| Flag3 | `18` | Flag3 category. |
| Flag4 | `19` | Flag4 category. |
| Flag5 | `20` | Flag5 category. |
| Flag6 | `21` | Flag6 category. |
| Flag7 | `22` | Flag7 category. |
| Flag8 | `23` | Flag8 category. |
| Flag9 | `24` | Flag9 category. |
| Flag10 | `25` | Flag10 category. |
| RolledUp | `26` | Rolled Up category. |
| ProjectSummary | `27` | Project Summary category. |
| Split | `28` | Split category. |
| ExternalTasks | `29` | External Tasks category. |
| Flag11 | `30` | Flag11 category. |
| Flag12 | `31` | Flag12 category. |
| Flag13 | `32` | Flag13 category. |
| Flag14 | `33` | Flag14 category. |
| Flag15 | `34` | Flag15 category. |
| Flag16 | `35` | Flag16 category. |
| Flag17 | `36` | Flag17 category. |
| Flag18 | `37` | Flag18 category. |
| Flag19 | `38` | Flag19 category. |
| Flag20 | `39` | Flag20 category. |
| GroupBySummary | `40` | Group By Summary category. |
| Deliverable | `41` | Deliverable category. |
| Dependency | `42` | Dependency category. |
| Active | `43` | Active category. |
| ManuallyScheduled | `44` | Manually Scheduled category. |
| Warning | `45` | Warning category. |
| PlaceholderStart | `46` | Placeholder (Start) category. |
| PlaceholderFinish | `47` | Placeholder (Finish) category. |
| PlaceholderDuration | `48` | Placeholder (Duration) category. |
| Placeholder | `49` | Placeholder category. |
| Late | `50` | Late category. |
| NotNormal | `64` | Not Normal |
| NotMilestone | `65` | Not Milestone category. |
| NotSummary | `66` | Not Summary category. |
| NotCritical | `67` | Not Critical category. |
| NotMarked | `69` | Not Marked = 69 category. |
| NotInProgress | `71` | Not In Progress = 71 category. |
| NotStartedLate | `74` | Not Started Late = 74 category. |
| NotFinishedLate | `75` | Not Finished Late category. |
| NotStartedEarly | `76` | Not Started Early category. |
| NotFinishedEarly | `77` | Not Finished Early category. |
| NotStartedOnTime | `78` | Not Started On Time category. |
| NotFinishedOnTime | `79` | Not Finished On Time category. |
| NotFlag1 | `80` | Not Flag1 category. |
| NotFlag2 | `81` | Not Flag2 category. |
| NotFlag3 | `82` | Not Flag3 category. |
| NotFlag4 | `83` | Not Flag4 category. |
| NotFlag5 | `84` | Not Flag5 category. |
| NotFlag6 | `85` | Not Flag6 category. |
| NotFlag7 | `86` | Not Flag7 category. |
| NotFlag8 | `87` | Not Flag8 category. |
| NotFlag9 | `88` | Not Flag9 category. |
| NotFlag10 | `89` | Not Flag10 category. |
| NotRolledUp | `90` | Not Rolled Up category. |
| NotProjectSummary | `91` | Not Project Summary category. |
| NotSplit | `92` | Not Split category. |
| NotExternalTasks | `93` | Not External Tasks category. |
| NotFlag11 | `94` | Not Flag11 category. |
| NotFlag12 | `95` | Not Flag12 category. |
| NotFlag13 | `96` | Not Flag13 category. |
| NotFlag14 | `97` | Not Flag14 category. |
| NotFlag15 | `98` | Not Flag15 category. |
| NotFlag16 | `99` | Not Flag16 category. |
| NotFlag17 | `100` | Not Flag17 category. |
| NotFlag18 | `101` | Not Flag18 category. |
| NotFlag19 | `102` | Not Flag19 category. |
| NotFlag20 | `103` | Not Flag20 category. |
| NotGroupBySummary | `104` | Not Group By Summary category. |
| NotDeliverable | `105` | Not Deliverable category. |
| NotDependency | `106` | Not Dependency category. |
| NotActive | `107` | Not Active category. |
| NotManuallyScheduled | `108` | Not Manually Scheduled category. |
| NotWarning | `109` | Not Warning category. |
| NotPlaceholderStart | `110` | Not Placeholder (Start) category. |
| NotPlaceholderFinish | `111` | Not Placeholder (Finish) category. |
| NotPlaceholderDuration | `112` | Not Placeholder (Duration) category. |
| NotPlaceholder | `113` | Not Placeholder category. |
| NotLate | `114` | Not Late category. |

## Remarks

See 'Bar Styles' dialog of Gantt chart, 'Show For' column.

## Examples

Shows how to use ShowFor categories.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var view = (GanttChartView)project.DefaultView;

var barStyle = this.GetCustomBarStyle();
barStyle.ShowForTaskUid = null;

var showForCategories = new[]
{
    GanttBarShowFor.Active,
    GanttBarShowFor.NotSummary,
    GanttBarShowFor.Milestone,
    GanttBarShowFor.Finished
};

barStyle.ShowForCategories = new List<GanttBarShowFor>(showForCategories);
barStyle.Name = "My common style";
view.BarStyles.Add(barStyle);

// work with project...
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


