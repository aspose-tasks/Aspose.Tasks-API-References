---
title: "枚举 TaskKey"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TaskKey 枚举。表示受支持任务字段的列表"
type: docs
weight: 2400
url: /zh/net/aspose.tasks/taskkey/
---
## TaskKey enumeration

表示受支持的任务字段列表。

```csharp
public enum TaskKey : byte
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Uid | `0` | 表示唯一标识 (Task) 字段。 |
| Id | `1` | 表示标识 (Task) 字段。 |
| Name | `2` | 表示名称 (Task) 字段。 |
| Type | `3` | 表示类型 (Task) 字段。 |
| IsNull | `4` | 表示是否为空 (Task) 字段。 |
| Created | `5` | 表示创建时间 (Task) 字段。 |
| Contact | `6` | 表示联系人 (Task) 字段。 |
| WBS | `7` | 表示 WBS (Task) 字段。 |
| WBSLevel | `8` | 表示 WBSLevel (Task) 字段。 |
| OutlineNumber | `9` | 表示大纲编号 (Task) 字段。 |
| OutlineLevel | `10` | 表示大纲级别 (Task) 字段。 |
| Priority | `11` | 表示优先级 (Task) 字段。 |
| Start | `12` | 表示开始时间 (Task) 字段。 |
| Finish | `13` | 表示完成时间 (Task) 字段。 |
| Duration | `14` | 表示持续时间 (Task) 字段。 |
| DurationVariance | `15` | 表示持续时间差异 (Task) 字段。 |
| Work | `16` | 表示工作量 (Task) 字段。 |
| Stop | `17` | 表示停止时间 (Task) 字段。 |
| Resume | `18` | 表示恢复时间 (Task) 字段。 |
| IsResumeValid | `19` | 表示恢复是否有效 (Task) 字段。 |
| IsEffortDriven | `20` | 表示是否按工作量驱动 (Task) 字段。 |
| IsRecurring | `21` | 表示是否循环 (Task) 字段。 |
| IsOverallocated | `22` | 表示是否超额分配 (Task) 字段。 |
| HasOverallocatedResource | `23` | 表示是否有超额分配资源 (Task) 字段。 |
| IsEstimated | `24` | 表示是否为估计 (Task) 字段。 |
| IsMilestone | `25` | 表示 IsMilestone（Task）字段。 |
| IsCritical | `26` | 表示 IsCritical（Task）字段。 |
| IsSubproject | `27` | 表示 IsSubproject（Task）字段。 |
| IsSubprojectReadOnly | `28` | 表示 IsSubprojectReadOnly（Task）字段。 |
| IsMarked | `29` | 表示 IsMarked（Task）字段。 |
| IgnoreWarnings | `30` | 表示 IgnoreWarnings（Task）字段。 |
| SubprojectName | `31` | 表示 SubprojectName（Task）字段。 |
| IsExternalTask | `32` | 表示 IsExternalTask（Task）字段。 |
| IsSummary | `33` | 表示 IsSummary（Task）字段。 |
| ExternalTaskProject | `34` | 表示 ExternalTaskProject（Task）字段。 |
| ExternalId | `35` | 表示 ExternalId（Task）字段。 |
| EarlyStart | `36` | 表示 EarlyStart（Task）字段。 |
| EarlyFinish | `37` | 表示 EarlyFinish（Task）字段。 |
| LateStart | `38` | 表示 LateStart（Task）字段。 |
| LateFinish | `39` | 表示 LateFinish（Task）字段。 |
| StartVariance | `40` | 表示 StartVariance（Task）字段。 |
| FinishVariance | `41` | 表示 FinishVariance（Task）字段。 |
| WorkVariance | `42` | 表示 WorkVariance（Task）字段。 |
| CostVariance | `43` | 表示 CostVariance（Task）字段。 |
| FreeSlack | `44` | 表示 FreeSlack（Task）字段。 |
| TotalSlack | `45` | 表示 TotalSlack（Task）字段。 |
| StartSlack | `46` | 表示 StartSlack（Task）字段。 |
| FinishSlack | `47` | 表示 FinishSlack（Task）字段。 |
| FixedCost | `48` | 表示 FixedCost（Task）字段。 |
| FixedCostAccrual | `49` | 表示 FixedCostAccrual（Task）字段。 |
| PercentComplete | `50` | 表示 PercentComplete (Task) 字段。 |
| PercentWorkComplete | `51` | 表示 PercentWorkComplete (Task) 字段。 |
| Cost | `52` | 表示 Cost (Task) 字段。 |
| OvertimeCost | `53` | 表示 OvertimeCost (Task) 字段。 |
| ActualStart | `54` | 表示 ActualStart (Task) 字段。 |
| ActualFinish | `55` | 表示 ActualFinish (Task) 字段。 |
| ActualDuration | `56` | 表示 ActualDuration (Task) 字段。 |
| ActualCost | `57` | 表示 ActualCost (Task) 字段。 |
| ActualOvertimeCost | `58` | 表示 ActualOvertimeCost (Task) 字段。 |
| ActualWork | `59` | 表示 ActualWork (Task) 字段。 |
| ActualOvertimeWork | `60` | 表示 ActualOvertimeWork (Task) 字段。 |
| OvertimeWork | `61` | 表示 OvertimeWork (Task) 字段。 |
| RegularWork | `62` | 表示 RegularWork (Task) 字段。 |
| RemainingDuration | `63` | 表示 RemainingDuration (Task) 字段。 |
| RemainingCost | `64` | 表示 RemainingCost (Task) 字段。 |
| RemainingWork | `65` | 表示 RemainingWork (Task) 字段。 |
| RemainingOvertimeWork | `66` | 表示 RemainingOvertimeWork (Task) 字段。 |
| RemainingOvertimeCost | `67` | 表示 RemainingOvertimeCost (Task) 字段。 |
| ACWP | `68` | 表示 ACWP (Task) 字段。 |
| CV | `69` | 表示 CV (Task) 字段。 |
| SV | `70` | 表示 SV (Task) 字段。 |
| ConstraintType | `71` | 表示 ConstraintType (Task) 字段。 |
| Calendar | `72` | 表示 Calendar (Task) 字段。 |
| ConstraintDate | `73` | 表示 ConstraintDate (Task) 字段。 |
| Deadline | `74` | 表示 Deadline (Task) 字段。 |
| LevelAssignments | `75` | 表示 LevelAssignments (Task) 字段。 |
| LevelingCanSplit | `76` | 表示 LevelingCanSplit (Task) 字段。 |
| LevelingDelay | `77` | 表示 LevelingDelay (Task) 字段。 |
| PreleveledStart | `78` | 表示 PreleveledStart (Task) 字段。 |
| PreleveledFinish | `79` | 表示 PreleveledFinish (Task) 字段。 |
| Hyperlink | `80` | 表示 Hyperlink (Task) 字段。 |
| HyperlinkAddress | `81` | 表示 HyperlinkAddress (Task) 字段。 |
| HyperlinkSubAddress | `82` | 表示 HyperlinkSubAddress (Task) 字段。 |
| IgnoreResourceCalendar | `83` | 表示 IgnoreResourceCalendar (Task) 字段。 |
| HideBar | `84` | 表示 HideBar (Task) 字段。 |
| IsRollup | `85` | 表示 IsRollup (Task) 字段。 |
| BCWS | `86` | 表示 BCWS (Task) 字段。 |
| BCWP | `87` | 表示 BCWP (Task) 字段。 |
| PhysicalPercentComplete | `88` | 表示 PhysicalPercentComplete (Task) 字段。 |
| EarnedValueMethod | `89` | 表示 EarnedValueMethod (Task) 字段。 |
| ActualWorkProtected | `90` | 表示 ActualWorkProtected (Task) 字段。 |
| ActualOvertimeWorkProtected | `91` | 表示 ActualOvertimeWorkProtected (Task) 字段。 |
| IsPublished | `92` | 表示 IsPublished (Task) 字段。 |
| IsScheduled | `93` | 表示 IsScheduled (Task) 字段。 |
| StatusManager | `94` | 表示 StatusManager (Task) 字段。 |
| CommitmentStart | `95` | 表示 CommitmentStart (Task) 字段。 |
| CommitmentFinish | `96` | 表示 CommitmentFinish (Task) 字段。 |
| CommitmentType | `97` | 表示 CommitmentType (Task) 字段。 |
| IsManual | `98` | 表示 IsManual (Task) 字段。 |
| IsExpanded | `99` | 表示 IsExpanded (Task) 字段。 |
| Guid | `100` | 表示 Guid (Task) 字段。 |
| NotesText | `101` | 表示 NotesText (Task) 字段。 |
| NotesRTF | `102` | 表示 NotesRTF (Task) 字段。 |
| ManualStart | `103` | 表示 ManualStart (Task) 字段。 |
| ManualFinish | `104` | 表示 ManualFinish (Task) 字段。 |
| ManualDuration | `105` | 表示 ManualDuration (Task) 字段。 |
| BudgetWork | `106` | 表示 BudgetWork (Task) 字段。 |
| BudgetCost | `107` | 表示 BudgetCost (Task) 字段。 |
| DisplayAsSummary | `108` | 表示 DisplayAsSummary (Task) 字段。 |
| SummaryProgress | `109` | 表示 Summary Progress (Task) 字段。 |
| IsActive | `110` | 表示 IsActive (Task) 字段。 |
| StartText | `111` | 表示 StartText (Task) 字段。 |
| FinishText | `112` | 表示 FinishText (Task) 字段。 |
| DurationText | `113` | 表示 DurationText (Task) 字段。 |
| CalendarUid | `114` | 表示 CalendarUid (Task) 字段。 |
| ParentTaskUid | `115` | 表示 ParentTaskUid (Task) 字段。 |
| DisplayOnTimeline | `116` | 表示 DisplayOnTimeline (Task) 字段。 |
| TaskIsAssigned | `117` | 表示 TaskIsAssigned (Task) 字段。 |
| TaskOriginalStart | `118` | 表示 原始开始 (Task) 字段。 |
| TaskOriginalFinish | `119` | 表示 原始完成 (Task) 字段。 |
| IsShowBeforeProjectStartDateWarning | `120` | 表示 使 MSP 显示警告的标志，任务在项目开始日期之前开始。 |
| Warning | `121` | 表示 指示任务存在计划差异的标志。 |
| ParentTaskGuid | `122` | 表示 ParentTaskGuid (Task) 字段。 |
| ActivityId | `123` | 表示 ActivityId 字段（仅适用于 Primavera 项目）。 |
| FreeSlackTimeSpan | `124` | 表示 FreeSlack（Task）字段。 |
| TotalSlackTimeSpan | `125` | 表示 TotalSlack（Task）字段。 |
| StartSlackTimeSpan | `126` | 表示 StartSlack（Task）字段。 |
| FinishSlackTimeSpan | `127` | 表示 FinishSlack（Task）字段。 |
| ExternalUid | `128` | 表示 外部任务的唯一标识。 |

## 示例

展示如何读取/写入任务属性。

```csharp
var project = new Project();

// 添加任务并设置任务属性
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 遍历所有收集的任务
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


