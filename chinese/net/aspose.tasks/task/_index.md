---
title: "类 Task"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Task 类。表示项目中的任务"
type: docs
weight: 2360
url: /zh/net/aspose.tasks/task/
---
## Task class

表示项目中的任务。

```csharp
public class Task : IEquatable<Task>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [ActivityId](../../aspose.tasks/task/activityid/) { get; set; } | 表示活动 ID 字段——Primavera 使用的任务唯一标识符。（仅适用于 Primavera 项目） |
| [ActualCost](../../aspose.tasks/task/actualcost/) { get; set; } | 获取或设置 ActualCost 的值。 |
| [ActualDuration](../../aspose.tasks/task/actualduration/) { get; set; } | 获取或设置 ActualDuration 的值。 |
| [ActualFinish](../../aspose.tasks/task/actualfinish/) { get; set; } | 获取或设置 ActualFinish 的值。 |
| [ActualOvertimeCost](../../aspose.tasks/task/actualovertimecost/) { get; set; } | 获取或设置 ActualOvertimeCost 的值。 |
| [ActualOvertimeWork](../../aspose.tasks/task/actualovertimework/) { get; set; } | 获取或设置 ActualOvertimeWork 的值。 |
| [ActualOvertimeWorkProtected](../../aspose.tasks/task/actualovertimeworkprotected/) { get; set; } | 获取或设置 ActualOvertimeWorkProtected 的值。 |
| [ActualStart](../../aspose.tasks/task/actualstart/) { get; set; } | 获取或设置 ActualStart 的值。 |
| [ActualWork](../../aspose.tasks/task/actualwork/) { get; set; } | 获取或设置 ActualWork 的值。 |
| [ActualWorkProtected](../../aspose.tasks/task/actualworkprotected/) { get; set; } | 获取或设置 ActualWorkProtected 的值。 |
| [ACWP](../../aspose.tasks/task/acwp/) { get; set; } | 获取或设置 ACWP 的值。 |
| [Assignments](../../aspose.tasks/task/assignments/) { get; } | 获取此对象的资源分配集合。 |
| [Baselines](../../aspose.tasks/task/baselines/) { get; set; } | 获取或设置任务的基线值集合。 |
| [BCWP](../../aspose.tasks/task/bcwp/) { get; set; } | 获取或设置 BCWP 的值。 |
| [BCWS](../../aspose.tasks/task/bcws/) { get; set; } | 获取或设置 BCWS 的值。 |
| [BudgetCost](../../aspose.tasks/task/budgetcost/) { get; set; } | 获取或设置 BudgetCost 的值。 |
| [BudgetWork](../../aspose.tasks/task/budgetwork/) { get; set; } | 获取或设置 BudgetWork 的值。 |
| [Calendar](../../aspose.tasks/task/calendar/) { get; set; } | 获取或设置 Calendar 的值。 |
| [Children](../../aspose.tasks/task/children/) { get; } | 获取此对象的子任务集合。TaskCollection 对象，表示子任务。 |
| [CommitmentFinish](../../aspose.tasks/task/commitmentfinish/) { get; set; } | 获取或设置 CommitmentFinish 的值。 |
| [CommitmentStart](../../aspose.tasks/task/commitmentstart/) { get; set; } | 获取或设置 CommitmentStart 的值。 |
| [CommitmentType](../../aspose.tasks/task/commitmenttype/) { get; set; } | 获取或设置 CommitmentType 的值。 |
| [ConstraintDate](../../aspose.tasks/task/constraintdate/) { get; set; } | 获取或设置 ConstraintDate 的值。 |
| [ConstraintType](../../aspose.tasks/task/constrainttype/) { get; set; } | 获取或设置 ConstraintType 的值。 |
| [Contact](../../aspose.tasks/task/contact/) { get; set; } | 获取或设置 Contact 的值。 |
| [Cost](../../aspose.tasks/task/cost/) { get; set; } | 获取或设置 Cost 的值。 |
| [CostVariance](../../aspose.tasks/task/costvariance/) { get; set; } | 获取或设置 CostVariance 的值。 |
| [Created](../../aspose.tasks/task/created/) { get; set; } | 获取或设置 Created 的值。 |
| [CV](../../aspose.tasks/task/cv/) { get; set; } | 获取或设置 CV 的值。 |
| [Deadline](../../aspose.tasks/task/deadline/) { get; set; } | 获取或设置 Deadline 的值。 |
| [DisplayAsSummary](../../aspose.tasks/task/displayassummary/) { get; set; } | 获取或设置一个值，指示是否已设置 DisplayAsSummary。 |
| [DisplayOnTimeline](../../aspose.tasks/task/displayontimeline/) { get; set; } | 获取或设置一个值，指示是否已设置 DisplayOnTimeline。 |
| [Duration](../../aspose.tasks/task/duration/) { get; set; } | 获取或设置 Duration 的值。 |
| [DurationFormat](../../aspose.tasks/task/durationformat/) { get; set; } | 获取或设置 DurationFormat 的值。 |
| [DurationText](../../aspose.tasks/task/durationtext/) { get; set; } | 获取或设置 DurationText 的值。 |
| [DurationVariance](../../aspose.tasks/task/durationvariance/) { get; set; } | 获取或设置 DurationVariance 的值。 |
| [EarlyFinish](../../aspose.tasks/task/earlyfinish/) { get; set; } | 获取或设置 EarlyFinish 的值。 |
| [EarlyStart](../../aspose.tasks/task/earlystart/) { get; set; } | 获取或设置 EarlyStart 的值。 |
| [EarnedValueMethod](../../aspose.tasks/task/earnedvaluemethod/) { get; set; } | 获取或设置 EarnedValueMethod 的值。 |
| [ExtendedAttributes](../../aspose.tasks/task/extendedattributes/) { get; } | 获取包含扩展属性值的 ExtendedAttributeCollection 对象。 |
| [ExternalId](../../aspose.tasks/task/externalid/) { get; set; } | 获取或设置 ExternalId 的值。 |
| [ExternalTaskProject](../../aspose.tasks/task/externaltaskproject/) { get; set; } | 获取或设置 ExternalTaskProject 的值。 |
| [ExternalUid](../../aspose.tasks/task/externaluid/) { get; set; } | 获取或设置外部任务的唯一标识符（当任务为外部时）。 |
| [Finish](../../aspose.tasks/task/finish/) { get; set; } | 获取或设置 Finish 的值。 |
| [FinishSlack](../../aspose.tasks/task/finishslack/) { get; set; } | 获取或设置 FinishSlack 的值。 |
| [FinishText](../../aspose.tasks/task/finishtext/) { get; set; } | 获取或设置 FinishText 的值。 |
| [FinishVariance](../../aspose.tasks/task/finishvariance/) { get; set; } | 获取或设置 FinishVariance 的值。 |
| [FixedCost](../../aspose.tasks/task/fixedcost/) { get; set; } | 获取或设置 FixedCost 的值。 |
| [FixedCostAccrual](../../aspose.tasks/task/fixedcostaccrual/) { get; set; } | 获取或设置 FixedCostAccrual 的值。 |
| [FreeSlack](../../aspose.tasks/task/freeslack/) { get; set; } | 获取或设置 FreeSlack 的值。 |
| [Guid](../../aspose.tasks/task/guid/) { get; set; } | 获取或设置 Guid 的值。 |
| [HideBar](../../aspose.tasks/task/hidebar/) { get; set; } | 获取或设置一个值，指示是否已设置 HideBar。 |
| [Hyperlink](../../aspose.tasks/task/hyperlink/) { get; set; } | 获取或设置与任务关联的超链接的标题或说明文字。 |
| [HyperlinkAddress](../../aspose.tasks/task/hyperlinkaddress/) { get; set; } | 获取或设置与任务关联的超链接的地址。 |
| [HyperlinkSubAddress](../../aspose.tasks/task/hyperlinksubaddress/) { get; set; } | 获取或设置与任务关联的超链接中文档的具体位置。 |
| [Id](../../aspose.tasks/task/id/) { get; set; } | 获取或设置 Id 的值。 |
| [IgnoreResourceCalendar](../../aspose.tasks/task/ignoreresourcecalendar/) { get; set; } | 获取或设置一个值，指示是否已设置 IgnoreResourceCalendar。 |
| [IgnoreWarnings](../../aspose.tasks/task/ignorewarnings/) { get; set; } | 获取或设置一个值，指示是否已设置 IgnoreWarnings。 |
| [IsActive](../../aspose.tasks/task/isactive/) { get; set; } | 获取或设置一个值，指示是否已设置 IsActive。 |
| [IsCritical](../../aspose.tasks/task/iscritical/) { get; set; } | 获取或设置一个值，指示是否已设置 IsCritical。 |
| [IsEffortDriven](../../aspose.tasks/task/iseffortdriven/) { get; set; } | 获取或设置一个值，指示是否已设置 IsEffortDriven。 |
| [IsEstimated](../../aspose.tasks/task/isestimated/) { get; set; } | 获取或设置一个值，指示是否已设置 IsEstimated。 |
| [IsExpanded](../../aspose.tasks/task/isexpanded/) { get; set; } | 获取或设置一个值，指示 IsExpanded 是否已设置。 |
| [IsExternalTask](../../aspose.tasks/task/isexternaltask/) { get; set; } | 获取或设置一个值，指示 IsExternalTask 是否已设置。 |
| [IsManual](../../aspose.tasks/task/ismanual/) { get; set; } | 获取或设置一个值，指示 IsManual 是否已设置。 |
| [IsMarked](../../aspose.tasks/task/ismarked/) { get; set; } | 获取或设置一个值，指示 IsMarked 是否已设置。 |
| [IsMilestone](../../aspose.tasks/task/ismilestone/) { get; set; } | 获取或设置一个值，指示 IsMilestone 是否已设置。 |
| [IsNull](../../aspose.tasks/task/isnull/) { get; set; } | 获取或设置一个值，指示 IsNull 是否已设置。 |
| [IsOverallocated](../../aspose.tasks/task/isoverallocated/) { get; set; } | 获取或设置一个值，指示 IsOverallocated 是否已设置。 |
| [IsPublished](../../aspose.tasks/task/ispublished/) { get; set; } | 获取或设置一个值，指示 IsPublished 是否已设置。 |
| [IsRecurring](../../aspose.tasks/task/isrecurring/) { get; set; } | 获取或设置一个值，指示 IsRecurring 是否已设置。 |
| [IsResumeValid](../../aspose.tasks/task/isresumevalid/) { get; set; } | 获取或设置一个值，指示 IsResumeValid 是否已设置。 |
| [IsRollup](../../aspose.tasks/task/isrollup/) { get; set; } | 获取或设置一个值，指示 IsRollup 是否已设置。 |
| [IsSubproject](../../aspose.tasks/task/issubproject/) { get; set; } | 获取或设置一个值，指示 IsSubproject 是否已设置。 |
| [IsSubprojectReadOnly](../../aspose.tasks/task/issubprojectreadonly/) { get; set; } | 获取或设置一个值，指示 IsSubprojectReadOnly 是否已设置。 |
| [IsSummary](../../aspose.tasks/task/issummary/) { get; set; } | 获取或设置一个值，指示 IsSummary 是否已设置。 |
| [LateFinish](../../aspose.tasks/task/latefinish/) { get; set; } | 获取或设置 LateFinish 的值。 |
| [LateStart](../../aspose.tasks/task/latestart/) { get; set; } | 获取或设置 LateStart 的值。 |
| [LevelAssignments](../../aspose.tasks/task/levelassignments/) { get; set; } | 获取或设置一个值，指示 LevelAssignments 是否已设置。 |
| [LevelingCanSplit](../../aspose.tasks/task/levelingcansplit/) { get; set; } | 获取或设置一个值，指示 LevelingCanSplit 是否已设置。 |
| [LevelingDelay](../../aspose.tasks/task/levelingdelay/) { get; set; } | 获取或设置 LevelingDelay 的值。 |
| [ManualDuration](../../aspose.tasks/task/manualduration/) { get; set; } | 获取或设置 ManualDuration 的值。 |
| [ManualFinish](../../aspose.tasks/task/manualfinish/) { get; set; } | 获取或设置 ManualFinish 的值。 |
| [ManualStart](../../aspose.tasks/task/manualstart/) { get; set; } | 获取或设置 ManualStart 的值。 |
| [Name](../../aspose.tasks/task/name/) { get; set; } | 获取或设置 Name 的值。 |
| [NotesRTF](../../aspose.tasks/task/notesrtf/) { get; set; } | 获取或设置 NotesRTF 的值。 |
| [NotesText](../../aspose.tasks/task/notestext/) { get; set; } | 获取或设置 NotesText 的值。 |
| [OutlineCodes](../../aspose.tasks/task/outlinecodes/) { get; set; } | 获取或设置 [`OutlineCodeCollection`](../outlinecodecollection/) 对象。 |
| [OutlineLevel](../../aspose.tasks/task/outlinelevel/) { get; set; } | 获取或设置 OutlineLevel 的值。 |
| [OutlineNumber](../../aspose.tasks/task/outlinenumber/) { get; set; } | 获取或设置 OutlineNumber 的值。 |
| [OvertimeCost](../../aspose.tasks/task/overtimecost/) { get; set; } | 获取或设置 OvertimeCost 的值。 |
| [OvertimeWork](../../aspose.tasks/task/overtimework/) { get; set; } | 获取或设置 OvertimeWork 的值。 |
| [ParentProject](../../aspose.tasks/task/parentproject/) { get; } | 获取任务的父项目。 |
| [ParentTask](../../aspose.tasks/task/parenttask/) { get; } | 获取任务的父任务。 |
| [PercentComplete](../../aspose.tasks/task/percentcomplete/) { get; set; } | 获取或设置 PercentComplete 的值。 |
| [PercentWorkComplete](../../aspose.tasks/task/percentworkcomplete/) { get; set; } | 获取或设置 PercentWorkComplete 的值。 |
| [PhysicalPercentComplete](../../aspose.tasks/task/physicalpercentcomplete/) { get; set; } | 获取或设置 PhysicalPercentComplete 的值。 |
| [Predecessors](../../aspose.tasks/task/predecessors/) { get; } | 获取一个 [`TaskCollection`](../taskcollection/) 对象，其中包含此 Task 对象的所有前置任务。 |
| [PreleveledFinish](../../aspose.tasks/task/preleveledfinish/) { get; set; } | 获取或设置 PreleveledFinish 的值。 |
| [PreleveledStart](../../aspose.tasks/task/preleveledstart/) { get; set; } | 获取或设置 PreleveledStart 的值。 |
| [PrimaveraProperties](../../aspose.tasks/task/primaveraproperties/) { get; } | 获取一个对象，其中包含从 Primavera 文件读取的任务的 Primavera 特定属性。 |
| [Priority](../../aspose.tasks/task/priority/) { get; set; } | 获取或设置 Priority 的值。 |
| [RecurringInfo](../../aspose.tasks/task/recurringinfo/) { get; } | 获取任务的 [`RecurringTaskInfo`](../recurringtaskinfo/) 类实例（该任务为循环任务）；如果任务不是循环任务，则返回 null；[`RecurringTaskInfo`](../recurringtaskinfo/) 实例的信息仅在 mpp 文件格式中存在。 |
| [RegularWork](../../aspose.tasks/task/regularwork/) { get; set; } | 获取或设置 RegularWork 的值。 |
| [RemainingCost](../../aspose.tasks/task/remainingcost/) { get; set; } | 获取或设置 RemainingCost 的值。 |
| [RemainingDuration](../../aspose.tasks/task/remainingduration/) { get; set; } | 获取或设置 RemainingDuration 的值。 |
| [RemainingOvertimeCost](../../aspose.tasks/task/remainingovertimecost/) { get; set; } | 获取或设置 RemainingOvertimeCost 的值。 |
| [RemainingOvertimeWork](../../aspose.tasks/task/remainingovertimework/) { get; set; } | 获取或设置 RemainingOvertimeWork 的值。 |
| [RemainingWork](../../aspose.tasks/task/remainingwork/) { get; set; } | 获取或设置 RemainingWork 的值。 |
| [Resume](../../aspose.tasks/task/resume/) { get; set; } | 获取或设置 Resume 的值。 |
| [SplitParts](../../aspose.tasks/task/splitparts/) { get; } | 获取一个 SplitPart 集合，表示任务的各个部分。 |
| [Start](../../aspose.tasks/task/start/) { get; set; } | 获取或设置 Start 的值。 |
| [StartSlack](../../aspose.tasks/task/startslack/) { get; set; } | 获取或设置 StartSlack 的值。 |
| [StartText](../../aspose.tasks/task/starttext/) { get; set; } | 获取或设置 StartText 的值。 |
| [StartVariance](../../aspose.tasks/task/startvariance/) { get; set; } | 获取或设置 StartVariance 的值。 |
| [Status](../../aspose.tasks/task/status/) { get; } | 获取任务状态。 |
| [StatusManager](../../aspose.tasks/task/statusmanager/) { get; set; } | 获取或设置 StatusManager 的值。 |
| [Stop](../../aspose.tasks/task/stop/) { get; set; } | 获取或设置 Stop 的值。 |
| [SubprojectName](../../aspose.tasks/task/subprojectname/) { get; set; } | 获取或设置 SubprojectName 的值。 |
| [Successors](../../aspose.tasks/task/successors/) { get; } | 获取一个 [`TaskCollection`](../taskcollection/) 对象，其中包含此 Task 对象的所有后续任务。 |
| [SV](../../aspose.tasks/task/sv/) { get; set; } | 截至项目状态日期的挣值进度差异。进度差异（SV）是 BCWP 与 BCWS 之间的差额。 |
| [TimephasedData](../../aspose.tasks/task/timephaseddata/) { get; set; } | 获取或设置此任务的 TimephasedDataCollection 对象。与任务关联的时间分段数据块。 |
| [TotalSlack](../../aspose.tasks/task/totalslack/) { get; set; } | 获取或设置 TotalSlack 的值。 |
| [Type](../../aspose.tasks/task/type/) { get; set; } | 获取或设置 Type 的值。 |
| [Uid](../../aspose.tasks/task/uid/) { get; set; } | 获取或设置 Uid 的值。 |
| [Warning](../../aspose.tasks/task/warning/) { get; set; } | 获取或设置一个指示是否已设置 Warning 的值。 |
| [WBS](../../aspose.tasks/task/wbs/) { get; set; } | 获取或设置 WBS 的值。 |
| [WBSLevel](../../aspose.tasks/task/wbslevel/) { get; set; } | 获取或设置 WBSLevel 的值。 |
| [Work](../../aspose.tasks/task/work/) { get; set; } | 获取或设置 Work 的值。 |
| [WorkVariance](../../aspose.tasks/task/workvariance/) { get; set; } | 获取或设置 WorkVariance 的值。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Clone](../../aspose.tasks/task/clone/)() | 创建任务的完整副本（不包括子任务）。 |
| [Delete](../../aspose.tasks/task/delete/)() | 从父项目任务集合中删除任务以及其所有分配。 |
| override [Equals](../../aspose.tasks/task/equals/#equals_1)(object) | 返回一个值，指示此实例是否等于指定的对象。 |
| [Equals](../../aspose.tasks/task/equals/#equals)(Task) | 返回一个值，指示此实例是否等于指定的任务。 |
| [Get&lt;T&gt;](../../aspose.tasks/task/get/)(Key&lt;T, TaskKey&gt;) | 返回属性在此容器中映射的值。 |
| override [GetHashCode](../../aspose.tasks/task/gethashcode/)() | 返回此 Task 的哈希码值。 |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata/#gettimephaseddata)(DateTime, DateTime) | 返回在给定的开始和结束日期范围内，包含[`TimephasedData`](./timephaseddata/)值的[`TimephasedDataCollection`](../timephaseddatacollection/)对象。 |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata/#gettimephaseddata_1)(DateTime, DateTime, TimephasedDataType) | 返回在给定的开始和结束日期范围内、指定时间分段数据类型的[`TimephasedData`](./timephaseddata/)值的[`TimephasedDataCollection`](../timephaseddatacollection/)对象。 |
| [MoveToSibling](../../aspose.tasks/task/movetosibling/#movetosibling_1)(int) | 将当前任务在相同的 Outline Level 上移动到具有指定 Id 的任务之前。如果 ParentProject.CalculationMode 为 None，用户应在使用此方法后调用 Project.Recalculate()（它将重新安排所有项目任务（开始/结束日期，设置提前/延后日期）并计算诸如时差、工作和成本字段、轮廓级别等依赖字段）。如果 ParentProject.CalculationMode 为 Manual，方法仅自动计算任务 id、轮廓级别和轮廓编号。若 ParentProject.CalculationMode 为 Automatic，方法会自动重新安排所有项目任务（开始/结束日期，设置提前/延后日期，计算时差、工作和成本字段，重新计算 id 和轮廓级别）。 |
| [MoveToSibling](../../aspose.tasks/task/movetosibling/#movetosibling)(Task) | 将当前任务在相同的 Outline Level 上移动到指定任务之前。如果 ParentProject.CalculationMode 为 None，用户应在使用此方法后调用 Project.Recalculate()（它将重新安排所有项目任务（开始/结束日期，设置提前/延后日期）并计算诸如时差、工作和成本字段、轮廓级别等依赖字段）。如果 ParentProject.CalculationMode 为 Manual，方法仅自动计算任务 id、轮廓级别和轮廓编号。若 ParentProject.CalculationMode 为 Automatic，方法会自动重新安排所有项目任务（开始/结束日期，设置提前/延后日期，计算时差、工作和成本字段，重新计算 id 和轮廓级别）。 |
| [OutlineIndent](../../aspose.tasks/task/outlineindent/)() | 在大纲中缩进任务。 |
| [OutlineOutdent](../../aspose.tasks/task/outlineoutdent/)() | 在大纲中提升任务。 |
| [SelectAllChildTasks](../../aspose.tasks/task/selectallchildtasks/)() | 递归收集此任务的所有子任务。 |
| [Set&lt;T&gt;](../../aspose.tasks/task/set/)(Key&lt;T, TaskKey&gt;, T) | 将指定属性映射到此容器中的指定值。 |
| override [ToString](../../aspose.tasks/task/tostring/)() | 返回任务的简短字符串表示。表示的具体细节未指定，可能会更改。 |

## 备注

该 **Task** 表示一个原子工作块。

可以使用 **Task** 通过创建任务并分配适当的资源来规划项目。项目中的任务组织为一个根层次的树结构，包含根任务及其子任务子树。

要构建任务树，可以通过访问 [`RootTask`](../project/roottask/) 属性，使用专用集合 [`TaskCollection`](../taskcollection/) ，例如：

```csharp
Project project = new Project();

// 添加新任务
Task task1 = project.RootTask.Children.Add(); // a parent task with empty name is added
Task childTask1 = task1.Children.Add("Child 1");
childTask1.Set(Tsk.Start, new DateTime(2020, 2, 12, 8, 0, 0))
childTask1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask1.Set(Tsk.Finish, new DateTime(2020, 2, 12, 17, 0, 0));
Task childTask3 = task1.Children.Add("Child 3");
childTask3.Set(Tsk.Start, new DateTime(2020, 2, 13, 8, 0, 0))
childTask3.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask3.Set(Tsk.Finish, new DateTime(2020, 2, 13, 17, 0, 0));
Task childTask2 = task1.Children.Add("Child 2", 2); // inserts a task before the childTask3
childTask2.Set(Tsk.Start, new DateTime(2020, 2, 14, 8, 0, 0))
childTask2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask2.Set(Tsk.Finish, new DateTime(2020, 2, 14, 17, 0, 0));

// 将项目保存为可用格式之一
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

## 示例

展示如何向项目中添加任务。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "CreateNewTask_out.xml", SaveFileFormat.Xml);
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


