---
title: Tsk
second_title: Aspose.Tasks for .NET API 参考
description: 表示属性Task./task对象.
type: docs
weight: 2290
url: /zh/net/aspose.tasks/tsk/
---
## Tsk class

表示属性[`Task`](../task)对象.

```csharp
public static class Tsk
```

## 字段

| 姓名 | 描述 |
| --- | --- |
| static readonly [ActivityId](../../aspose.tasks/tsk/activityid) | 表示活动 ID 字段 - Primavera 使用的任务的唯一标识符。 （仅适用于 Primavera 项目）. |
| static readonly [ActualCost](../../aspose.tasks/tsk/actualcost) | 资源已在其任务上执行的工作所产生的成本，以及与该任务相关的任何其他记录成本。 |
| static readonly [ActualDuration](../../aspose.tasks/tsk/actualduration) | 任务的实际工作时间跨度，基于计划的持续时间和当前剩余工时或完成百分比。 |
| static readonly [ActualFinish](../../aspose.tasks/tsk/actualfinish) | 任务完成的日期。 |
| static readonly [ActualOvertimeCost](../../aspose.tasks/tsk/actualovertimecost) | 已分配资源对任务执行的加班工作产生的成本。 |
| static readonly [ActualOvertimeWork](../../aspose.tasks/tsk/actualovertimework) | 分配给任务的资源已经执行的实际加班工作量。 |
| static readonly [ActualOvertimeWorkProtected](../../aspose.tasks/tsk/actualovertimeworkprotected) | 保护实际加班工作的持续时间。 仅支持 XML 格式的读取。 [`Duration`](./duration)类型. |
| static readonly [ActualStart](../../aspose.tasks/tsk/actualstart) | 任务实际开始的日期和时间。 |
| static readonly [ActualWork](../../aspose.tasks/tsk/actualwork) | 分配给任务的资源已经完成的工作量。 |
| static readonly [ActualWorkProtected](../../aspose.tasks/tsk/actualworkprotected) | 实际工作受到保护的持续时间。 仅支持 XML 格式的读取。 [`Duration`](./duration)类型. |
| static readonly [ACWP](../../aspose.tasks/tsk/acwp) | 截止到项目状态日期或今天日期，已完成任务的工作所产生的成本。 |
| static readonly [BCWP](../../aspose.tasks/tsk/bcwp) | 任务完成百分比的累积值乘以时间分段基准成本。 |
| static readonly [BCWS](../../aspose.tasks/tsk/bcws) | 截至状态日期或今天日期的累计时间分段基准成本。 |
| static readonly [BudgetCost](../../aspose.tasks/tsk/budgetcost) | 预算成本资源的预算成本。预算资源仅分配给项目摘要任务。 |
| static readonly [BudgetWork](../../aspose.tasks/tsk/budgetwork) | 预算工作和材料资源的预算工作。预算资源仅分配给项目摘要任务。 |
| static readonly [Calendar](../../aspose.tasks/tsk/calendar) | 任务日历. |
| static readonly [CommitmentFinish](../../aspose.tasks/tsk/commitmentfinish) | 交货的完成日期。  仅支持 XML 格式的读取。 DateTime类型。 |
| static readonly [CommitmentStart](../../aspose.tasks/tsk/commitmentstart) | 交货的开始日期。  仅支持 XML 格式的读取。 DateTime类型。 |
| static readonly [CommitmentType](../../aspose.tasks/tsk/commitmenttype) | 确定任务是否具有关联的交付或 对关联交付的依赖关系。  仅支持 XML 格式的读取。 Int32类型. |
| static readonly [ConstraintDate](../../aspose.tasks/tsk/constraintdate) | 与约束类型关联的具体日期。 |
| static readonly [ConstraintType](../../aspose.tasks/tsk/constrainttype) | 提供可用于调度任务的约束类型的选择。 |
| static readonly [Contact](../../aspose.tasks/tsk/contact) | 负责某项任务的个人的姓名。 |
| static readonly [Cost](../../aspose.tasks/tsk/cost) | 除剩余工时的计划成本外，任务的计划或预计总成本基于分配给任务的资源执行的工时已产生的成本。 |
| static readonly [CostVariance](../../aspose.tasks/tsk/costvariance) | 任务、资源或工作分配的基准成本与总成本之间的差异。 |
| static readonly [Created](../../aspose.tasks/tsk/created) | 创建任务的日期。 |
| static readonly [CV](../../aspose.tasks/tsk/cv) | 任务的基准成本和总成本之间的差异。 成本差异 = 成本 - 基准成本 |
| static readonly [Deadline](../../aspose.tasks/tsk/deadline) | 指示任务何时完成的目标日期。 |
| static readonly [DisplayAsSummary](../../aspose.tasks/tsk/displayassummary) | 确定任务是否应显示为摘要任务。  仅支持 XML 格式的读取。 Boolean类型。 |
| static readonly [DisplayOnTimeline](../../aspose.tasks/tsk/displayontimeline) | 指定是否应在时间线视图上显示任务。 |
| static readonly [Duration](../../aspose.tasks/tsk/duration) | 根据开始日期、完成日期、日历和其他计划因素输入或由 Microsoft Project 计算的任务的活动工作时间的总跨度。 |
| static readonly [DurationFormat](../../aspose.tasks/tsk/durationformat) | 任务持续时间格式. |
| static readonly [DurationText](../../aspose.tasks/tsk/durationtext) | 返回任务的持续时间文本。 |
| static readonly [DurationVariance](../../aspose.tasks/tsk/durationvariance) | 任务的基线持续时间与任务的总持续时间（当前估计）之间的差异。 |
| static readonly [EarlyFinish](../../aspose.tasks/tsk/earlyfinish) | 任务可能完成的最早日期，基于前任和后续任务的提前完成日期、其他限制和任何升级延迟。 |
| static readonly [EarlyStart](../../aspose.tasks/tsk/earlystart) | 任务可能开始的最早日期，基于前任和后继任务的最早开始日期和其他限制。 |
| static readonly [EarnedValueMethod](../../aspose.tasks/tsk/earnedvaluemethod) | 确定应使用完成百分比还是物理完成百分比字段来计算已完成工作的预算成本 (BCWP)。 |
| static readonly [ExternalId](../../aspose.tasks/tsk/externalid) | 如果任务是外部任务，则它包含任务的外部 ID。 |
| static readonly [ExternalTaskProject](../../aspose.tasks/tsk/externaltaskproject) | 外部任务的源位置和任务标识符。 |
| static readonly [Finish](../../aspose.tasks/tsk/finish) | 任务的预定完成日期。 |
| static readonly [FinishSlackTimeSpan](../../aspose.tasks/tsk/finishslacktimespan) | 提前完成日期和延迟完成日期之间的持续时间。 |
| static readonly [FinishText](../../aspose.tasks/tsk/finishtext) | 返回任务的完成文本。 |
| static readonly [FinishVariance](../../aspose.tasks/tsk/finishvariance) | 表示任务或分配的基线完成日期与其当前完成日期之间的差异的时间。 |
| static readonly [FixedCost](../../aspose.tasks/tsk/fixedcost) | 显示任何非资源任务费用。 |
| static readonly [FixedCostAccrual](../../aspose.tasks/tsk/fixedcostaccrual) | 确定如何以及何时将固定成本计入或应计到任务成本中的选择。 |
| static readonly [FreeSlackTimeSpan](../../aspose.tasks/tsk/freeslacktimespan) | 可以延迟任务而不延迟任何后续任务的时间。 |
| static readonly [Guid](../../aspose.tasks/tsk/guid) | 为任务生成的唯一标识码。 |
| static readonly [HasOverallocatedResource](../../aspose.tasks/tsk/hasoverallocatedresource) | 指示任务是否分配了资源，该资源在分配的任务上的工作量超过了正常工作能力内所能完成的工作量。 |
| static readonly [HideBar](../../aspose.tasks/tsk/hidebar) | 确定任务的甘特条在 Microsoft Project 中显示时是否隐藏。 |
| static readonly [Hyperlink](../../aspose.tasks/tsk/hyperlink) | 与任务关联的超链接的标题或说明性文本。 |
| static readonly [HyperlinkAddress](../../aspose.tasks/tsk/hyperlinkaddress) | 与任务关联的超链接的地址。 |
| static readonly [HyperlinkSubAddress](../../aspose.tasks/tsk/hyperlinksubaddress) | 文档中与任务关联的超链接中的特定位置。 |
| static readonly [Id](../../aspose.tasks/tsk/id) | 任务列表中任务的位置标识符。 |
| static readonly [IgnoreResourceCalendar](../../aspose.tasks/tsk/ignoreresourcecalendar) | 确定任务的调度是否考虑分配给任务的资源的日历。 |
| static readonly [IgnoreWarnings](../../aspose.tasks/tsk/ignorewarnings) | 表示是否在 Microsoft Project 中隐藏计划冲突警告指示器。 |
| static readonly [IsActive](../../aspose.tasks/tsk/isactive) | 确定任务是否处于活动状态。非活动任务不再影响其他任务或整个项目计划。 |
| static readonly [IsCritical](../../aspose.tasks/tsk/iscritical) | 确定任务是否在关键路径上。 |
| static readonly [IsEffortDriven](../../aspose.tasks/tsk/iseffortdriven) | 确定任务的计划是否为投入驱动计划。 |
| static readonly [IsEstimated](../../aspose.tasks/tsk/isestimated) | 确定是否估计任务。 |
| static readonly [IsExpanded](../../aspose.tasks/tsk/isexpanded) | 确定摘要任务是否在甘特图视图中展开。 |
| static readonly [IsExternalTask](../../aspose.tasks/tsk/isexternaltask) | 确定任务是否是外部的。 |
| static readonly [IsManual](../../aspose.tasks/tsk/ismanual) | 判断任务是否手动调度。 |
| static readonly [IsMarked](../../aspose.tasks/tsk/ismarked) | 显示任务是否被标记为进一步行动或某种识别。 |
| static readonly [IsMilestone](../../aspose.tasks/tsk/ismilestone) | 确定任务是否为里程碑。 |
| static readonly [IsNull](../../aspose.tasks/tsk/isnull) | 判断一个任务是否为空任务。 |
| static readonly [IsOverallocated](../../aspose.tasks/tsk/isoverallocated) | 指示任务上的任何已分配资源是否被分配给该任务的工作量超过了正常工作能力所能完成的工作量。 |
| static readonly [IsPublished](../../aspose.tasks/tsk/ispublished) | 确定当前任务是否应与项目的其余部分一起发布到 Project Server。 |
| static readonly [IsRecurring](../../aspose.tasks/tsk/isrecurring) | 确定一个任务是否是一系列重复任务的一部分。 |
| static readonly [IsResumeValid](../../aspose.tasks/tsk/isresumevalid) | 确定任务是否可以恢复。 |
| static readonly [IsRollup](../../aspose.tasks/tsk/isrollup) | 确定是否将有关子任务甘特条的信息汇总到摘要任务栏。 |
| static readonly [IsSubproject](../../aspose.tasks/tsk/issubproject) | 判断任务是否为插入项目。 |
| static readonly [IsSubprojectReadOnly](../../aspose.tasks/tsk/issubprojectreadonly) | 确定子项目是否为只读。 |
| static readonly [IsSummary](../../aspose.tasks/tsk/issummary) | 确定任务是否为摘要任务。 |
| static readonly [LateFinish](../../aspose.tasks/tsk/latefinish) | 任务可以在不延迟项目完成的情况下完成的最晚日期。 |
| static readonly [LateStart](../../aspose.tasks/tsk/latestart) | 任务可以在不延迟项目完成的情况下开始的最晚日期。 |
| static readonly [LevelAssignments](../../aspose.tasks/tsk/levelassignments) | 确定调配功能是否可以延迟和拆分单个分配以解决过度分配问题。 |
| static readonly [LevelingCanSplit](../../aspose.tasks/tsk/levelingcansplit) | 确定资源调配功能是否会导致拆分此任务的剩余工作。 |
| static readonly [LevelingDelay](../../aspose.tasks/tsk/levelingdelay) | 由于资源平衡，任务从其早期开始日期延迟的时间。 |
| static readonly [LevelingDelayFormat](../../aspose.tasks/tsk/levelingdelayformat) | 表示延迟持续时间的格式。 |
| static readonly [ManualDuration](../../aspose.tasks/tsk/manualduration) | 定义手动计划的任务持续时间。 |
| static readonly [ManualFinish](../../aspose.tasks/tsk/manualfinish) | 定义任务的手动计划完成时间。 |
| static readonly [ManualStart](../../aspose.tasks/tsk/manualstart) | 定义手动计划的任务开始。 |
| static readonly [Name](../../aspose.tasks/tsk/name) | 任务的名称。 |
| static readonly [NotesRTF](../../aspose.tasks/tsk/notesrtf) | RTF 格式的文字注释。 |
| static readonly [NotesText](../../aspose.tasks/tsk/notestext) | 从 RTF 数据中提取的 Notes 纯文本。 |
| static readonly [OutlineLevel](../../aspose.tasks/tsk/outlinelevel) | 任务的大纲级别。 |
| static readonly [OutlineNumber](../../aspose.tasks/tsk/outlinenumber) | 代表任务在分层大纲结构中的位置的数字。 |
| static readonly [OvertimeCost](../../aspose.tasks/tsk/overtimecost) | 任务、所有已分配任务的资源或资源分配的总加班成本。 |
| static readonly [OvertimeWork](../../aspose.tasks/tsk/overtimework) | 分配给任务的所有资源计划执行的加班量。 |
| static readonly [PercentComplete](../../aspose.tasks/tsk/percentcomplete) | 任务的当前状态，表示为已完成任务持续时间的百分比。 |
| static readonly [PercentWorkComplete](../../aspose.tasks/tsk/percentworkcomplete) | 任务的当前状态，表示为已完成工作的百分比。 |
| static readonly [PhysicalPercentComplete](../../aspose.tasks/tsk/physicalpercentcomplete) | 可用作计算已完成工作的预算成本 (BCWP) 的替代方法的完成百分比值。 |
| static readonly [PreleveledFinish](../../aspose.tasks/tsk/preleveledfinish) | 资源调配完成前任务的完成日期。 |
| static readonly [PreleveledStart](../../aspose.tasks/tsk/preleveledstart) | 资源调配完成之前的任务开始日期。 |
| static readonly [Priority](../../aspose.tasks/tsk/priority) | 赋予任务的重要性级别，这反过来表示在资源调配期间任务或分配可以延迟或拆分的难易程度。 |
| static readonly [RegularWork](../../aspose.tasks/tsk/regularwork) | 资源计划执行的非加班工作总量。 |
| static readonly [RemainingCost](../../aspose.tasks/tsk/remainingcost) | 完成剩余预定工作将产生的剩余预定费用。 |
| static readonly [RemainingDuration](../../aspose.tasks/tsk/remainingduration) | 完成任务未完成部分所需的时间。 |
| static readonly [RemainingOvertimeCost](../../aspose.tasks/tsk/remainingovertimecost) | 任务的剩余计划加班费用。 |
| static readonly [RemainingOvertimeWork](../../aspose.tasks/tsk/remainingovertimework) | 剩余计划加班时间。 |
| static readonly [RemainingWork](../../aspose.tasks/tsk/remainingwork) | 完成一项或一组任务所需的时间。 |
| static readonly [Resume](../../aspose.tasks/tsk/resume) | 任务的剩余部分计划在输入任何进度后恢复的日期。 |
| static readonly [Start](../../aspose.tasks/tsk/start) | 任务的计划开始日期。 |
| static readonly [StartSlackTimeSpan](../../aspose.tasks/tsk/startslacktimespan) | 提前开始日期和延迟开始日期之间的持续时间。 |
| static readonly [StartText](../../aspose.tasks/tsk/starttext) | 返回任务的开始文本。 |
| static readonly [StartVariance](../../aspose.tasks/tsk/startvariance) | 表示任务或分配的基线开始日期与其当前计划开始日期之间的差异的时间。 |
| static readonly [StatusManager](../../aspose.tasks/tsk/statusmanager) | 将从资源接收当前任务状态更新的企业资源的名称。 |
| static readonly [Stop](../../aspose.tasks/tsk/stop) | 表示任务实际部分结束的日期。 |
| static readonly [SubprojectName](../../aspose.tasks/tsk/subprojectname) | 子项目的源位置。 |
| static readonly [SV](../../aspose.tasks/tsk/sv) | 挣值进度差异，通过项目状态日期。 进度差异 (SV) 是 BCWP 和 BCWS 之间的差异。 |
| static readonly [TotalSlackTimeSpan](../../aspose.tasks/tsk/totalslacktimespan) | 可以延迟任务的完成日期而不延迟项目的完成日期的时间。 |
| static readonly [Type](../../aspose.tasks/tsk/type) | 任务的类型。 |
| static readonly [Uid](../../aspose.tasks/tsk/uid) | 任务的唯一 ID。 |
| static readonly [Warning](../../aspose.tasks/tsk/warning) | 表示指示任务有调度差异的标志。 |
| static readonly [WBS](../../aspose.tasks/tsk/wbs) | 工作分解结构 (WBS) 代码。 |
| static readonly [WBSLevel](../../aspose.tasks/tsk/wbslevel) | 任务最右侧的 WBS 级别。 |
| static readonly [Work](../../aspose.tasks/tsk/work) | 为所有分配的资源安排任务的总时间。 |
| static readonly [WorkVariance](../../aspose.tasks/tsk/workvariance) | 任务的基线工时与当前计划工时之间的差异。 |

### 也可以看看

* 命名空间 [Aspose.Tasks](../../aspose.tasks)
* 部件 [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
