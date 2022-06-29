---
title: TaskKey
second_title: Aspose.Tasks for .NET API 参考
description: 表示支持的任务字段列表
type: docs
weight: 2100
url: /zh/net/aspose.tasks/taskkey/
---
## TaskKey enumeration

表示支持的任务字段列表。

```csharp
public enum TaskKey
```

### 价值观

| 姓名 | 价值 | 描述 |
| --- | --- | --- |
| Uid | `0` | 表示Uid(Task) 字段。 |
| Id | `1` | 表示 Id（任务）字段。 |
| Name | `2` | 表示名称（任务）字段。 |
| Type | `3` | 表示类型（任务）字段。 |
| IsNull | `4` | 表示 IsNull（任务）字段。 |
| Created | `5` | 表示已创建（任务）字段。 |
| Contact | `6` | 表示联系人（任务）字段。 |
| WBS | `7` | 表示 WBS（任务）字段。 |
| WBSLevel | `8` | 表示 WBSLevel（任务）字段。 |
| OutlineNumber | `9` | 表示 OutlineNumber（任务）字段。 |
| OutlineLevel | `10` | 表示 OutlineLevel（任务）字段。 |
| Priority | `11` | 表示优先级（任务）字段。 |
| Start | `12` | 表示开始（任务）字段。 |
| Finish | `13` | 表示完成（任务）字段。 |
| Duration | `14` | 表示持续时间（任务）字段。 |
| DurationVariance | `15` | 表示 DurationVariance（任务）字段。 |
| DurationFormat | `16` | 表示 DurationFormat（任务）字段。 |
| Work | `17` | 表示工作（任务）字段。 |
| Stop | `18` | 表示停止（任务）字段。 |
| Resume | `19` | 表示 Resume (Task) 字段。 |
| IsResumeValid | `20` | 表示 IsResumeValid（任务）字段。 |
| IsEffortDriven | `21` | 表示 IsEffortDriven（任务）字段。 |
| IsRecurring | `22` | 表示 IsRecurring（任务）字段。 |
| IsOverallocated | `23` | 表示 IsOverallocated（任务）字段。 |
| HasOverallocatedResource | `24` | 表示 HasOverallocatedResource（任务）字段。 |
| IsEstimated | `25` | 表示 IsEstimated（任务）字段。 |
| IsMilestone | `26` | 表示 IsMilestone（任务）字段。 |
| IsCritical | `27` | 表示 IsCritical（任务）字段。 |
| IsSubproject | `28` | 表示 IsSubproject（任务）字段。 |
| IsSubprojectReadOnly | `29` | 表示 IsSubprojectReadOnly（任务）字段。 |
| IsMarked | `30` | 表示 IsMarked（任务）字段。 |
| IgnoreWarnings | `31` | 表示 IgnoreWarnings（任务）字段。 |
| SubprojectName | `32` | 表示 SubprojectName（任务）字段。 |
| IsExternalTask | `33` | 表示 IsExternalTask（任务）字段。 |
| IsSummary | `34` | 表示 IsSummary（任务）字段。 |
| ExternalTaskProject | `35` | 表示 ExternalTaskProject（任务）字段。 |
| ExternalId | `36` | 表示 ExternalId（任务）字段。 |
| ExternalKey | `37` | 表示 ExternalKey（任务）字段。 |
| EarlyStart | `38` | 表示 EarlyStart（任务）字段。 |
| EarlyFinish | `39` | 表示 EarlyFinish（任务）字段。 |
| LateStart | `40` | 表示 LateStart（任务）字段。 |
| LateFinish | `41` | 表示 LateFinish（任务）字段。 |
| StartVariance | `42` | 表示 StartVariance（任务）字段。 |
| FinishVariance | `43` | 表示 FinishVariance（任务）字段。 |
| WorkVariance | `44` | 表示 WorkVariance（任务）字段。 |
| CostVariance | `45` | 表示 CostVariance（任务）字段。 |
| FreeSlack | `46` | 表示 FreeSlack（任务）字段。 |
| TotalSlack | `47` | 表示 TotalSlack（任务）字段。 |
| StartSlack | `48` | 表示 StartSlack（任务）字段。 |
| FinishSlack | `49` | 表示 FinishSlack（任务）字段。 |
| FixedCost | `50` | 表示固定成本（任务）字段。 |
| FixedCostAccrual | `51` | 表示 FixedCostAccrual（任务）字段。 |
| PercentComplete | `52` | 表示百分比完成（任务）字段。 |
| PercentWorkComplete | `53` | 表示百分比工作完成（任务）字段。 |
| Cost | `54` | 表示成本（任务）字段。 |
| OvertimeCost | `55` | 表示 OvertimeCost（任务）字段。 |
| ActualStart | `56` | 表示 ActualStart（任务）字段。 |
| ActualFinish | `57` | 表示 ActualFinish（任务）字段。 |
| ActualDuration | `58` | 表示 ActualDuration（任务）字段。 |
| ActualCost | `59` | 表示实际成本（任务）字段。 |
| ActualOvertimeCost | `60` | 表示 ActualOvertimeCost（任务）字段。 |
| ActualWork | `61` | 表示 ActualWork（任务）字段。 |
| ActualOvertimeWork | `62` | 表示 ActualOvertimeWork（任务）字段。 |
| OvertimeWork | `63` | 表示 OvertimeWork（任务）字段。 |
| RegularWork | `64` | 表示RegularWork（任务）字段。 |
| RemainingDuration | `65` | 表示 RemainingDuration（任务）字段。 |
| RemainingCost | `66` | 表示剩余成本（任务）字段。 |
| RemainingWork | `67` | 表示 RemainingWork（任务）字段。 |
| RemainingOvertimeWork | `68` | 表示 RemainingOvertimeWork（任务）字段。 |
| RemainingOvertimeCost | `69` | 表示 RemainingOvertimeCost（任务）字段。 |
| ACWP | `70` | 表示 ACWP（任务）字段。 |
| CV | `71` | 表示 CV（任务）字段。 |
| SV | `72` | 表示 SV（任务）字段。 |
| ConstraintType | `73` | 表示 ConstraintType（任务）字段。 |
| Calendar | `74` | 表示日历（任务）字段。 |
| ConstraintDate | `75` | 表示 ConstraintDate（任务）字段。 |
| Deadline | `76` | 表示截止日期（任务）字段。 |
| LevelAssignments | `77` | 表示 LevelAssignments（任务）字段。 |
| LevelingCanSplit | `78` | 表示LevelingCanSplit（任务）字段。 |
| LevelingDelay | `79` | 表示LevelingDelay（任务）字段。 |
| LevelingDelayFormat | `80` | 表示LevelingDelayFormat（任务）字段。 |
| PreleveledStart | `81` | 表示 PreleveledStart（任务）字段。 |
| PreleveledFinish | `82` | 表示 PreleveledFinish（任务）字段。 |
| Hyperlink | `83` | 表示超链接（任务）字段。 |
| HyperlinkAddress | `84` | 表示超链接地址（任务）字段。 |
| HyperlinkSubAddress | `85` | 表示 HyperlinkSubAddress（任务）字段。 |
| IgnoreResourceCalendar | `86` | 表示 IgnoreResourceCalendar（任务）字段。 |
| HideBar | `87` | 表示 HideBar（任务）字段。 |
| IsRollup | `88` | 表示 IsRollup（任务）字段。 |
| BCWS | `89` | 表示 BCWS（任务）字段。 |
| BCWP | `90` | 表示 BCWP（任务）字段。 |
| PhysicalPercentComplete | `91` | 表示 PhysicalPercentComplete（任务）字段。 |
| EarnedValueMethod | `92` | 表示 EarnedValueMethod（任务）字段。 |
| ActualWorkProtected | `93` | 表示 ActualWorkProtected (Task) 字段。 |
| ActualOvertimeWorkProtected | `94` | 表示 ActualOvertimeWorkProtected（任务）字段。 |
| IsPublished | `95` | 表示 IsPublished（任务）字段。 |
| IsScheduled | `96` | 表示 IsScheduled（任务）字段。 |
| StatusManager | `97` | 表示 StatusManager（任务）字段。 |
| CommitmentStart | `98` | 表示 CommitmentStart（任务）字段。 |
| CommitmentFinish | `99` | 表示 CommitmentFinish（任务）字段。 |
| CommitmentType | `100` | 表示 CommitmentType（任务）字段。 |
| IsManual | `101` | 表示 IsManual（任务）字段。 |
| IsExpanded | `102` | 表示 IsExpanded（任务）字段。 |
| Guid | `103` | 表示 Guid（任务）字段。 |
| NotesText | `104` | 表示 NotesText（任务）字段。 |
| NotesRTF | `105` | 表示 NotesRTF（任务）字段。 |
| ManualStart | `106` | 表示 ManualStart（任务）字段。 |
| ManualFinish | `107` | 表示 ManualFinish（任务）字段。 |
| ManualDuration | `108` | 表示 ManualDuration（任务）字段。 |
| BudgetWork | `109` | 表示 BudgetWork（任务）字段。 |
| BudgetCost | `110` | 表示 BudgetCost（任务）字段。 |
| DisplayAsSummary | `111` | 表示 DisplayAsSummary（任务）字段。 |
| SummaryProgress | `112` | 表示摘要进度（任务）字段。 |
| IsActive | `113` | 表示 IsActive（任务）字段。 |
| StartText | `114` | 表示 StartText（任务）字段。 |
| FinishText | `115` | 表示 FinishText（任务）字段。 |
| DurationText | `116` | 表示 DurationText（任务）字段。 |
| CalendarUid | `117` | 表示 CalendarUid（任务）字段。 |
| ParentTaskUid | `118` | 表示 ParentTaskUid（任务）字段。 |
| DisplayOnTimeline | `119` | 表示 DisplayOnTimeline（任务）字段。 |
| TaskIsAssigned | `120` | 表示TaskIsAssigned（任务）字段。 |
| TaskOriginalStart | `121` | 表示原始开始（任务）字段。 |
| TaskOriginalFinish | `122` | 表示原始完成（任务）字段。 |
| IsShowBeforeProjectStartDateWarning | `123` | 表示使 MSP 显示任务在项目开始日期之前开始的警告的标志。 |
| Warning | `124` | 表示指示任务有调度差异的标志。 |
| ParentTaskGuid | `125` | 表示 ParentTaskGuid（任务）字段。 |
| ActivityId | `126` | 表示 ActivityId 字段（仅适用于 Primavera 项目）。 |
| FreeSlackTimeSpan | `127` | 表示 FreeSlack（任务）字段。 |
| TotalSlackTimeSpan | `128` | 表示 TotalSlack（任务）字段。 |
| StartSlackTimeSpan | `129` | 表示 StartSlack（任务）字段。 |
| FinishSlackTimeSpan | `130` | 表示 FinishSlack（任务）字段。 |

### 也可以看看

* 命名空间 [Aspose.Tasks](../../aspose.tasks)
* 部件 [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
