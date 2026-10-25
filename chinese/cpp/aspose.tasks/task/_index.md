---
title: "Aspose::Tasks::Task 类"
linktitle: "Task"
articleTitle: "Task"
second_title: "Aspose.Tasks for C++"
description: "表示项目中的任务。"
type: docs
weight: 10
url: /zh/cpp/aspose.tasks/task/
---

## Task class

**Inherits:** Aspose::Tasks::IEntityWithTd

表示项目中的任务。

Task 表示一个原子工作块。

可以使用 Task 通过创建任务并分配适当的资源来规划项目。项目中的任务组织为根层次树结构，包含根任务以及子任务的子树。

要构建任务树，可以使用专门的集合 Aspose::Tasks::TaskCollection，通过访问 Project::RootTask 属性，例如：

```cpp
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

## 方法

| 表示 ResourceAssignment 对象的属性。 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| [Clone](./clone/) | 创建任务的完整副本（不包括子任务）。 |
| [Delete](./delete/) | 从父项目任务集合中删除任务及其所有分配。 |
| [Equals (2 overloads)](./equals/) | 返回一个值，指示此实例是否等于指定的对象。 |
| [Get](./get/) | 返回属性在此容器中映射的值。 |
| [get_ActivityId](./get_activityid/) | 表示活动 ID 字段——Primavera 使用的任务唯一标识符。（仅适用于 Primavera 项目） |
| [get_ActualCost](./get_actualcost/) | 获取 ActualCost 的值。 |
| [get_ActualDuration](./get_actualduration/) | 获取 ActualDuration 的值。 |
| [get_ActualFinish](./get_actualfinish/) | 获取 ActualFinish 的值。 |
| [get_ActualOvertimeCost](./get_actualovertimecost/) | 获取 ActualOvertimeCost 的值。 |
| [get_ActualOvertimeWork](./get_actualovertimework/) | 获取 ActualOvertimeWork 的值。 |
| [get_ActualOvertimeWorkProtected](./get_actualovertimeworkprotected/) | 获取 ActualOvertimeWorkProtected 的值。 |
| [get_ActualStart](./get_actualstart/) | 获取 ActualStart 的值。 |
| [get_ActualWork](./get_actualwork/) | 获取 ActualWork 的值。 |
| [get_ActualWorkProtected](./get_actualworkprotected/) | 获取 ActualWorkProtected 的值。 |
| [get_ACWP](./get_acwp/) | 获取 ACWP 的值。 |
| [get_Assignments](./get_assignments/) | 获取此对象的资源分配集合。 |
| [get_Baselines](./get_baselines/) | 获取任务基线值的集合。 |
| [get_BCWP](./get_bcwp/) | 获取 BCWP 的值。 |
| [get_BCWS](./get_bcws/) | 获取 BCWS 的值。 |
| [get_BudgetCost](./get_budgetcost/) | 获取 BudgetCost 的值。 |
| [get_BudgetWork](./get_budgetwork/) | 获取 BudgetWork 的值。 |
| [get_Calendar](./get_calendar/) | 获取 Calendar 的值。 |
| [get_Children](./get_children/) | 获取此对象的子任务集合。TaskCollection 对象表示子任务。 |
| [get_CommitmentFinish](./get_commitmentfinish/) | 获取 CommitmentFinish 的值。 |
| [get_CommitmentStart](./get_commitmentstart/) | 获取 CommitmentStart 的值。 |
| [get_CommitmentType](./get_commitmenttype/) | 获取 CommitmentType 的值。 |
| [get_ConstraintDate](./get_constraintdate/) | 获取 ConstraintDate 的值。 |
| [get_ConstraintType](./get_constrainttype/) | 获取 ConstraintType 的值。 |
| [get_Contact](./get_contact/) | 获取 Contact 的值。 |
| [get_Cost](./get_cost/) | 获取 Cost 的值。 |
| [get_CostVariance](./get_costvariance/) | 获取 CostVariance 的值。 |
| [get_Created](./get_created/) | 获取 Created 的值。 |
| [get_CV](./get_cv/) | 获取 CV 的值。 |
| [get_Deadline](./get_deadline/) | 获取 Deadline 的值。 |
| [get_DisplayAsSummary](./get_displayassummary/) | 获取指示是否设置了 DisplayAsSummary 的值。 |
| [get_DisplayOnTimeline](./get_displayontimeline/) | 获取指示是否设置了 DisplayOnTimeline 的值。 |
| [get_Duration](./get_duration/) | 获取 Duration 的值。 |
| [get_DurationFormat](./get_durationformat/) | 获取 DurationFormat 的值。 |
| [get_DurationText](./get_durationtext/) | 获取 DurationText 的值。 |
| [get_DurationVariance](./get_durationvariance/) | 获取 DurationVariance 的值。 |
| [get_EarlyFinish](./get_earlyfinish/) | 获取 EarlyFinish 的值。 |
| [get_EarlyStart](./get_earlystart/) | 获取 EarlyStart 的值。 |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | 获取 EarnedValueMethod 的值。 |
| [get_ExtendedAttributes](./get_extendedattributes/) | 获取包含扩展属性值的 ExtendedAttributeCollection 对象。 |
| [get_ExternalId](./get_externalid/) | 获取 ExternalId 的值。 |
| [get_ExternalTaskProject](./get_externaltaskproject/) | 获取 ExternalTaskProject 的值。 |
| [get_ExternalUid](./get_externaluid/) | 获取或设置外部任务为外部时的唯一标识符。 |
| [get_Finish](./get_finish/) | 获取 Finish 的值。 |
| [get_FinishSlack](./get_finishslack/) | 获取 FinishSlack 的值。 |
| [get_FinishText](./get_finishtext/) | 获取 FinishText 的值。 |
| [get_FinishVariance](./get_finishvariance/) | 获取 FinishVariance 的值。 |
| [get_FixedCost](./get_fixedcost/) | 获取 FixedCost 的值。 |
| [get_FixedCostAccrual](./get_fixedcostaccrual/) | 获取 FixedCostAccrual 的值。 |
| [get_FreeSlack](./get_freeslack/) | 获取 FreeSlack 的值。 |
| [get_Guid](./get_guid/) | 获取 Guid 的值。 |
| [get_HideBar](./get_hidebar/) | 获取指示 HideBar 是否已设置的值。 |
| [get_Hyperlink](./get_hyperlink/) | 获取与任务关联的超链接的标题或说明文本。 |
| [get_HyperlinkAddress](./get_hyperlinkaddress/) | 获取与任务关联的超链接的地址。 |
| [get_HyperlinkSubAddress](./get_hyperlinksubaddress/) | 获取与任务关联的超链接中文档的具体位置。 |
| [get_Id](./get_id/) | 获取 Id 的值。 |
| [get_IgnoreResourceCalendar](./get_ignoreresourcecalendar/) | 获取指示 IgnoreResourceCalendar 是否已设置的值。 |
| [get_IgnoreWarnings](./get_ignorewarnings/) | 获取指示 IgnoreWarnings 是否已设置的值。 |
| [get_IsActive](./get_isactive/) | 获取指示 IsActive 是否已设置的值。 |
| [get_IsCritical](./get_iscritical/) | 获取指示 IsCritical 是否已设置的值。 |
| [get_IsEffortDriven](./get_iseffortdriven/) | 获取指示 IsEffortDriven 是否已设置的值。 |
| [get_IsEstimated](./get_isestimated/) | 获取指示 IsEstimated 是否已设置的值。 |
| [get_IsExpanded](./get_isexpanded/) | 获取指示 IsExpanded 是否已设置的值。 |
| [get_IsExternalTask](./get_isexternaltask/) | 获取指示 IsExternalTask 是否已设置的值。 |
| [get_IsManual](./get_ismanual/) | 获取指示 IsManual 是否已设置的值。 |
| [get_IsMarked](./get_ismarked/) | 获取指示 IsMarked 是否已设置的值。 |
| [get_IsMilestone](./get_ismilestone/) | 获取指示 IsMilestone 是否已设置的值。 |
| [get_IsNull](./get_isnull/) | 获取指示是否设置了 IsNull 的值。 |
| [get_IsOverallocated](./get_isoverallocated/) | 获取指示 IsOverallocated 是否已设置的值。 |
| [get_IsPublished](./get_ispublished/) | 获取指示 IsPublished 是否已设置的值。 |
| [get_IsRecurring](./get_isrecurring/) | 获取指示 IsRecurring 是否已设置的值。 |
| [get_IsResumeValid](./get_isresumevalid/) | 获取指示 IsResumeValid 是否已设置的值。 |
| [get_IsRollup](./get_isrollup/) | 获取一个指示 IsRollup 是否已设置的值。 |
| [get_IsSubproject](./get_issubproject/) | 获取一个指示 IsSubproject 是否已设置的值。 |
| [get_IsSubprojectReadOnly](./get_issubprojectreadonly/) | 获取一个指示 IsSubprojectReadOnly 是否已设置的值。 |
| [get_IsSummary](./get_issummary/) | 获取一个指示 IsSummary 是否已设置的值。 |
| [get_LateFinish](./get_latefinish/) | 获取 LateFinish 的值。 |
| [get_LateStart](./get_latestart/) | 获取 LateStart 的值。 |
| [get_LevelAssignments](./get_levelassignments/) | 获取一个指示 LevelAssignments 是否已设置的值。 |
| [get_LevelingCanSplit](./get_levelingcansplit/) | 获取一个指示 LevelingCanSplit 是否已设置的值。 |
| [get_LevelingDelay](./get_levelingdelay/) | 获取 LevelingDelay 的值。 |
| [get_ManualDuration](./get_manualduration/) | 获取 ManualDuration 的值。 |
| [get_ManualFinish](./get_manualfinish/) | 获取 ManualFinish 的值。 |
| [get_ManualStart](./get_manualstart/) | 获取 ManualStart 的值。 |
| [get_Name](./get_name/) | 获取 Name 的值。 |
| [get_NotesRTF](./get_notesrtf/) | 获取 NotesRTF 的值。 |
| [get_NotesText](./get_notestext/) | 获取 NotesText 的值。 |
| [get_OutlineCodes](./get_outlinecodes/) | 获取 OutlineCodeCollection 对象。 |
| [get_OutlineLevel](./get_outlinelevel/) | 获取 OutlineLevel 的值。 |
| [get_OutlineNumber](./get_outlinenumber/) | 获取 OutlineNumber 的值。 |
| [get_OvertimeCost](./get_overtimecost/) | 获取 OvertimeCost 的值。 |
| [get_OvertimeWork](./get_overtimework/) | 获取 OvertimeWork 的值。 |
| [get_ParentProject](./get_parentproject/) | 获取任务的父项目。 |
| [get_ParentTask](./get_parenttask/) | 获取任务的父任务。 |
| [get_PercentComplete](./get_percentcomplete/) | 获取 PercentComplete 的值。 |
| [get_PercentWorkComplete](./get_percentworkcomplete/) | 获取 PercentWorkComplete 的值。 |
| [get_PhysicalPercentComplete](./get_physicalpercentcomplete/) | 获取 PhysicalPercentComplete 的值。 |
| [get_Predecessors](./get_predecessors/) | 获取一个 TaskCollection 对象，其中包含此 Task 对象的所有前置任务。 |
| [get_PreleveledFinish](./get_preleveledfinish/) | 获取 PreleveledFinish 的值。 |
| [get_PreleveledStart](./get_preleveledstart/) | 获取 PreleveledStart 的值。 |
| [get_PrimaveraProperties](./get_primaveraproperties/) | 获取一个对象，其中包含从 Primavera 文件读取的任务的 Primavera 特定属性。 |
| [get_Priority](./get_priority/) | 获取 Priority 的值。 |
| [get_RecurringInfo](./get_recurringinfo/) | 获取任务的 RecurringTaskInfo 类实例（该任务为循环任务）；如果任务不是循环任务，则返回 null； |
| [get_RegularWork](./get_regularwork/) | 获取 RegularWork 的值。 |
| [get_RemainingCost](./get_remainingcost/) | 获取 RemainingCost 的值。 |
| [get_RemainingDuration](./get_remainingduration/) | 获取 RemainingDuration 的值。 |
| [get_RemainingOvertimeCost](./get_remainingovertimecost/) | 获取 RemainingOvertimeCost 的值。 |
| [get_RemainingOvertimeWork](./get_remainingovertimework/) | 获取 RemainingOvertimeWork 的值。 |
| [get_RemainingWork](./get_remainingwork/) | 获取 RemainingWork 的值。 |
| [get_Resume](./get_resume/) | 获取 Resume 的值。 |
| [get_SplitParts](./get_splitparts/) | 获取一个 SplitPart 集合，表示任务的各个部分。 |
| [get_Start](./get_start/) | 获取 Start 的值。 |
| [get_StartSlack](./get_startslack/) | 获取 StartSlack 的值。 |
| [get_StartText](./get_starttext/) | 获取 StartText 的值。 |
| [get_StartVariance](./get_startvariance/) | 获取 StartVariance 的值。 |
| [get_Status](./get_status/) | 获取任务状态。 |
| [get_StatusManager](./get_statusmanager/) | 获取 StatusManager 的值。 |
| [get_Stop](./get_stop/) | 获取 Stop 的值。 |
| [get_SubprojectName](./get_subprojectname/) | 获取 SubprojectName 的值。 |
| [get_Successors](./get_successors/) | 获取一个 TaskCollection 对象，其中包含此 Task 对象的所有后继任务。 |
| [get_SV](./get_sv/) | 截至项目状态日期的挣值进度偏差。进度偏差（SV）是 BCWP 与 BCWS 之间的差异。 |
| [get_TimephasedData](./get_timephaseddata/) | 获取此任务的 TimephasedDataCollection 对象。与任务关联的时间分段数据块。 |
| [get_TotalSlack](./get_totalslack/) | 获取 TotalSlack 的值。 |
| [get_Type](./get_type/) | 获取 Type 的值。 |
| [get_Uid](./get_uid/) | 获取 Uid 的值。 |
| [get_Warning](./get_warning/) | 获取一个值，指示是否已设置 Warning。 |
| [get_WBS](./get_wbs/) | 获取 WBS 的值。 |
| [get_WBSLevel](./get_wbslevel/) | 获取 WBSLevel 的值。 |
| [get_Work](./get_work/) | 获取 Work 的值。 |
| [get_WorkVariance](./get_workvariance/) | 获取 WorkVariance 的值。 |
| [GetHashCode](./gethashcode/) | 返回此 Task 的哈希码值。 |
| [GetTimephasedData (2 overloads)](./gettimephaseddata/) | 返回一个 TimephasedDataCollection 对象，其中包含给定开始和结束日期范围内的 TimephasedData 值。 |
| [MoveToSibling (2 overloads)](./movetosibling/) | 将当前任务在相同的大纲级别上移动到指定任务之前。若 ParentProject.CalculationMode 为 None，用户应在使用此方法后调用 Project.Recalculate()（它将重新安排所有项目任务（开始/结束日期，设置早/晚日期）并计算诸如时差、工作和成本字段、以及大纲级别等依赖字段）。若 ParentProject.CalculationMode 为 Manual，方法仅自动计算任务 ID、大纲级别和大纲编号。若 ParentProject.CalculationMode 为 Automatic，方法会自动重新安排整个项目的任务（开始/结束日期，设置早/晚日期，计算时差、工作和成本字段，重新计算 ID 和大纲级别）。 |
| [OutlineIndent](./outlineindent/) | 在大纲中缩进任务。 |
| [OutlineOutdent](./outlineoutdent/) | 在大纲中提升任务。 |
| [SelectAllChildTasks](./selectallchildtasks/) | 递归收集此任务的所有子任务。 |
| [Set](./set/) | 将指定属性映射到此容器中的指定值。 |
| [set_ActivityId](./set_activityid/) | 表示活动 ID 字段——Primavera 使用的任务唯一标识符。（仅适用于 Primavera 项目） |
| [set_ActualCost](./set_actualcost/) | 设置 ActualCost 的值。 |
| [set_ActualDuration](./set_actualduration/) | 设置 ActualDuration 的值。 |
| [set_ActualFinish](./set_actualfinish/) | 设置 ActualFinish 的值。 |
| [set_ActualOvertimeCost](./set_actualovertimecost/) | 设置 ActualOvertimeCost 的值。 |
| [set_ActualOvertimeWork](./set_actualovertimework/) | 设置 ActualOvertimeWork 的值。 |
| [set_ActualOvertimeWorkProtected](./set_actualovertimeworkprotected/) | 设置 ActualOvertimeWorkProtected 的值。 |
| [set_ActualStart](./set_actualstart/) | 设置 ActualStart 的值。 |
| [set_ActualWork](./set_actualwork/) | 设置 ActualWork 的值。 |
| [set_ActualWorkProtected](./set_actualworkprotected/) | 设置 ActualWorkProtected 的值。 |
| [set_ACWP](./set_acwp/) | 设置 ACWP 的值。 |
| [set_Baselines](./set_baselines/) | 设置任务的基线值集合。 |
| [set_BCWP](./set_bcwp/) | 设置 BCWP 的值。 |
| [set_BCWS](./set_bcws/) | 设置 BCWS 的值。 |
| [set_BudgetCost](./set_budgetcost/) | 设置 BudgetCost 的值。 |
| [set_BudgetWork](./set_budgetwork/) | 设置 BudgetWork 的值。 |
| [set_Calendar](./set_calendar/) | 设置 Calendar 的值。 |
| [set_CommitmentFinish](./set_commitmentfinish/) | 设置 CommitmentFinish 的值。 |
| [set_CommitmentStart](./set_commitmentstart/) | 设置 CommitmentStart 的值。 |
| [set_CommitmentType](./set_commitmenttype/) | 设置 CommitmentType 的值。 |
| [set_ConstraintDate](./set_constraintdate/) | 设置 ConstraintDate 的值。 |
| [set_ConstraintType](./set_constrainttype/) | 设置 ConstraintType 的值。 |
| [set_Contact](./set_contact/) | 设置 Contact 的值。 |
| [set_Cost](./set_cost/) | 设置 Cost 的值。 |
| [set_CostVariance](./set_costvariance/) | 设置 CostVariance 的值。 |
| [set_Created](./set_created/) | 设置 Created 的值。 |
| [set_CV](./set_cv/) | 设置 CV 的值。 |
| [set_Deadline](./set_deadline/) | 设置 Deadline 的值。 |
| [set_DisplayAsSummary](./set_displayassummary/) | 设置一个值，指示 DisplayAsSummary 是否已设置。 |
| [set_DisplayOnTimeline](./set_displayontimeline/) | 设置一个值，指示 DisplayOnTimeline 是否已设置。 |
| [set_Duration](./set_duration/) | 设置 Duration 的值。 |
| [set_DurationFormat](./set_durationformat/) | 设置 DurationFormat 的值。 |
| [set_DurationText](./set_durationtext/) | 设置 DurationText 的值。 |
| [set_DurationVariance](./set_durationvariance/) | 设置 DurationVariance 的值。 |
| [set_EarlyFinish](./set_earlyfinish/) | 设置 EarlyFinish 的值。 |
| [set_EarlyStart](./set_earlystart/) | 设置 EarlyStart 的值。 |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | 设置 EarnedValueMethod 的值。 |
| [set_ExternalId](./set_externalid/) | 设置 ExternalId 的值。 |
| [set_ExternalTaskProject](./set_externaltaskproject/) | 设置 ExternalTaskProject 的值。 |
| [set_ExternalUid](./set_externaluid/) | 获取或设置外部任务为外部时的唯一标识符。 |
| [set_Finish](./set_finish/) | 设置 Finish 的值。 |
| [set_FinishSlack](./set_finishslack/) | 设置 FinishSlack 的值。 |
| [set_FinishText](./set_finishtext/) | 设置 FinishText 的值。 |
| [set_FinishVariance](./set_finishvariance/) | 设置 FinishVariance 的值。 |
| [set_FixedCost](./set_fixedcost/) | 设置 FixedCost 的值。 |
| [set_FixedCostAccrual](./set_fixedcostaccrual/) | 设置 FixedCostAccrual 的值。 |
| [set_FreeSlack](./set_freeslack/) | 设置 FreeSlack 的值。 |
| [set_Guid](./set_guid/) | 设置 Guid 的值。 |
| [set_HideBar](./set_hidebar/) | 设置一个值，指示 HideBar 是否已设置。 |
| [set_Hyperlink](./set_hyperlink/) | 设置与任务关联的超链接的标题或说明文本。 |
| [set_HyperlinkAddress](./set_hyperlinkaddress/) | 设置与任务关联的超链接的地址。 |
| [set_HyperlinkSubAddress](./set_hyperlinksubaddress/) | 设置与任务关联的超链接在文档中的具体位置。 |
| [set_Id](./set_id/) | 设置 Id 的值。 |
| [set_IgnoreResourceCalendar](./set_ignoreresourcecalendar/) | 设置一个值，指示 IgnoreResourceCalendar 是否已设置。 |
| [set_IgnoreWarnings](./set_ignorewarnings/) | 设置一个值，指示 IgnoreWarnings 是否已设置。 |
| [set_IsActive](./set_isactive/) | 设置一个值，指示 IsActive 是否已设置。 |
| [set_IsCritical](./set_iscritical/) | 设置一个值，指示 IsCritical 是否已设置。 |
| [set_IsEffortDriven](./set_iseffortdriven/) | 设置一个值，指示 IsEffortDriven 是否已设置。 |
| [set_IsEstimated](./set_isestimated/) | 设置一个值，指示 IsEstimated 是否已设置。 |
| [set_IsExpanded](./set_isexpanded/) | 设置一个值，指示 IsExpanded 是否已设置。 |
| [set_IsExternalTask](./set_isexternaltask/) | 设置一个值，指示 IsExternalTask 是否已设置。 |
| [set_IsManual](./set_ismanual/) | 设置一个值，指示 IsManual 是否已设置。 |
| [set_IsMarked](./set_ismarked/) | 设置一个值，指示 IsMarked 是否已设置。 |
| [set_IsMilestone](./set_ismilestone/) | 设置一个值，指示 IsMilestone 是否已设置。 |
| [set_IsNull](./set_isnull/) | 设置指示 IsNull 是否已设置的值。 |
| [set_IsOverallocated](./set_isoverallocated/) | 设置一个值，指示 IsOverallocated 是否已设置。 |
| [set_IsPublished](./set_ispublished/) | 设置一个值，指示 IsPublished 是否已设置。 |
| [set_IsRecurring](./set_isrecurring/) | 设置一个值，指示 IsRecurring 是否已设置。 |
| [set_IsResumeValid](./set_isresumevalid/) | 设置一个值，指示 IsResumeValid 是否已设置。 |
| [set_IsRollup](./set_isrollup/) | 设置一个值，指示 IsRollup 是否已设置。 |
| [set_IsSubproject](./set_issubproject/) | 设置一个值，指示 IsSubproject 是否已设置。 |
| [set_IsSubprojectReadOnly](./set_issubprojectreadonly/) | 设置一个值，指示 IsSubprojectReadOnly 是否已设置。 |
| [set_IsSummary](./set_issummary/) | 设置一个值，指示 IsSummary 是否已设置。 |
| [set_LateFinish](./set_latefinish/) | 设置 LateFinish 的值。 |
| [set_LateStart](./set_latestart/) | 设置 LateStart 的值。 |
| [set_LevelAssignments](./set_levelassignments/) | 设置一个值，指示 LevelAssignments 是否已设置。 |
| [set_LevelingCanSplit](./set_levelingcansplit/) | 设置一个值，指示 LevelingCanSplit 是否已设置。 |
| [set_LevelingDelay](./set_levelingdelay/) | 设置 LevelingDelay 的值。 |
| [set_ManualDuration](./set_manualduration/) | 设置 ManualDuration 的值。 |
| [set_ManualFinish](./set_manualfinish/) | 设置 ManualFinish 的值。 |
| [set_ManualStart](./set_manualstart/) | 设置 ManualStart 的值。 |
| [set_Name](./set_name/) | 设置 Name 的值。 |
| [set_NotesRTF](./set_notesrtf/) | 设置 NotesRTF 的值。 |
| [set_NotesText](./set_notestext/) | 设置 NotesText 的值。 |
| [set_OutlineCodes](./set_outlinecodes/) | 设置 OutlineCodeCollection 对象。 |
| [set_OutlineLevel](./set_outlinelevel/) | 设置 OutlineLevel 的值。 |
| [set_OutlineNumber](./set_outlinenumber/) | 设置 OutlineNumber 的值。 |
| [set_OvertimeCost](./set_overtimecost/) | 设置 OvertimeCost 的值。 |
| [set_OvertimeWork](./set_overtimework/) | 设置 OvertimeWork 的值。 |
| [set_PercentComplete](./set_percentcomplete/) | 设置 PercentComplete 的值。 |
| [set_PercentWorkComplete](./set_percentworkcomplete/) | 设置 PercentWorkComplete 的值。 |
| [set_PhysicalPercentComplete](./set_physicalpercentcomplete/) | 设置 PhysicalPercentComplete 的值。 |
| [set_PreleveledFinish](./set_preleveledfinish/) | 设置 PreleveledFinish 的值。 |
| [set_PreleveledStart](./set_preleveledstart/) | 设置 PreleveledStart 的值。 |
| [set_Priority](./set_priority/) | 设置 Priority 的值。 |
| [set_RegularWork](./set_regularwork/) | 设置 RegularWork 的值。 |
| [set_RemainingCost](./set_remainingcost/) | 设置 RemainingCost 的值。 |
| [set_RemainingDuration](./set_remainingduration/) | 设置 RemainingDuration 的值。 |
| [set_RemainingOvertimeCost](./set_remainingovertimecost/) | 设置 RemainingOvertimeCost 的值。 |
| [set_RemainingOvertimeWork](./set_remainingovertimework/) | 设置 RemainingOvertimeWork 的值。 |
| [set_RemainingWork](./set_remainingwork/) | 设置 RemainingWork 的值。 |
| [set_Resume](./set_resume/) | 设置 Resume 的值。 |
| [set_Start](./set_start/) | 设置 Start 的值。 |
| [set_StartSlack](./set_startslack/) | 设置 StartSlack 的值。 |
| [set_StartText](./set_starttext/) | 设置 StartText 的值。 |
| [set_StartVariance](./set_startvariance/) | 设置 StartVariance 的值。 |
| [set_StatusManager](./set_statusmanager/) | 设置 StatusManager 的值。 |
| [set_Stop](./set_stop/) | 设置 Stop 的值。 |
| [set_SubprojectName](./set_subprojectname/) | 设置 SubprojectName 的值。 |
| [set_SV](./set_sv/) | 截至项目状态日期的挣值进度偏差。进度偏差（SV）是 BCWP 与 BCWS 之间的差异。 |
| [set_TimephasedData](./set_timephaseddata/) | 设置此任务的 TimephasedDataCollection 对象。与任务关联的时间分段数据块。 |
| [set_TotalSlack](./set_totalslack/) | 设置 TotalSlack 的值。 |
| [set_Type](./set_type/) | 设置 Type 的值。 |
| [set_Uid](./set_uid/) | 设置 Uid 的值。 |
| [set_Warning](./set_warning/) | 设置一个值，指示 Warning 是否已设置。 |
| [set_WBS](./set_wbs/) | 设置 WBS 的值。 |
| [set_WBSLevel](./set_wbslevel/) | 设置 WBSLevel 的值。 |
| [set_Work](./set_work/) | 设置 Work 的值。 |
| [set_WorkVariance](./set_workvariance/) | 设置 WorkVariance 的值。 |
| [ToString](./tostring/) | 返回任务的简短字符串表示。表示的具体细节未指定，可能会更改。 |

