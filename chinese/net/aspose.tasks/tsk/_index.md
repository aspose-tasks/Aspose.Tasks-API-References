---
title: "类 Tsk"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Tsk 类。表示 Task 对象的属性"
type: docs
weight: 2620
url: /zh/net/aspose.tasks/tsk/
---
## Tsk class

表示 [`Task`](../task/) 对象的属性。

```csharp
public static class Tsk
```

## 字段

| 名称 | 描述 |
| --- | --- |
| static readonly [ActivityId](../../aspose.tasks/tsk/activityid/) | 表示活动 ID 字段——Primavera 使用的任务唯一标识符。（仅适用于 Primavera 项目） |
| static readonly [ActualCost](../../aspose.tasks/tsk/actualcost/) | 已由资源在其任务上完成的工作产生的成本，以及与任务相关的任何其他记录成本。 |
| static readonly [ActualDuration](../../aspose.tasks/tsk/actualduration/) | 基于计划持续时间和当前剩余工作或完成百分比的任务实际工作时间跨度。 |
| static readonly [ActualFinish](../../aspose.tasks/tsk/actualfinish/) | 任务完成的日期。 |
| static readonly [ActualOvertimeCost](../../aspose.tasks/tsk/actualovertimecost/) | 指派资源在任务上已完成的加班工作产生的费用。 |
| static readonly [ActualOvertimeWork](../../aspose.tasks/tsk/actualovertimework/) | 已由分配到任务的资源完成的实际加班工作量。 |
| static readonly [ActualOvertimeWorkProtected](../../aspose.tasks/tsk/actualovertimeworkprotected/) | 实际加班工作受到保护的持续时间。 |
| static readonly [ActualStart](../../aspose.tasks/tsk/actualstart/) | 任务实际开始的日期和时间。 |
| static readonly [ActualWork](../../aspose.tasks/tsk/actualwork/) | 已由分配到任务的资源完成的工作量。 |
| static readonly [ActualWorkProtected](../../aspose.tasks/tsk/actualworkprotected/) | 实际工作受到保护的持续时间。仅支持 XML 格式的读取。 |
| static readonly [ACWP](../../aspose.tasks/tsk/acwp/) | 截至项目状态日期或今天的任务已完成工作产生的成本。 |
| static readonly [BCWP](../../aspose.tasks/tsk/bcwp/) | 任务完成百分比乘以时间分阶段基线成本的累计值。 |
| static readonly [BCWS](../../aspose.tasks/tsk/bcws/) | 截至状态日期或今天的累计时间分阶段基线成本。 |
| static readonly [BudgetCost](../../aspose.tasks/tsk/budgetcost/) | 预算成本资源的预算成本。预算资源仅分配给项目汇总任务。 |
| static readonly [BudgetWork](../../aspose.tasks/tsk/budgetwork/) | 预算工作用于预算工作和材料资源。预算资源仅分配给项目汇总任务。 |
| static readonly [Calendar](../../aspose.tasks/tsk/calendar/) | 任务日历。 |
| static readonly [CommitmentFinish](../../aspose.tasks/tsk/commitmentfinish/) | 交付的完成日期。仅支持 XML 格式的读取。 |
| static readonly [CommitmentStart](../../aspose.tasks/tsk/commitmentstart/) | 交付的开始日期。仅支持 XML 格式的读取。 |
| static readonly [CommitmentType](../../aspose.tasks/tsk/commitmenttype/) | 确定任务是否具有关联的交付或对关联交付的依赖。仅支持 XML 格式的读取。 |
| static readonly [ConstraintDate](../../aspose.tasks/tsk/constraintdate/) | 与约束类型关联的特定日期。 |
| static readonly [ConstraintType](../../aspose.tasks/tsk/constrainttype/) | 提供可用于任务调度的约束类型的选择。 |
| static readonly [Contact](../../aspose.tasks/tsk/contact/) | 任务负责人的姓名。 |
| static readonly [Cost](../../aspose.tasks/tsk/cost/) | 任务的总计划或预计成本，基于已分配资源完成工作已产生的成本以及剩余工作计划的成本。 |
| static readonly [CostVariance](../../aspose.tasks/tsk/costvariance/) | 任务、资源或分配的基准成本与总成本之间的差额。 |
| static readonly [Created](../../aspose.tasks/tsk/created/) | 任务创建的日期。 |
| static readonly [CV](../../aspose.tasks/tsk/cv/) | 任务的基准成本与总成本之间的差额。成本差异 = 成本 - 基准成本。 |
| static readonly [Deadline](../../aspose.tasks/tsk/deadline/) | 指示任务完成时间的目标日期。 |
| static readonly [DisplayAsSummary](../../aspose.tasks/tsk/displayassummary/) | 确定任务是否应显示为汇总任务。仅支持 XML 格式的读取。 |
| static readonly [DisplayOnTimeline](../../aspose.tasks/tsk/displayontimeline/) | 指定任务是否应在时间轴视图中显示。 |
| static readonly [Duration](../../aspose.tasks/tsk/duration/) | 任务的总活跃工作时间跨度，依据输入或 Microsoft Project 根据开始日期、完成日期、日历及其他调度因素计算得出。 |
| static readonly [DurationText](../../aspose.tasks/tsk/durationtext/) | 返回任务的持续时间文本。 |
| static readonly [DurationVariance](../../aspose.tasks/tsk/durationvariance/) | 任务的基准持续时间与总持续时间（当前估计）之间的差额。 |
| static readonly [EarlyFinish](../../aspose.tasks/tsk/earlyfinish/) | 基于前置和后续任务的最早完成日期、其他约束以及任何平衡延迟，任务可能完成的最早日期。 |
| static readonly [EarlyStart](../../aspose.tasks/tsk/earlystart/) | 基于前置和后续任务的最早开始日期以及其他约束，任务可能开始的最早日期。 |
| static readonly [EarnedValueMethod](../../aspose.tasks/tsk/earnedvaluemethod/) | 确定应使用“完成百分比”还是“实际完成百分比”字段来计算已完成工作预算成本（BCWP）。 |
| static readonly [ExternalId](../../aspose.tasks/tsk/externalid/) | 如果任务是外部任务，则包含该任务的外部 ID。 |
| static readonly [ExternalTaskProject](../../aspose.tasks/tsk/externaltaskproject/) | 外部任务的来源位置和任务标识符。 |
| static readonly [ExternalUid](../../aspose.tasks/tsk/externaluid/) | 当任务为外部任务时，包含外部任务的唯一标识符。 |
| static readonly [Finish](../../aspose.tasks/tsk/finish/) | 任务的计划完成日期。 |
| static readonly [FinishSlackTimeSpan](../../aspose.tasks/tsk/finishslacktimespan/) | 最早完成日期与最迟完成日期之间的持续时间。 |
| static readonly [FinishText](../../aspose.tasks/tsk/finishtext/) | 返回任务的完成文本。 |
| static readonly [FinishVariance](../../aspose.tasks/tsk/finishvariance/) | 表示任务或分配的基准完成日期与当前完成日期之间差异的时间。 |
| static readonly [FixedCost](../../aspose.tasks/tsk/fixedcost/) | 显示任何非资源任务费用。 |
| static readonly [FixedCostAccrual](../../aspose.tasks/tsk/fixedcostaccrual/) | 确定固定成本何时以及如何计入任务成本的选项。 |
| static readonly [FreeSlackTimeSpan](../../aspose.tasks/tsk/freeslacktimespan/) | 任务可以延迟而不影响任何后续任务的时间。 |
| static readonly [Guid](../../aspose.tasks/tsk/guid/) | 为任务生成的唯一标识代码。 |
| static readonly [HasOverallocatedResource](../../aspose.tasks/tsk/hasoverallocatedresource/) | 指示任务是否分配了资源，该资源在已分配的任务上工作量超过正常工作容量所能完成的范围。 |
| static readonly [HideBar](../../aspose.tasks/tsk/hidebar/) | 确定在 Microsoft Project 中显示时，任务的甘特条是否被隐藏。 |
| static readonly [Hyperlink](../../aspose.tasks/tsk/hyperlink/) | 与任务关联的超链接的标题或说明文字。 |
| static readonly [HyperlinkAddress](../../aspose.tasks/tsk/hyperlinkaddress/) | 与任务关联的超链接的地址。 |
| static readonly [HyperlinkSubAddress](../../aspose.tasks/tsk/hyperlinksubaddress/) | 与任务关联的超链接在文档中的具体位置。 |
| static readonly [Id](../../aspose.tasks/tsk/id/) | 任务在任务列表中的位置标识符。 |
| static readonly [IgnoreResourceCalendar](../../aspose.tasks/tsk/ignoreresourcecalendar/) | 确定任务的调度是否考虑了分配给该任务的资源日历。 |
| static readonly [IgnoreWarnings](../../aspose.tasks/tsk/ignorewarnings/) | 指示是否在 Microsoft Project 中隐藏日程冲突警告指示器。 |
| static readonly [IsActive](../../aspose.tasks/tsk/isactive/) | 确定任务是否处于活动状态。非活动任务不再影响其他任务或整体项目进度。 |
| static readonly [IsCritical](../../aspose.tasks/tsk/iscritical/) | 确定任务是否位于关键路径上。 |
| static readonly [IsEffortDriven](../../aspose.tasks/tsk/iseffortdriven/) | 确定任务的调度是否为基于工作量的调度。 |
| static readonly [IsEstimated](../../aspose.tasks/tsk/isestimated/) | 确定任务是否为估计任务。 |
| static readonly [IsExpanded](../../aspose.tasks/tsk/isexpanded/) | 确定在甘特图视图中汇总任务是否展开。 |
| static readonly [IsExternalTask](../../aspose.tasks/tsk/isexternaltask/) | 确定任务是否为外部任务。 |
| static readonly [IsManual](../../aspose.tasks/tsk/ismanual/) | 确定任务是否为手动调度。 |
| static readonly [IsMarked](../../aspose.tasks/tsk/ismarked/) | 显示任务是否被标记为需要进一步操作或某种标识。 |
| static readonly [IsMilestone](../../aspose.tasks/tsk/ismilestone/) | 确定任务是否为里程碑。 |
| static readonly [IsNull](../../aspose.tasks/tsk/isnull/) | 确定任务是否为空任务。 |
| static readonly [IsOverallocated](../../aspose.tasks/tsk/isoverallocated/) | 指示任务上分配的任何资源是否承担了超过正常工作容量的工作量。 |
| static readonly [IsPublished](../../aspose.tasks/tsk/ispublished/) | 确定当前任务是否应与项目的其他部分一起发布到 Project Server。 |
| static readonly [IsRecurring](../../aspose.tasks/tsk/isrecurring/) | 确定任务是否是循环任务系列的一部分。 |
| static readonly [IsResumeValid](../../aspose.tasks/tsk/isresumevalid/) | 确定任务是否可以恢复。 |
| static readonly [IsRollup](../../aspose.tasks/tsk/isrollup/) | 确定子任务甘特条的信息是否会汇总到汇总任务条中。 |
| static readonly [IsSubproject](../../aspose.tasks/tsk/issubproject/) | 确定任务是否为插入的项目。 |
| static readonly [IsSubprojectReadOnly](../../aspose.tasks/tsk/issubprojectreadonly/) | 确定子项目是否为只读。 |
| static readonly [IsSummary](../../aspose.tasks/tsk/issummary/) | 确定任务是否为汇总任务。 |
| static readonly [LateFinish](../../aspose.tasks/tsk/latefinish/) | 任务可以完成而不延迟项目完成的最晚日期。 |
| static readonly [LateStart](../../aspose.tasks/tsk/latestart/) | 任务可以开始而不延迟项目完成的最晚日期。 |
| static readonly [LevelAssignments](../../aspose.tasks/tsk/levelassignments/) | 确定平衡功能是否可以延迟并拆分单个任务分配，以解决资源超额分配。 |
| static readonly [LevelingCanSplit](../../aspose.tasks/tsk/levelingcansplit/) | 确定资源平衡功能是否会对该任务的剩余工作进行拆分。 |
| static readonly [LevelingDelay](../../aspose.tasks/tsk/levelingdelay/) | 由于资源平衡，任务相对于其最早开始日期的延迟时间。 |
| static readonly [ManualDuration](../../aspose.tasks/tsk/manualduration/) | 定义任务的手动计划工期。 |
| static readonly [ManualFinish](../../aspose.tasks/tsk/manualfinish/) | 定义任务的手动计划完成时间。 |
| static readonly [ManualStart](../../aspose.tasks/tsk/manualstart/) | 定义任务的手动计划开始时间。 |
| static readonly [Name](../../aspose.tasks/tsk/name/) | 任务名称。 |
| static readonly [NotesRTF](../../aspose.tasks/tsk/notesrtf/) | RTF 格式的文本备注。仅支持 MPP 格式。 |
| static readonly [NotesText](../../aspose.tasks/tsk/notestext/) | 从 RTF 数据中提取的备注纯文本。 |
| static readonly [OutlineLevel](../../aspose.tasks/tsk/outlinelevel/) | 任务的大纲层级。 |
| static readonly [OutlineNumber](../../aspose.tasks/tsk/outlinenumber/) | 表示任务在层次大纲结构中位置的编号。 |
| static readonly [OvertimeCost](../../aspose.tasks/tsk/overtimecost/) | 任务的加班总费用，或资源在所有分配任务上的加班费用，或资源分配的加班费用。 |
| static readonly [OvertimeWork](../../aspose.tasks/tsk/overtimework/) | 分配给任务的所有资源计划执行的加班量。 |
| static readonly [PercentComplete](../../aspose.tasks/tsk/percentcomplete/) | 任务的当前状态，以已完成的任务工期百分比表示。 |
| static readonly [PercentWorkComplete](../../aspose.tasks/tsk/percentworkcomplete/) | 任务的当前状态，以已完成的工作百分比表示。 |
| static readonly [PhysicalPercentComplete](../../aspose.tasks/tsk/physicalpercentcomplete/) | 可用作计算已完成工作预算成本（BCWP）的替代值的完成百分比。 |
| static readonly [PreleveledFinish](../../aspose.tasks/tsk/preleveledfinish/) | 资源平衡之前任务的完成日期。 |
| static readonly [PreleveledStart](../../aspose.tasks/tsk/preleveledstart/) | 资源平衡之前任务的开始日期。 |
| static readonly [Priority](../../aspose.tasks/tsk/priority/) | 任务的重要性级别，这反映了在资源平衡期间任务或分配被延迟或拆分的可能性。 |
| static readonly [RegularWork](../../aspose.tasks/tsk/regularwork/) | 资源计划执行的非加班工作总量。 |
| static readonly [RemainingCost](../../aspose.tasks/tsk/remainingcost/) | 完成剩余计划工作将产生的剩余计划费用。 |
| static readonly [RemainingDuration](../../aspose.tasks/tsk/remainingduration/) | 完成任务未完成部分所需的时间。 |
| static readonly [RemainingOvertimeCost](../../aspose.tasks/tsk/remainingovertimecost/) | 任务剩余的计划加班费用。 |
| static readonly [RemainingOvertimeWork](../../aspose.tasks/tsk/remainingovertimework/) | 剩余的计划加班时间量。 |
| static readonly [RemainingWork](../../aspose.tasks/tsk/remainingwork/) | 完成任务或任务集仍需的时间。 |
| static readonly [Resume](../../aspose.tasks/tsk/resume/) | 任务剩余部分在进入任何进度后计划恢复的日期。 |
| static readonly [Start](../../aspose.tasks/tsk/start/) | 任务的计划开始日期。 |
| static readonly [StartSlackTimeSpan](../../aspose.tasks/tsk/startslacktimespan/) | 早开始和晚开始日期之间的持续时间。 |
| static readonly [StartText](../../aspose.tasks/tsk/starttext/) | 返回任务的开始文本。 |
| static readonly [StartVariance](../../aspose.tasks/tsk/startvariance/) | 表示任务或分配的基准开始日期与当前计划开始日期之间差异的时间。 |
| static readonly [StatusManager](../../aspose.tasks/tsk/statusmanager/) | 企业资源的名称，该资源将从资源处接收当前任务的状态更新。 |
| static readonly [Stop](../../aspose.tasks/tsk/stop/) | 表示任务实际部分结束的日期。 |
| static readonly [SubprojectName](../../aspose.tasks/tsk/subprojectname/) | 子项目的源位置。 |
| static readonly [SV](../../aspose.tasks/tsk/sv/) | 截至项目状态日期的挣值进度差异。进度差异（SV）是 BCWP 与 BCWS 之间的差额。 |
| static readonly [TotalSlackTimeSpan](../../aspose.tasks/tsk/totalslacktimespan/) | 任务完成日期可以延迟而不影响项目完成日期的时间。 |
| static readonly [Type](../../aspose.tasks/tsk/type/) | 任务的类型。 |
| static readonly [Uid](../../aspose.tasks/tsk/uid/) | 任务的唯一标识。 |
| static readonly [Warning](../../aspose.tasks/tsk/warning/) | 表示 指示任务存在计划差异的标志。 |
| static readonly [WBS](../../aspose.tasks/tsk/wbs/) | 工作分解结构（WBS）代码。 |
| static readonly [WBSLevel](../../aspose.tasks/tsk/wbslevel/) | 任务最右侧的 WBS 级别。 |
| static readonly [Work](../../aspose.tasks/tsk/work/) | 为所有分配资源在任务上计划的总时间。 |
| static readonly [WorkVariance](../../aspose.tasks/tsk/workvariance/) | 任务基准工作量与当前计划工作量之间的差异。 |

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


