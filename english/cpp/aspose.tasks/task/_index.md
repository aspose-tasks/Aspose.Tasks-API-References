---
title: "Aspose::Tasks::Task class"
linktitle: "Task"
articleTitle: "Task"
second_title: "Aspose.Tasks for C++"
description: "Represents a task in a project."
type: docs
weight: 10
url: /cpp/aspose.tasks/task/
---

## Task class

**Inherits:** Aspose::Tasks::IEntityWithTd

Represents a task in a project.

The Task is representing a one atomic chunk of work.

One can use Task to plan a project by creating tasks and assign appropriate resources onto them. Tasks in a project are organized as a rooted hierarchical tree structure, with a root task and subtrees of children tasks.

To build a tree of tasks one can use a specialized collection Aspose::Tasks::TaskCollection by accessing Project::RootTask property e.g.:

```cpp
Project project = new Project();
 
// add new tasks
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
 
// save project in the one of available formats
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

## Methods

| Name | Description |
| --- | --- |
| [Clone](./clone/) | Creates full copy of a task without subtasks. |
| [Delete](./delete/) | Deletes a task from parent project tasks collection and all its assignments. |
| [Equals (2 overloads)](./equals/) | Returns a value indicating whether this instance is equal to a specified object. |
| [Get](./get/) | Returns the value to which the property is mapped in this container. |
| [get_ActivityId](./get_activityid/) | Represents activity id field - a task's unique identifier used by Primavera. (only applicable to Primavera projects). |
| [get_ActualCost](./get_actualcost/) | Gets a value of ActualCost. |
| [get_ActualDuration](./get_actualduration/) | Gets a value of ActualDuration. |
| [get_ActualFinish](./get_actualfinish/) | Gets a value of ActualFinish. |
| [get_ActualOvertimeCost](./get_actualovertimecost/) | Gets a value of ActualOvertimeCost. |
| [get_ActualOvertimeWork](./get_actualovertimework/) | Gets a value of ActualOvertimeWork. |
| [get_ActualOvertimeWorkProtected](./get_actualovertimeworkprotected/) | Gets a value of ActualOvertimeWorkProtected. |
| [get_ActualStart](./get_actualstart/) | Gets a value of ActualStart. |
| [get_ActualWork](./get_actualwork/) | Gets a value of ActualWork. |
| [get_ActualWorkProtected](./get_actualworkprotected/) | Gets a value of ActualWorkProtected. |
| [get_ACWP](./get_acwp/) | Gets a value of ACWP. |
| [get_Assignments](./get_assignments/) | Gets a collection of resource assignments for this object. |
| [get_Baselines](./get_baselines/) | Gets the collection of baseline values of the task. |
| [get_BCWP](./get_bcwp/) | Gets a value of BCWP. |
| [get_BCWS](./get_bcws/) | Gets a value of BCWS. |
| [get_BudgetCost](./get_budgetcost/) | Gets a value of BudgetCost. |
| [get_BudgetWork](./get_budgetwork/) | Gets a value of BudgetWork. |
| [get_Calendar](./get_calendar/) | Gets a value of Calendar . |
| [get_Children](./get_children/) | Gets a child task collection of this object. TaskCollection object which represents children tasks. |
| [get_CommitmentFinish](./get_commitmentfinish/) | Gets a value of CommitmentFinish. |
| [get_CommitmentStart](./get_commitmentstart/) | Gets a value of CommitmentStart. |
| [get_CommitmentType](./get_commitmenttype/) | Gets a value of CommitmentType. |
| [get_ConstraintDate](./get_constraintdate/) | Gets a value of ConstraintDate. |
| [get_ConstraintType](./get_constrainttype/) | Gets a value of ConstraintType. |
| [get_Contact](./get_contact/) | Gets a value of Contact. |
| [get_Cost](./get_cost/) | Gets a value of Cost. |
| [get_CostVariance](./get_costvariance/) | Gets a value of CostVariance. |
| [get_Created](./get_created/) | Gets a value of Created. |
| [get_CV](./get_cv/) | Gets a value of CV. |
| [get_Deadline](./get_deadline/) | Gets a value of Deadline. |
| [get_DisplayAsSummary](./get_displayassummary/) | Gets a value indicating whether DisplayAsSummary is set or not. |
| [get_DisplayOnTimeline](./get_displayontimeline/) | Gets a value indicating whether DisplayOnTimeline is set or not. |
| [get_Duration](./get_duration/) | Gets a value of Duration . |
| [get_DurationFormat](./get_durationformat/) | Gets a value of DurationFormat. |
| [get_DurationText](./get_durationtext/) | Gets a value of DurationText. |
| [get_DurationVariance](./get_durationvariance/) | Gets a value of DurationVariance. |
| [get_EarlyFinish](./get_earlyfinish/) | Gets a value of EarlyFinish. |
| [get_EarlyStart](./get_earlystart/) | Gets a value of EarlyStart. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | Gets a value of EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | Gets ExtendedAttributeCollection object containing the values of an extended attribute. |
| [get_ExternalId](./get_externalid/) | Gets a value of ExternalId. |
| [get_ExternalTaskProject](./get_externaltaskproject/) | Gets a value of ExternalTaskProject. |
| [get_ExternalUid](./get_externaluid/) | Gets or set the external task's Unique identifier when the task is external. |
| [get_Finish](./get_finish/) | Gets a value of Finish. |
| [get_FinishSlack](./get_finishslack/) | Gets a value of FinishSlack. |
| [get_FinishText](./get_finishtext/) | Gets a value of FinishText. |
| [get_FinishVariance](./get_finishvariance/) | Gets a value of FinishVariance. |
| [get_FixedCost](./get_fixedcost/) | Gets a value of FixedCost. |
| [get_FixedCostAccrual](./get_fixedcostaccrual/) | Gets a value of FixedCostAccrual. |
| [get_FreeSlack](./get_freeslack/) | Gets a value of FreeSlack. |
| [get_Guid](./get_guid/) | Gets a value of Guid. |
| [get_HideBar](./get_hidebar/) | Gets a value indicating whether HideBar is set or not. |
| [get_Hyperlink](./get_hyperlink/) | Gets the title or explanatory text for a hyperlink associated with a task. |
| [get_HyperlinkAddress](./get_hyperlinkaddress/) | Gets the address for a hyperlink associated with a task. |
| [get_HyperlinkSubAddress](./get_hyperlinksubaddress/) | Gets the specific location in a document in a hyperlink associated with a task. |
| [get_Id](./get_id/) | Gets a value of Id. |
| [get_IgnoreResourceCalendar](./get_ignoreresourcecalendar/) | Gets a value indicating whether IgnoreResourceCalendar is set or not. |
| [get_IgnoreWarnings](./get_ignorewarnings/) | Gets a value indicating whether IgnoreWarnings is set or not. |
| [get_IsActive](./get_isactive/) | Gets a value indicating whether IsActive is set or not. |
| [get_IsCritical](./get_iscritical/) | Gets a value indicating whether IsCritical is set or not. |
| [get_IsEffortDriven](./get_iseffortdriven/) | Gets a value indicating whether IsEffortDriven is set or not. |
| [get_IsEstimated](./get_isestimated/) | Gets a value indicating whether IsEstimated is set or not. |
| [get_IsExpanded](./get_isexpanded/) | Gets a value indicating whether IsExpanded is set or not. |
| [get_IsExternalTask](./get_isexternaltask/) | Gets a value indicating whether IsExternalTask is set or not. |
| [get_IsManual](./get_ismanual/) | Gets a value indicating whether IsManual is set or not. |
| [get_IsMarked](./get_ismarked/) | Gets a value indicating whether IsMarked is set or not. |
| [get_IsMilestone](./get_ismilestone/) | Gets a value indicating whether IsMilestone is set or not. |
| [get_IsNull](./get_isnull/) | Gets a value indicating whether IsNull is set or not. |
| [get_IsOverallocated](./get_isoverallocated/) | Gets a value indicating whether IsOverallocated is set or not. |
| [get_IsPublished](./get_ispublished/) | Gets a value indicating whether IsPublished is set or not. |
| [get_IsRecurring](./get_isrecurring/) | Gets a value indicating whether IsRecurring is set or not. |
| [get_IsResumeValid](./get_isresumevalid/) | Gets a value indicating whether IsResumeValid is set or not. |
| [get_IsRollup](./get_isrollup/) | Gets a value indicating whether IsRollup is set or not. |
| [get_IsSubproject](./get_issubproject/) | Gets a value indicating whether IsSubproject is set or not. |
| [get_IsSubprojectReadOnly](./get_issubprojectreadonly/) | Gets a value indicating whether IsSubprojectReadOnly is set or not. |
| [get_IsSummary](./get_issummary/) | Gets a value indicating whether IsSummary is set or not. |
| [get_LateFinish](./get_latefinish/) | Gets a value of LateFinish. |
| [get_LateStart](./get_latestart/) | Gets a value of LateStart. |
| [get_LevelAssignments](./get_levelassignments/) | Gets a value indicating whether LevelAssignments is set or not. |
| [get_LevelingCanSplit](./get_levelingcansplit/) | Gets a value indicating whether LevelingCanSplit is set or not. |
| [get_LevelingDelay](./get_levelingdelay/) | Gets a value of LevelingDelay. |
| [get_ManualDuration](./get_manualduration/) | Gets a value of ManualDuration. |
| [get_ManualFinish](./get_manualfinish/) | Gets a value of ManualFinish. |
| [get_ManualStart](./get_manualstart/) | Gets a value of ManualStart. |
| [get_Name](./get_name/) | Gets a value of Name. |
| [get_NotesRTF](./get_notesrtf/) | Gets a value of NotesRTF. |
| [get_NotesText](./get_notestext/) | Gets a value of NotesText. |
| [get_OutlineCodes](./get_outlinecodes/) | Gets OutlineCodeCollection object. |
| [get_OutlineLevel](./get_outlinelevel/) | Gets a value of OutlineLevel. |
| [get_OutlineNumber](./get_outlinenumber/) | Gets a value of OutlineNumber. |
| [get_OvertimeCost](./get_overtimecost/) | Gets a value of OvertimeCost. |
| [get_OvertimeWork](./get_overtimework/) | Gets a value of OvertimeWork. |
| [get_ParentProject](./get_parentproject/) | Gets the parent project of a task. |
| [get_ParentTask](./get_parenttask/) | Gets the parent task of a task. |
| [get_PercentComplete](./get_percentcomplete/) | Gets a value of PercentComplete. |
| [get_PercentWorkComplete](./get_percentworkcomplete/) | Gets a value of PercentWorkComplete. |
| [get_PhysicalPercentComplete](./get_physicalpercentcomplete/) | Gets a value of PhysicalPercentComplete. |
| [get_Predecessors](./get_predecessors/) | Gets a TaskCollection object which contains all predecessors of this Task object. |
| [get_PreleveledFinish](./get_preleveledfinish/) | Gets a value of PreleveledFinish. |
| [get_PreleveledStart](./get_preleveledstart/) | Gets a value of PreleveledStart. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Gets an object containing Primavera-specific properties for a task read from Primavera file. |
| [get_Priority](./get_priority/) | Gets a value of Priority. |
| [get_RecurringInfo](./get_recurringinfo/) | Gets the instance of RecurringTaskInfo class for the task which is a recurring task; if the task is not a recurring one then returns null; |
| [get_RegularWork](./get_regularwork/) | Gets a value of RegularWork. |
| [get_RemainingCost](./get_remainingcost/) | Gets a value of RemainingCost. |
| [get_RemainingDuration](./get_remainingduration/) | Gets a value of RemainingDuration. |
| [get_RemainingOvertimeCost](./get_remainingovertimecost/) | Gets a value of RemainingOvertimeCost. |
| [get_RemainingOvertimeWork](./get_remainingovertimework/) | Gets a value of RemainingOvertimeWork. |
| [get_RemainingWork](./get_remainingwork/) | Gets a value of RemainingWork. |
| [get_Resume](./get_resume/) | Gets a value of Resume. |
| [get_SplitParts](./get_splitparts/) | Gets a SplitPart collection that represents the portions of a task. |
| [get_Start](./get_start/) | Gets a value of Start. |
| [get_StartSlack](./get_startslack/) | Gets a value of StartSlack. |
| [get_StartText](./get_starttext/) | Gets a value of StartText. |
| [get_StartVariance](./get_startvariance/) | Gets a value of StartVariance. |
| [get_Status](./get_status/) | Gets task status. |
| [get_StatusManager](./get_statusmanager/) | Gets a value of StatusManager. |
| [get_Stop](./get_stop/) | Gets a value of Stop. |
| [get_SubprojectName](./get_subprojectname/) | Gets a value of SubprojectName. |
| [get_Successors](./get_successors/) | Gets a TaskCollection object which contains all successors of this Task object. |
| [get_SV](./get_sv/) | The earned value schedule variance, through the project status date. Schedule variance (SV) is the difference between the BCWP and the BCWS. |
| [get_TimephasedData](./get_timephaseddata/) | Gets a TimephasedDataCollection object of this task. The time phased data block associated with a task. |
| [get_TotalSlack](./get_totalslack/) | Gets a value of TotalSlack. |
| [get_Type](./get_type/) | Gets a value of Type. |
| [get_Uid](./get_uid/) | Gets a value of Uid. |
| [get_Warning](./get_warning/) | Gets a value indicating whether Warning is set or not. |
| [get_WBS](./get_wbs/) | Gets a value of WBS. |
| [get_WBSLevel](./get_wbslevel/) | Gets a value of WBSLevel. |
| [get_Work](./get_work/) | Gets a value of Work. |
| [get_WorkVariance](./get_workvariance/) | Gets a value of WorkVariance. |
| [GetHashCode](./gethashcode/) | Returns a hash code value for this Task . |
| [GetTimephasedData (2 overloads)](./gettimephaseddata/) | Returns TimephasedDataCollection object with TimephasedData values within given start and end dates. |
| [MoveToSibling (2 overloads)](./movetosibling/) | Moves the current task at the same Outline Level before the specified task. If ParentProject.CalculationMode is None user should invoke Project.Recalculate() after using this method (It will reschedule all project tasks (start/finish dates, sets early/late dates) and calculate the dependent fields such as slacks, work and cost fields, outline levels). If ParentProject.CalculationMode is Manual the method will calculate only task id, outline level and outline numbers automatically. If ParentProject.CalculationMode is Automatic the method reschedules all project's tasks automatically (start/finish dates, sets early/late dates, calculates slacks, work and cost fields, recalculates ids and outline levels). |
| [OutlineIndent](./outlineindent/) | Indents a task in the outline. |
| [OutlineOutdent](./outlineoutdent/) | Promotes a task in the outline. |
| [SelectAllChildTasks](./selectallchildtasks/) | Recursively collects all child tasks of this task. |
| [Set](./set/) | Maps the specified property to the specified value in this container. |
| [set_ActivityId](./set_activityid/) | Represents activity id field - a task's unique identifier used by Primavera. (only applicable to Primavera projects). |
| [set_ActualCost](./set_actualcost/) | Sets a value of ActualCost. |
| [set_ActualDuration](./set_actualduration/) | Sets a value of ActualDuration. |
| [set_ActualFinish](./set_actualfinish/) | Sets a value of ActualFinish. |
| [set_ActualOvertimeCost](./set_actualovertimecost/) | Sets a value of ActualOvertimeCost. |
| [set_ActualOvertimeWork](./set_actualovertimework/) | Sets a value of ActualOvertimeWork. |
| [set_ActualOvertimeWorkProtected](./set_actualovertimeworkprotected/) | Sets a value of ActualOvertimeWorkProtected. |
| [set_ActualStart](./set_actualstart/) | Sets a value of ActualStart. |
| [set_ActualWork](./set_actualwork/) | Sets a value of ActualWork. |
| [set_ActualWorkProtected](./set_actualworkprotected/) | Sets a value of ActualWorkProtected. |
| [set_ACWP](./set_acwp/) | Sets a value of ACWP. |
| [set_Baselines](./set_baselines/) | Sets the collection of baseline values of the task. |
| [set_BCWP](./set_bcwp/) | Sets a value of BCWP. |
| [set_BCWS](./set_bcws/) | Sets a value of BCWS. |
| [set_BudgetCost](./set_budgetcost/) | Sets a value of BudgetCost. |
| [set_BudgetWork](./set_budgetwork/) | Sets a value of BudgetWork. |
| [set_Calendar](./set_calendar/) | Sets a value of Calendar . |
| [set_CommitmentFinish](./set_commitmentfinish/) | Sets a value of CommitmentFinish. |
| [set_CommitmentStart](./set_commitmentstart/) | Sets a value of CommitmentStart. |
| [set_CommitmentType](./set_commitmenttype/) | Sets a value of CommitmentType. |
| [set_ConstraintDate](./set_constraintdate/) | Sets a value of ConstraintDate. |
| [set_ConstraintType](./set_constrainttype/) | Sets a value of ConstraintType. |
| [set_Contact](./set_contact/) | Sets a value of Contact. |
| [set_Cost](./set_cost/) | Sets a value of Cost. |
| [set_CostVariance](./set_costvariance/) | Sets a value of CostVariance. |
| [set_Created](./set_created/) | Sets a value of Created. |
| [set_CV](./set_cv/) | Sets a value of CV. |
| [set_Deadline](./set_deadline/) | Sets a value of Deadline. |
| [set_DisplayAsSummary](./set_displayassummary/) | Sets a value indicating whether DisplayAsSummary is set or not. |
| [set_DisplayOnTimeline](./set_displayontimeline/) | Sets a value indicating whether DisplayOnTimeline is set or not. |
| [set_Duration](./set_duration/) | Sets a value of Duration . |
| [set_DurationFormat](./set_durationformat/) | Sets a value of DurationFormat. |
| [set_DurationText](./set_durationtext/) | Sets a value of DurationText. |
| [set_DurationVariance](./set_durationvariance/) | Sets a value of DurationVariance. |
| [set_EarlyFinish](./set_earlyfinish/) | Sets a value of EarlyFinish. |
| [set_EarlyStart](./set_earlystart/) | Sets a value of EarlyStart. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | Sets a value of EarnedValueMethod. |
| [set_ExternalId](./set_externalid/) | Sets a value of ExternalId. |
| [set_ExternalTaskProject](./set_externaltaskproject/) | Sets a value of ExternalTaskProject. |
| [set_ExternalUid](./set_externaluid/) | Gets or set the external task's Unique identifier when the task is external. |
| [set_Finish](./set_finish/) | Sets a value of Finish. |
| [set_FinishSlack](./set_finishslack/) | Sets a value of FinishSlack. |
| [set_FinishText](./set_finishtext/) | Sets a value of FinishText. |
| [set_FinishVariance](./set_finishvariance/) | Sets a value of FinishVariance. |
| [set_FixedCost](./set_fixedcost/) | Sets a value of FixedCost. |
| [set_FixedCostAccrual](./set_fixedcostaccrual/) | Sets a value of FixedCostAccrual. |
| [set_FreeSlack](./set_freeslack/) | Sets a value of FreeSlack. |
| [set_Guid](./set_guid/) | Sets a value of Guid. |
| [set_HideBar](./set_hidebar/) | Sets a value indicating whether HideBar is set or not. |
| [set_Hyperlink](./set_hyperlink/) | Sets the title or explanatory text for a hyperlink associated with a task. |
| [set_HyperlinkAddress](./set_hyperlinkaddress/) | Sets the address for a hyperlink associated with a task. |
| [set_HyperlinkSubAddress](./set_hyperlinksubaddress/) | Sets the specific location in a document in a hyperlink associated with a task. |
| [set_Id](./set_id/) | Sets a value of Id. |
| [set_IgnoreResourceCalendar](./set_ignoreresourcecalendar/) | Sets a value indicating whether IgnoreResourceCalendar is set or not. |
| [set_IgnoreWarnings](./set_ignorewarnings/) | Sets a value indicating whether IgnoreWarnings is set or not. |
| [set_IsActive](./set_isactive/) | Sets a value indicating whether IsActive is set or not. |
| [set_IsCritical](./set_iscritical/) | Sets a value indicating whether IsCritical is set or not. |
| [set_IsEffortDriven](./set_iseffortdriven/) | Sets a value indicating whether IsEffortDriven is set or not. |
| [set_IsEstimated](./set_isestimated/) | Sets a value indicating whether IsEstimated is set or not. |
| [set_IsExpanded](./set_isexpanded/) | Sets a value indicating whether IsExpanded is set or not. |
| [set_IsExternalTask](./set_isexternaltask/) | Sets a value indicating whether IsExternalTask is set or not. |
| [set_IsManual](./set_ismanual/) | Sets a value indicating whether IsManual is set or not. |
| [set_IsMarked](./set_ismarked/) | Sets a value indicating whether IsMarked is set or not. |
| [set_IsMilestone](./set_ismilestone/) | Sets a value indicating whether IsMilestone is set or not. |
| [set_IsNull](./set_isnull/) | Sets a value indicating whether IsNull is set or not. |
| [set_IsOverallocated](./set_isoverallocated/) | Sets a value indicating whether IsOverallocated is set or not. |
| [set_IsPublished](./set_ispublished/) | Sets a value indicating whether IsPublished is set or not. |
| [set_IsRecurring](./set_isrecurring/) | Sets a value indicating whether IsRecurring is set or not. |
| [set_IsResumeValid](./set_isresumevalid/) | Sets a value indicating whether IsResumeValid is set or not. |
| [set_IsRollup](./set_isrollup/) | Sets a value indicating whether IsRollup is set or not. |
| [set_IsSubproject](./set_issubproject/) | Sets a value indicating whether IsSubproject is set or not. |
| [set_IsSubprojectReadOnly](./set_issubprojectreadonly/) | Sets a value indicating whether IsSubprojectReadOnly is set or not. |
| [set_IsSummary](./set_issummary/) | Sets a value indicating whether IsSummary is set or not. |
| [set_LateFinish](./set_latefinish/) | Sets a value of LateFinish. |
| [set_LateStart](./set_latestart/) | Sets a value of LateStart. |
| [set_LevelAssignments](./set_levelassignments/) | Sets a value indicating whether LevelAssignments is set or not. |
| [set_LevelingCanSplit](./set_levelingcansplit/) | Sets a value indicating whether LevelingCanSplit is set or not. |
| [set_LevelingDelay](./set_levelingdelay/) | Sets a value of LevelingDelay. |
| [set_ManualDuration](./set_manualduration/) | Sets a value of ManualDuration. |
| [set_ManualFinish](./set_manualfinish/) | Sets a value of ManualFinish. |
| [set_ManualStart](./set_manualstart/) | Sets a value of ManualStart. |
| [set_Name](./set_name/) | Sets a value of Name. |
| [set_NotesRTF](./set_notesrtf/) | Sets a value of NotesRTF. |
| [set_NotesText](./set_notestext/) | Sets a value of NotesText. |
| [set_OutlineCodes](./set_outlinecodes/) | Sets OutlineCodeCollection object. |
| [set_OutlineLevel](./set_outlinelevel/) | Sets a value of OutlineLevel. |
| [set_OutlineNumber](./set_outlinenumber/) | Sets a value of OutlineNumber. |
| [set_OvertimeCost](./set_overtimecost/) | Sets a value of OvertimeCost. |
| [set_OvertimeWork](./set_overtimework/) | Sets a value of OvertimeWork. |
| [set_PercentComplete](./set_percentcomplete/) | Sets a value of PercentComplete. |
| [set_PercentWorkComplete](./set_percentworkcomplete/) | Sets a value of PercentWorkComplete. |
| [set_PhysicalPercentComplete](./set_physicalpercentcomplete/) | Sets a value of PhysicalPercentComplete. |
| [set_PreleveledFinish](./set_preleveledfinish/) | Sets a value of PreleveledFinish. |
| [set_PreleveledStart](./set_preleveledstart/) | Sets a value of PreleveledStart. |
| [set_Priority](./set_priority/) | Sets a value of Priority. |
| [set_RegularWork](./set_regularwork/) | Sets a value of RegularWork. |
| [set_RemainingCost](./set_remainingcost/) | Sets a value of RemainingCost. |
| [set_RemainingDuration](./set_remainingduration/) | Sets a value of RemainingDuration. |
| [set_RemainingOvertimeCost](./set_remainingovertimecost/) | Sets a value of RemainingOvertimeCost. |
| [set_RemainingOvertimeWork](./set_remainingovertimework/) | Sets a value of RemainingOvertimeWork. |
| [set_RemainingWork](./set_remainingwork/) | Sets a value of RemainingWork. |
| [set_Resume](./set_resume/) | Sets a value of Resume. |
| [set_Start](./set_start/) | Sets a value of Start. |
| [set_StartSlack](./set_startslack/) | Sets a value of StartSlack. |
| [set_StartText](./set_starttext/) | Sets a value of StartText. |
| [set_StartVariance](./set_startvariance/) | Sets a value of StartVariance. |
| [set_StatusManager](./set_statusmanager/) | Sets a value of StatusManager. |
| [set_Stop](./set_stop/) | Sets a value of Stop. |
| [set_SubprojectName](./set_subprojectname/) | Sets a value of SubprojectName. |
| [set_SV](./set_sv/) | The earned value schedule variance, through the project status date. Schedule variance (SV) is the difference between the BCWP and the BCWS. |
| [set_TimephasedData](./set_timephaseddata/) | Sets a TimephasedDataCollection object of this task. The time phased data block associated with a task. |
| [set_TotalSlack](./set_totalslack/) | Sets a value of TotalSlack. |
| [set_Type](./set_type/) | Sets a value of Type. |
| [set_Uid](./set_uid/) | Sets a value of Uid. |
| [set_Warning](./set_warning/) | Sets a value indicating whether Warning is set or not. |
| [set_WBS](./set_wbs/) | Sets a value of WBS. |
| [set_WBSLevel](./set_wbslevel/) | Sets a value of WBSLevel. |
| [set_Work](./set_work/) | Sets a value of Work. |
| [set_WorkVariance](./set_workvariance/) | Sets a value of WorkVariance. |
| [ToString](./tostring/) | Returns short string representation of a task. The exact details of the representation are unspecified and subject to change. |

