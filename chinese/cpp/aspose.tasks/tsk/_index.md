---
title: "Aspose::Tasks::Tsk 类"
linktitle: "Tsk"
articleTitle: "Tsk"
second_title: "Aspose.Tasks for C++"
description: "表示 Task 对象的属性。"
type: docs
weight: 10
url: /zh/cpp/aspose.tasks/tsk/
---

## Tsk class

表示 Task 对象的属性。

## 方法

| 表示 ResourceAssignment 对象的属性。 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| [ActivityId](./activityid/) | 表示活动 ID 字段——Primavera 使用的任务唯一标识符。（仅适用于 Primavera 项目） |
| [ActualCost](./actualcost/) | 已由资源在其任务上完成的工作产生的费用，以及与任务相关的任何其他已记录费用。 |
| [ActualDuration](./actualduration/) | 基于计划工期和当前剩余工作量或完成百分比的任务实际工作时间跨度。 |
| [ActualFinish](./actualfinish/) | 任务完成的日期。 |
| [ActualOvertimeCost](./actualovertimecost/) | 已由指派资源在任务上完成的加班工作产生的成本。 |
| [ActualOvertimeWork](./actualovertimework/) | 已由分配到任务的资源完成的实际加班工作量。 |
| [ActualOvertimeWorkProtected](./actualovertimeworkprotected/) | 实际加班工作受到保护的持续时间。 |
| [ActualStart](./actualstart/) | 任务实际开始的日期和时间。 |
| [ActualWork](./actualwork/) | 已由分配到任务的资源完成的工作量。 |
| [ActualWorkProtected](./actualworkprotected/) | 实际工作受到保护的持续时间。 |
| [ACWP](./acwp/) | 截至项目状态日期或今天的任务已完成工作产生的费用。 |
| [BCWP](./bcwp/) | 任务完成百分比乘以时间分阶段基线成本的累计值。 |
| [BCWS](./bcws/) | 截至状态日期或今天的累计时间分阶段基线成本。 |
| [BudgetCost](./budgetcost/) | 预算成本资源的预算成本。预算资源仅分配给项目汇总任务。 |
| [BudgetWork](./budgetwork/) | 预算工作用于预算工作和材料资源。预算资源仅分配给项目汇总任务。 |
| [Calendar](./calendar/) | 任务日历。 |
| [CommitmentFinish](./commitmentfinish/) | 交付的完成日期。 |
| [CommitmentStart](./commitmentstart/) | 交付的开始日期。 |
| [CommitmentType](./commitmenttype/) | 确定任务是否具有关联的交付或对关联交付的依赖关系。 |
| [ConstraintDate](./constraintdate/) | 与约束类型关联的具体日期。 |
| [ConstraintType](./constrainttype/) | 提供可用于任务调度的约束类型的选择。 |
| [Contact](./contact/) | 负责任务的个人姓名。 |
| [Cost](./cost/) | 任务的总计划或预计成本，包括已分配资源完成工作已产生的成本以及剩余工作计划的成本。 |
| [CostVariance](./costvariance/) | 任务、资源或分配的基准成本与总成本之间的差额。 |
| [Created](./created/) | 任务创建的日期。 |
| [CV](./cv/) | 任务的基准成本与总成本之间的差额。成本差异 = 成本 - 基准成本 |
| [Deadline](./deadline/) | 指示任务完成时间的目标日期。 |
| [DisplayAsSummary](./displayassummary/) | 确定任务是否应显示为汇总任务。 |
| [DisplayOnTimeline](./displayontimeline/) | 指定任务是否应在时间线视图中显示。 |
| [Duration](./duration/) | 任务的总活跃工作时间跨度，依据输入或 Microsoft Project 根据开始日期、结束日期、日历和其他调度因素计算得出。 |
| [DurationText](./durationtext/) | 返回任务的持续时间文本。 |
| [DurationVariance](./durationvariance/) | 任务的基准持续时间与总持续时间（当前估计）之间的差额。 |
| [EarlyFinish](./earlyfinish/) | 基于前置和后续任务的最早完成日期、其他约束以及任何平衡延迟，任务可能完成的最早日期。 |
| [EarlyStart](./earlystart/) | 基于前置和后续任务的最早开始日期以及其他约束，任务可能开始的最早日期。 |
| [EarnedValueMethod](./earnedvaluemethod/) | 确定是使用 % 完成还是物理 % 完成字段来计算已完成工作预算成本（BCWP）。 |
| [ExternalId](./externalid/) | 如果任务是外部任务，则包含该任务的外部 ID。 |
| [ExternalTaskProject](./externaltaskproject/) | 外部任务的来源位置和任务标识符。 |
| [ExternalUid](./externaluid/) | 当任务为外部任务时，包含其唯一标识符。 |
| [Finish](./finish/) | 任务的计划完成日期。 |
| [FinishSlackTimeSpan](./finishslacktimespan/) | 最早完成日期与最迟完成日期之间的持续时间。 |
| [FinishText](./finishtext/) | 返回任务的完成文本。 |
| [FinishVariance](./finishvariance/) | 表示任务或分配的基准完成日期与当前完成日期之间差异的时间。 |
| [FixedCost](./fixedcost/) | 显示任何非资源任务费用。 |
| [FixedCostAccrual](./fixedcostaccrual/) | 确定固定成本何时以及如何计入任务成本的选择。 |
| [FreeSlackTimeSpan](./freeslacktimespan/) | 任务可以延迟的时间，而不会导致任何后继任务延迟。 |
| [Guid](./guid/) | 为任务生成的唯一标识代码。 |
| [HasOverallocatedResource](./hasoverallocatedresource/) | 指示任务是否分配了资源，该资源在已分配的任务上工作量超过正常工作容量所能完成的范围。 |
| [HideBar](./hidebar/) | 确定在 Microsoft Project 中显示时，任务的甘特条是否隐藏。 |
| [Hyperlink](./hyperlink/) | 与任务关联的超链接的标题或说明文字。 |
| [HyperlinkAddress](./hyperlinkaddress/) | 与任务关联的超链接的地址。 |
| [HyperlinkSubAddress](./hyperlinksubaddress/) | 任务关联的超链接中文档的具体位置。 |
| [Id](./id/) | 任务在任务列表中的位置标识符。 |
| [IgnoreResourceCalendar](./ignoreresourcecalendar/) | 确定任务的调度是否考虑分配给该任务的资源日历。 |
| [IgnoreWarnings](./ignorewarnings/) | 指示是否在 Microsoft Project 中隐藏调度冲突警告指示器。 |
| [IsActive](./isactive/) | 确定任务是否处于活动状态。非活动任务不再影响其他任务或整体项目进度。 |
| [IsCritical](./iscritical/) | 确定任务是否位于关键路径上。 |
| [IsEffortDriven](./iseffortdriven/) | 确定任务的调度是否为基于工作量的调度。 |
| [IsEstimated](./isestimated/) | 确定任务是否为估计任务。 |
| [IsExpanded](./isexpanded/) | 确定在甘特图视图中汇总任务是否展开。 |
| [IsExternalTask](./isexternaltask/) | 确定任务是否为外部任务。 |
| [IsManual](./ismanual/) | 确定任务是否手动调度。 |
| [IsMarked](./ismarked/) | 显示任务是否标记为需要进一步操作或某种标识。 |
| [IsMilestone](./ismilestone/) | 确定任务是否为里程碑。 |
| [IsNull](./isnull/) | 确定任务是否为空任务。 |
| [IsOverallocated](./isoverallocated/) | 指示任务上分配的任何资源是否承担了超过正常工作容量的工作量。 |
| [IsPublished](./ispublished/) | 确定当前任务是否应与项目的其他部分一起发布到 Project Server。 |
| [IsRecurring](./isrecurring/) | 确定任务是否属于一系列循环任务。 |
| [IsResumeValid](./isresumevalid/) | 确定任务是否可以恢复。 |
| [IsRollup](./isrollup/) | 确定子任务甘特条的信息是否会汇总到汇总任务条中。 |
| [IsSubproject](./issubproject/) | 确定任务是否为插入的项目。 |
| [IsSubprojectReadOnly](./issubprojectreadonly/) | 确定子项目是否为只读。 |
| [IsSummary](./issummary/) | 确定任务是否为汇总任务。 |
| [LateFinish](./latefinish/) | 任务可以完成而不延迟项目完成的最迟日期。 |
| [LateStart](./latestart/) | 任务可以开始而不延迟项目完成的最迟日期。 |
| [LevelAssignments](./levelassignments/) | 确定平衡功能是否可以延迟并拆分各个分配，以解决资源超额分配。 |
| [LevelingCanSplit](./levelingcansplit/) | 确定资源平衡功能是否会对该任务的剩余工作进行拆分。 |
| [LevelingDelay](./levelingdelay/) | 由于资源平衡，任务从其最早开始日期被延迟的时间。 |
| [ManualDuration](./manualduration/) | 定义任务的手动计划持续时间。 |
| [ManualFinish](./manualfinish/) | 定义任务的手动计划完成时间。 |
| [ManualStart](./manualstart/) | 定义任务的手动计划开始时间。 |
| [Name](./name/) | 任务名称。 |
| [NotesRTF](./notesrtf/) | RTF 格式的文本备注。 |
| [NotesText](./notestext/) | 从 RTF 数据中提取的备注纯文本。 |
| [OutlineLevel](./outlinelevel/) | 任务的轮廓级别。 |
| [OutlineNumber](./outlinenumber/) | 表示任务在层次结构大纲中的位置的数字。 |
| [OvertimeCost](./overtimecost/) | 任务的加班总成本，或资源在所有分配任务上的加班总成本，或资源分配的加班成本。 |
| [OvertimeWork](./overtimework/) | 分配给任务的所有资源计划执行的加班量。 |
| [PercentComplete](./percentcomplete/) | 任务的当前状态，以已完成的任务持续时间百分比表示。 |
| [PercentWorkComplete](./percentworkcomplete/) | 任务的当前状态，以已完成的工作百分比表示。 |
| [PhysicalPercentComplete](./physicalpercentcomplete/) | 可用作计算已完成工作预算成本（BCWP）的替代值的完成百分比。 |
| [PreleveledFinish](./preleveledfinish/) | 资源平衡之前任务的完成日期。 |
| [PreleveledStart](./preleveledstart/) | 资源平衡之前任务的开始日期。 |
| [Priority](./priority/) | 任务的重要性级别，这反映了在资源平衡期间任务或分配被延迟或拆分的容易程度。 |
| [RegularWork](./regularwork/) | 资源计划执行的非加班工作总量。 |
| [RemainingCost](./remainingcost/) | 完成剩余计划工作将产生的剩余计划费用。 |
| [RemainingDuration](./remainingduration/) | 完成任务未完成部分所需的时间。 |
| [RemainingOvertimeCost](./remainingovertimecost/) | 任务剩余的计划加班费用。 |
| [RemainingOvertimeWork](./remainingovertimework/) | 剩余的计划加班时间量。 |
| [RemainingWork](./remainingwork/) | 完成任务或任务集仍需的时间。 |
| [Resume](./resume/) | 任务剩余部分在进入任何进度后计划恢复的日期。 |
| [Start](./start/) | 任务的计划开始日期。 |
| [StartSlackTimeSpan](./startslacktimespan/) | 早开始日期和晚开始日期之间的持续时间。 |
| [StartText](./starttext/) | 返回任务的开始文本。 |
| [StartVariance](./startvariance/) | 表示任务或分配的基准开始日期与当前计划开始日期之间差异的时间。 |
| [StatusManager](./statusmanager/) | 企业资源的名称，该资源将从资源处接收当前任务的状态更新。 |
| [Stop](./stop/) | 表示任务实际部分结束的日期。 |
| [SubprojectName](./subprojectname/) | 子项目的源位置。 |
| [SV](./sv/) | 截至项目状态日期的挣值进度偏差。进度偏差（SV）是 BCWP 与 BCWS 之间的差异。 |
| [TotalSlackTimeSpan](./totalslacktimespan/) | 任务完成日期可延迟而不影响项目完成日期的时间。 |
| [Type](./type/) | 任务的类型。 |
| [Uid](./uid/) | 任务的唯一标识符。 |
| [Warning](./warning/) | 表示指示任务存在进度差异的标志。 |
| [WBS](./wbs/) | 工作分解结构（WBS）代码。 |
| [WBSLevel](./wbslevel/) | 任务最右侧的 WBS 层级。 |
| [Work](./work/) | 为所有分配资源在任务上计划的总时间。 |
| [WorkVariance](./workvariance/) | 任务基准工作与当前计划工作之间的差异。 |

