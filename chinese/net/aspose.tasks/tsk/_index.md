---
title: Class Tsk
second_title: Aspose.Tasks for .NET API 参考
description: Aspose.Tasks.Tsk 班级. 代表属性Task对象.
type: docs
weight: 2310
url: /zh/net/aspose.tasks/tsk/
---
## Tsk class

代表属性[`Task`](../task/)对象.

```csharp
public static class Tsk
```

## 字段

| 姓名 | 描述 |
| --- | --- |
| static readonly [ActivityId](../../aspose.tasks/tsk/activityid/) | 表示活动 ID 字段 - Primavera 使用的任务的唯一标识符。 （仅适用于 Primavera 项目）. |
| static readonly [ActualCost](../../aspose.tasks/tsk/actualcost/) | 资源已在其任务中执行的工时所产生的成本，以及与该任务相关的任何其他已记录成本。 |
| static readonly [ActualDuration](../../aspose.tasks/tsk/actualduration/) | 任务的实际工作时间跨度，基于计划持续时间和当前剩余工时或完成百分比。 |
| static readonly [ActualFinish](../../aspose.tasks/tsk/actualfinish/) | 任务完成的日期。 |
| static readonly [ActualOvertimeCost](../../aspose.tasks/tsk/actualovertimecost/) | 已分配资源对任务执行的加班工作产生的成本。 |
| static readonly [ActualOvertimeWork](../../aspose.tasks/tsk/actualovertimework/) | 分配给任务的资源已执行的实际加班工时量。 |
| static readonly [ActualOvertimeWorkProtected](../../aspose.tasks/tsk/actualovertimeworkprotected/) | 实际加班工作受到保护的持续时间。 |
| static readonly [ActualStart](../../aspose.tasks/tsk/actualstart/) | 任务实际开始的日期和时间。 |
| static readonly [ActualWork](../../aspose.tasks/tsk/actualwork/) | 分配给任务的资源已经完成的工作量。 |
| static readonly [ActualWorkProtected](../../aspose.tasks/tsk/actualworkprotected/) | 实际工作受到保护的持续时间。 仅支持 XML 格式的读取。 |
| static readonly [ACWP](../../aspose.tasks/tsk/acwp/) | 截至项目状态日期或今天的日期，已完成任务的工时所产生的成本。 |
| static readonly [BCWP](../../aspose.tasks/tsk/bcwp/) | 任务完成百分比乘以时间分段基准成本的累积值。 |
| static readonly [BCWS](../../aspose.tasks/tsk/bcws/) | 截至状态日期或今天日期的累计时间分段基准成本。 |
| static readonly [BudgetCost](../../aspose.tasks/tsk/budgetcost/) | 预算成本资源的预算成本。预算资源仅分配给项目摘要任务。 |
| static readonly [BudgetWork](../../aspose.tasks/tsk/budgetwork/) | 预算工作和物质资源的预算工作。预算资源仅分配给项目摘要任务。 |
| static readonly [Calendar](../../aspose.tasks/tsk/calendar/) | 任务日历。 |
| static readonly [CommitmentFinish](../../aspose.tasks/tsk/commitmentfinish/) | 交货的完成日期。  仅支持 XML 格式的读取。 |
| static readonly [CommitmentStart](../../aspose.tasks/tsk/commitmentstart/) | 交货的开始日期。 仅支持 XML 格式的读取。 |
| static readonly [CommitmentType](../../aspose.tasks/tsk/commitmenttype/) | 确定任务是否具有关联的交付或 对关联交付的依赖性。 仅支持 XML 格式的读取。 |
| static readonly [ConstraintDate](../../aspose.tasks/tsk/constraintdate/) | 与约束类型关联的具体日期。 |
| static readonly [ConstraintType](../../aspose.tasks/tsk/constrainttype/) | 提供可用于调度任务的约束类型的选择。 |
| static readonly [Contact](../../aspose.tasks/tsk/contact/) | 任务负责人的姓名。 |
| static readonly [Cost](../../aspose.tasks/tsk/cost/) | 任务的计划或预计总成本，该成本基于分配给任务的资源所执行的工作已经产生的成本，以及剩余工作的计划成本。 |
| static readonly [CostVariance](../../aspose.tasks/tsk/costvariance/) | 任务、资源或分配的比较基准成本与总成本之间的差异。 |
| static readonly [Created](../../aspose.tasks/tsk/created/) | 创建任务的日期。 |
| static readonly [CV](../../aspose.tasks/tsk/cv/) | 任务的基准成本与总成本之间的差异。 成本差异 = 成本 - 基准成本 |
| static readonly [Deadline](../../aspose.tasks/tsk/deadline/) | 指示任务何时完成的目标日期。 |
| static readonly [DisplayAsSummary](../../aspose.tasks/tsk/displayassummary/) | 确定任务是否应显示为摘要任务。 仅支持 XML 格式的读取。 |
| static readonly [DisplayOnTimeline](../../aspose.tasks/tsk/displayontimeline/) | 指定任务是否应显示在时间线视图上。 |
| static readonly [Duration](../../aspose.tasks/tsk/duration/) | Microsoft Project 根据开始日期、结束日期、日历和其他计划因素输入或计算的任务活动工作时间的总跨度。 |
| static readonly [DurationFormat](../../aspose.tasks/tsk/durationformat/) | 任务持续时间格式。 |
| static readonly [DurationText](../../aspose.tasks/tsk/durationtext/) | 返回任务的持续时间文本。 |
| static readonly [DurationVariance](../../aspose.tasks/tsk/durationvariance/) | 任务的基线持续时间与任务的总持续时间（当前估计）之间的差异。 |
| static readonly [EarlyFinish](../../aspose.tasks/tsk/earlyfinish/) | 任务可能完成的最早日期，基于前置任务和后续任务的最早完成日期、其他约束以及任何调平延迟。 |
| static readonly [EarlyStart](../../aspose.tasks/tsk/earlystart/) | 任务可能开始的最早日期，基于前置任务和后续任务的最早开始日期以及其他约束条件。 |
| static readonly [EarnedValueMethod](../../aspose.tasks/tsk/earnedvaluemethod/) | 确定是否应该使用“完成百分比”或“物理完成百分比”字段来计算已执行工作的预算成本 (BCWP)。 |
| static readonly [ExternalId](../../aspose.tasks/tsk/externalid/) | 如果任务是外部任务，它包含任务的外部 Id. |
| static readonly [ExternalTaskProject](../../aspose.tasks/tsk/externaltaskproject/) | 外部任务的源位置和任务标识符。 |
| static readonly [ExternalUid](../../aspose.tasks/tsk/externaluid/) | 当任务是外部时包含外部任务的唯一标识符。 |
| static readonly [Finish](../../aspose.tasks/tsk/finish/) | 任务的预定完成日期。 |
| static readonly [FinishSlackTimeSpan](../../aspose.tasks/tsk/finishslacktimespan/) | 最早完成日期和最晚完成日期之间的持续时间。 |
| static readonly [FinishText](../../aspose.tasks/tsk/finishtext/) | 返回任务的完成文本。 |
| static readonly [FinishVariance](../../aspose.tasks/tsk/finishvariance/) | 表示任务或分配的比较基准完成日期与其当前完成日期之间的差异的时间。 |
| static readonly [FixedCost](../../aspose.tasks/tsk/fixedcost/) | 显示任何非资源任务费用。 |
| static readonly [FixedCostAccrual](../../aspose.tasks/tsk/fixedcostaccrual/) | 确定如何以及何时将固定成本计入或计入任务成本的选择。 |
| static readonly [FreeSlackTimeSpan](../../aspose.tasks/tsk/freeslacktimespan/) | 在不延迟任何后续任务的情况下可以延迟任务的时间。 |
| static readonly [Guid](../../aspose.tasks/tsk/guid/) | 为任务生成的唯一标识码。 |
| static readonly [HasOverallocatedResource](../../aspose.tasks/tsk/hasoverallocatedresource/) | 指示任务是否分配了资源，该资源在分配的任务上的工作量超过正常工作能力内可以完成的工作量。 |
| static readonly [HideBar](../../aspose.tasks/tsk/hidebar/) | 确定任务的甘特图在 Microsoft Project 中显示时是否隐藏。 |
| static readonly [Hyperlink](../../aspose.tasks/tsk/hyperlink/) | 与任务关联的超链接的标题或解释性文本。 |
| static readonly [HyperlinkAddress](../../aspose.tasks/tsk/hyperlinkaddress/) | 与任务关联的超链接地址。 |
| static readonly [HyperlinkSubAddress](../../aspose.tasks/tsk/hyperlinksubaddress/) | 与任务关联的超链接中文档中的特定位置。 |
| static readonly [Id](../../aspose.tasks/tsk/id/) | 任务列表中任务的位置标识符。 |
| static readonly [IgnoreResourceCalendar](../../aspose.tasks/tsk/ignoreresourcecalendar/) | 确定任务的计划是否考虑分配给任务的资源的日历。 |
| static readonly [IgnoreWarnings](../../aspose.tasks/tsk/ignorewarnings/) | 指示是否在 Microsoft Project 中隐藏日程冲突警告指示器。 |
| static readonly [IsActive](../../aspose.tasks/tsk/isactive/) | 确定任务是否处于活动状态。非活动任务不再影响其他任务或整个项目进度。 |
| static readonly [IsCritical](../../aspose.tasks/tsk/iscritical/) | 确定任务是否在关键路径上。 |
| static readonly [IsEffortDriven](../../aspose.tasks/tsk/iseffortdriven/) | 确定任务的调度是否为投入比驱动的调度。 |
| static readonly [IsEstimated](../../aspose.tasks/tsk/isestimated/) | 判断一个任务是否被估计。 |
| static readonly [IsExpanded](../../aspose.tasks/tsk/isexpanded/) | 确定摘要任务是否在甘特图视图中展开。 |
| static readonly [IsExternalTask](../../aspose.tasks/tsk/isexternaltask/) | 判断一个任务是否是外部的。 |
| static readonly [IsManual](../../aspose.tasks/tsk/ismanual/) | 判断任务是否手动调度。 |
| static readonly [IsMarked](../../aspose.tasks/tsk/ismarked/) | 显示任务是否标记为进一步操作或某种标识。 |
| static readonly [IsMilestone](../../aspose.tasks/tsk/ismilestone/) | 确定任务是否为里程碑。 |
| static readonly [IsNull](../../aspose.tasks/tsk/isnull/) | 判断任务是否为空任务。 |
| static readonly [IsOverallocated](../../aspose.tasks/tsk/isoverallocated/) | 表示任务上分配的任何资源是否分配给了比正常工作能力所能完成的工作更多的工作。 |
| static readonly [IsPublished](../../aspose.tasks/tsk/ispublished/) | 确定当前任务是否应与项目的其余部分一起发布到 Project Server。 |
| static readonly [IsRecurring](../../aspose.tasks/tsk/isrecurring/) | 确定任务是否是一系列重复任务的一部分。 |
| static readonly [IsResumeValid](../../aspose.tasks/tsk/isresumevalid/) | 确定任务是否可以恢复。 |
| static readonly [IsRollup](../../aspose.tasks/tsk/isrollup/) | 确定有关子任务甘特图条的信息是否将汇总到摘要任务栏。 |
| static readonly [IsSubproject](../../aspose.tasks/tsk/issubproject/) | 判断任务是否为插入项目。 |
| static readonly [IsSubprojectReadOnly](../../aspose.tasks/tsk/issubprojectreadonly/) | 确定子项目是否为只读。 |
| static readonly [IsSummary](../../aspose.tasks/tsk/issummary/) | 判断任务是否为摘要任务。 |
| static readonly [LateFinish](../../aspose.tasks/tsk/latefinish/) | 任务可以在不延迟项目完成的情况下完成的最晚日期。 |
| static readonly [LateStart](../../aspose.tasks/tsk/latestart/) | 任务可以开始而不延迟项目完成的最晚日期。 |
| static readonly [LevelAssignments](../../aspose.tasks/tsk/levelassignments/) | 确定均衡功能是否可以延迟和拆分单个分配以解决过度分配问题。 |
| static readonly [LevelingCanSplit](../../aspose.tasks/tsk/levelingcansplit/) | 确定资源平衡功能是否会导致拆分此任务的剩余工作。 |
| static readonly [LevelingDelay](../../aspose.tasks/tsk/levelingdelay/) | 由于资源平衡，任务从其最早开始日期延迟的时间。 |
| static readonly [LevelingDelayFormat](../../aspose.tasks/tsk/levelingdelayformat/) | 延迟持续时间的表示格式。 |
| static readonly [ManualDuration](../../aspose.tasks/tsk/manualduration/) | 定义任务的手动计划持续时间。 |
| static readonly [ManualFinish](../../aspose.tasks/tsk/manualfinish/) | 定义任务的手动计划完成。 |
| static readonly [ManualStart](../../aspose.tasks/tsk/manualstart/) | 定义任务的手动计划开始。 |
| static readonly [Name](../../aspose.tasks/tsk/name/) | 任务名称. |
| static readonly [NotesRTF](../../aspose.tasks/tsk/notesrtf/) | RTF 格式的文本注释。 |
| static readonly [NotesText](../../aspose.tasks/tsk/notestext/) | 从 RTF 数据中提取的笔记的纯文本。 |
| static readonly [OutlineLevel](../../aspose.tasks/tsk/outlinelevel/) | 任务的大纲级别。 |
| static readonly [OutlineNumber](../../aspose.tasks/tsk/outlinenumber/) | 表示任务在层次结构中的位置的数字。 |
| static readonly [OvertimeCost](../../aspose.tasks/tsk/overtimecost/) | 任务、所有已分配任务的资源或资源分配的总加班成本。 |
| static readonly [OvertimeWork](../../aspose.tasks/tsk/overtimework/) | 分配给任务的所有资源计划执行的加班量。 |
| static readonly [PercentComplete](../../aspose.tasks/tsk/percentcomplete/) | 任务的当前状态，表示为已完成的任务持续时间的百分比。 |
| static readonly [PercentWorkComplete](../../aspose.tasks/tsk/percentworkcomplete/) | 任务的当前状态，表示为已完成工作的百分比。 |
| static readonly [PhysicalPercentComplete](../../aspose.tasks/tsk/physicalpercentcomplete/) | 可用作计算已执行工作的预算成本 (BCWP) 的替代值的百分比值。 |
| static readonly [PreleveledFinish](../../aspose.tasks/tsk/preleveledfinish/) | 完成资源平衡之前任务的完成日期。 |
| static readonly [PreleveledStart](../../aspose.tasks/tsk/preleveledstart/) | 完成资源平衡之前的任务开始日期。 |
| static readonly [Priority](../../aspose.tasks/tsk/priority/) | 赋予任务的重要性级别，这反过来表明在资源平衡期间任务或分配可以延迟或拆分的容易程度。 |
| static readonly [RegularWork](../../aspose.tasks/tsk/regularwork/) | 计划由资源执行的非加班工时总量。 |
| static readonly [RemainingCost](../../aspose.tasks/tsk/remainingcost/) | 完成剩余计划工时将产生的剩余计划费用。 |
| static readonly [RemainingDuration](../../aspose.tasks/tsk/remainingduration/) | 完成任务未完成部分所需的时间。 |
| static readonly [RemainingOvertimeCost](../../aspose.tasks/tsk/remainingovertimecost/) | 任务的剩余计划加班费用。 |
| static readonly [RemainingOvertimeWork](../../aspose.tasks/tsk/remainingovertimework/) | 剩余计划加班时间。 |
| static readonly [RemainingWork](../../aspose.tasks/tsk/remainingwork/) | 完成一个任务或一组任务还需要的时间。 |
| static readonly [Resume](../../aspose.tasks/tsk/resume/) | 在输入任何进度后任务的剩余部分计划恢复的日期。 |
| static readonly [Start](../../aspose.tasks/tsk/start/) | 任务的预定开始日期。 |
| static readonly [StartSlackTimeSpan](../../aspose.tasks/tsk/startslacktimespan/) | 最早开始日期和最晚开始日期之间的持续时间。 |
| static readonly [StartText](../../aspose.tasks/tsk/starttext/) | 返回任务的开始文本。 |
| static readonly [StartVariance](../../aspose.tasks/tsk/startvariance/) | 表示任务或分配的基线开始日期与其当前计划的开始日期之间的差异的时间。 |
| static readonly [StatusManager](../../aspose.tasks/tsk/statusmanager/) | 要从资源中接收当前任务的状态更新的企业资源的名称。 |
| static readonly [Stop](../../aspose.tasks/tsk/stop/) | 表示任务实际部分结束的日期。 |
| static readonly [SubprojectName](../../aspose.tasks/tsk/subprojectname/) | 子项目的源位置。 |
| static readonly [SV](../../aspose.tasks/tsk/sv/) | 挣值进度差异，通过项目状态日期。 进度差异 (SV) 是 BCWP 和 BCWS 之间的差异。 |
| static readonly [TotalSlackTimeSpan](../../aspose.tasks/tsk/totalslacktimespan/) | 在不延迟项目完成日期的情况下可以延迟任务完成日期的时间。 |
| static readonly [Type](../../aspose.tasks/tsk/type/) | 任务的类型。 |
| static readonly [Uid](../../aspose.tasks/tsk/uid/) | 任务的唯一ID。 |
| static readonly [Warning](../../aspose.tasks/tsk/warning/) | 表示任务有进度差异的标志。 |
| static readonly [WBS](../../aspose.tasks/tsk/wbs/) | 工作分解结构 (WBS) 代码。 |
| static readonly [WBSLevel](../../aspose.tasks/tsk/wbslevel/) | 任务最右边的 WBS 级别。 |
| static readonly [Work](../../aspose.tasks/tsk/work/) | 为所有已分配资源安排的任务总时间。 |
| static readonly [WorkVariance](../../aspose.tasks/tsk/workvariance/) | 任务的基线工时与当前计划工时之间的差异。 |

### 也可以看看

* 命名空间 [Aspose.Tasks](../../aspose.tasks/)
* 部件 [Aspose.Tasks](../../)


