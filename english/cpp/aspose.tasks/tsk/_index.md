---
title: "Aspose::Tasks::Tsk class"
linktitle: "Tsk"
articleTitle: "Tsk"
second_title: "Aspose.Tasks for C++"
description: "Represents properties of Task object."
type: docs
weight: 10
url: /cpp/aspose.tasks/tsk/
---

## Tsk class

Represents properties of Task object.

## Methods

| Name | Description |
| --- | --- |
| [ActivityId](./activityid/) | Represents activity id field - a task's unique identifier used by Primavera. (only applicable to Primavera projects). |
| [ActualCost](./actualcost/) | Costs incurred for work already performed by resources on their tasks, together with any other recorded costs associated with the task. |
| [ActualDuration](./actualduration/) | The span of actual working time for a task, based on the scheduled duration and current remaining work or percent complete. |
| [ActualFinish](./actualfinish/) | The date when a task was completed. |
| [ActualOvertimeCost](./actualovertimecost/) | Costs incurred for overtime work already performed on tasks by assigned resources. |
| [ActualOvertimeWork](./actualovertimework/) | The actual amount of overtime work already performed by resources assigned to tasks. |
| [ActualOvertimeWorkProtected](./actualovertimeworkprotected/) | The duration through which actual overtime work is protected. |
| [ActualStart](./actualstart/) | The date and time that a task actually began. |
| [ActualWork](./actualwork/) | The amount of work that has already been done by resources assigned to tasks. |
| [ActualWorkProtected](./actualworkprotected/) | The duration through which actual work is protected. |
| [ACWP](./acwp/) | Costs incurred for work already done on a task, up to the project status date or today's date. |
| [BCWP](./bcwp/) | The cumulative value of the task's percent complete multiplied by the time phased baseline costs. |
| [BCWS](./bcws/) | The cumulative time phased baseline costs up to the status date or today's date. |
| [BudgetCost](./budgetcost/) | Budget costs for budget cost resources. Budget resources are assigned only to the project summary task. |
| [BudgetWork](./budgetwork/) | Budget work for budget work and material resources. Budget resources are assigned only to the project summary task. |
| [Calendar](./calendar/) | The task calendar. |
| [CommitmentFinish](./commitmentfinish/) | The finish date of a delivery. |
| [CommitmentStart](./commitmentstart/) | The start date of a delivery. |
| [CommitmentType](./commitmenttype/) | Determines whether a task has an associated delivery or a dependency on an associated delivery. |
| [ConstraintDate](./constraintdate/) | The specific date associated with the constraint type. |
| [ConstraintType](./constrainttype/) | Provides choices for the type of constraint that can be applied for scheduling a task. |
| [Contact](./contact/) | The name of an individual responsible for a task. |
| [Cost](./cost/) | The total scheduled or projected cost for a task based on costs already incurred for work performed by resources assigned to the tasks, in addition to the costs planned for the remaining work. |
| [CostVariance](./costvariance/) | The difference between the baseline cost and total cost for a task, resource, or assignment. |
| [Created](./created/) | The date when a task was created. |
| [CV](./cv/) | The difference between the baseline cost and total cost for a task. Cost Variance = Cost - Baseline Cost |
| [Deadline](./deadline/) | A target date that indicates when a task is to be completed. |
| [DisplayAsSummary](./displayassummary/) | Determines whether the task should be displayed as a summary task. |
| [DisplayOnTimeline](./displayontimeline/) | Specifies whether a task should be displayed on a timeline view. |
| [Duration](./duration/) | The total span of active working time for a task as entered or as calculated by Microsoft Project based on start date, finish date, calendars, and other scheduling factors. |
| [DurationText](./durationtext/) | Returns the task's duration text. |
| [DurationVariance](./durationvariance/) | The difference between the baseline duration of a task and the total duration (current estimate) of a task. |
| [EarlyFinish](./earlyfinish/) | The earliest date that a task could possibly finish, based on early finish dates of predecessor and successor tasks, other constraints, and any leveling delay. |
| [EarlyStart](./earlystart/) | The earliest date that a task could possibly begin, based on the early start dates of predecessor and successor tasks and other constraints. |
| [EarnedValueMethod](./earnedvaluemethod/) | Determines whether the % Complete or Physical % Complete field should be used to calculate budgeted cost of work performed (BCWP). |
| [ExternalId](./externalid/) | If a task is an external task it contains the task's external Id. |
| [ExternalTaskProject](./externaltaskproject/) | The source location and task identifier of an external task. |
| [ExternalUid](./externaluid/) | Contains the external task's Unique identifier when the task is external. |
| [Finish](./finish/) | The scheduled finish date of a task. |
| [FinishSlackTimeSpan](./finishslacktimespan/) | The duration between the Early Finish and Late Finish dates. |
| [FinishText](./finishtext/) | Returns the task's finish text. |
| [FinishVariance](./finishvariance/) | The time that represents the difference between the baseline finish date of a task or assignment and its current finish date. |
| [FixedCost](./fixedcost/) | Shows any non resource task expense. |
| [FixedCostAccrual](./fixedcostaccrual/) | Determines choices for how and when fixed costs are to be charged, or accrued, to the cost of a task. |
| [FreeSlackTimeSpan](./freeslacktimespan/) | The time that a task can be delayed without delaying any successor tasks. |
| [Guid](./guid/) | The generated unique identification codes for a task. |
| [HasOverallocatedResource](./hasoverallocatedresource/) | Indicates whether the task has an resource assigned which has more work on assigned tasks than can be completed within normal working capacity. |
| [HideBar](./hidebar/) | Determines whether the Gantt bar of a task is hidden when displayed in Microsoft Project . |
| [Hyperlink](./hyperlink/) | The title or explanatory text for a hyperlink associated with a task. |
| [HyperlinkAddress](./hyperlinkaddress/) | The address for a hyperlink associated with a task. |
| [HyperlinkSubAddress](./hyperlinksubaddress/) | The specific location in a document in a hyperlink associated with a task. |
| [Id](./id/) | The position identifier of a task within the list of tasks. |
| [IgnoreResourceCalendar](./ignoreresourcecalendar/) | Determines whether the scheduling of the task considers the calendars of the resources assigned to the task. |
| [IgnoreWarnings](./ignorewarnings/) | Indicates whether to hide the schedule conflict warning indicator in Microsoft Project . |
| [IsActive](./isactive/) | Determines whether a task is active. Inactive tasks no longer affect other tasks or the overall Project schedule. |
| [IsCritical](./iscritical/) | Determines whether a task is on the critical path. |
| [IsEffortDriven](./iseffortdriven/) | Determines whether the scheduling for the task is effort-driven scheduling. |
| [IsEstimated](./isestimated/) | Determines whether a task is estimated. |
| [IsExpanded](./isexpanded/) | Determines whether a summary task is expanded or not in GanttChart view. |
| [IsExternalTask](./isexternaltask/) | Determines whether a task is external. |
| [IsManual](./ismanual/) | Determines whether a task is manually scheduled. |
| [IsMarked](./ismarked/) | Shows whether a task is marked for further action or identification of some kind. |
| [IsMilestone](./ismilestone/) | Determines whether a task is a milestone. |
| [IsNull](./isnull/) | Determines whether a task is a null task. |
| [IsOverallocated](./isoverallocated/) | Indicates whether any of the assigned resources on a task is assigned to more work on the task than can be done withing the normal working capacity. |
| [IsPublished](./ispublished/) | Determines whether the current task should be published to Project Server with the rest of the project. |
| [IsRecurring](./isrecurring/) | Determines whether a task is part of a series of recurring tasks. |
| [IsResumeValid](./isresumevalid/) | Determines whether a task can be resumed. |
| [IsRollup](./isrollup/) | Determines whether information about the subtask Gantt bars will be rolled up to the summary task bar. |
| [IsSubproject](./issubproject/) | Determines whether a task is an inserted project. |
| [IsSubprojectReadOnly](./issubprojectreadonly/) | Determines whether a subproject is read-only. |
| [IsSummary](./issummary/) | Determines whether a task is a summary task. |
| [LateFinish](./latefinish/) | The latest date that a task can finish without delaying the finish of the project. |
| [LateStart](./latestart/) | The latest date that a task can start without delaying the finish of the project. |
| [LevelAssignments](./levelassignments/) | Determines whether the leveling function can delay and split individual assignments in order to resolve over allocations. |
| [LevelingCanSplit](./levelingcansplit/) | Determines whether the resource leveling function can cause splits on remaining work on this task. |
| [LevelingDelay](./levelingdelay/) | The time that a task is to be delayed from its early start date because of resource leveling. |
| [ManualDuration](./manualduration/) | Defines manually scheduled duration of a task. |
| [ManualFinish](./manualfinish/) | Defines manually scheduled finish of a task. |
| [ManualStart](./manualstart/) | Defines manually scheduled start of a task. |
| [Name](./name/) | A task's name. |
| [NotesRTF](./notesrtf/) | The text notes in RTF format. |
| [NotesText](./notestext/) | Notes' plain text extracted from RTF data. |
| [OutlineLevel](./outlinelevel/) | The outline level of a task. |
| [OutlineNumber](./outlinenumber/) | The number that represents a task's position in the hierarchical outline structure. |
| [OvertimeCost](./overtimecost/) | The total overtime cost for a task, for a resource on all assigned tasks, or for a resource assignment. |
| [OvertimeWork](./overtimework/) | The amount of overtime scheduled to be performed by all resources assigned to a task. |
| [PercentComplete](./percentcomplete/) | The current status of a task, expressed as the percentage of the task's duration that has been completed. |
| [PercentWorkComplete](./percentworkcomplete/) | The current status of a task expressed as the percentage of work that has been completed. |
| [PhysicalPercentComplete](./physicalpercentcomplete/) | Percent complete value that can be be used as an alternative for calculating budgeted cost of work performed (BCWP). |
| [PreleveledFinish](./preleveledfinish/) | The finish date of a task as it was before resource leveling was done. |
| [PreleveledStart](./preleveledstart/) | The start date of a task as it was before resource leveling was done. |
| [Priority](./priority/) | The level of importance given to a task, which in turn indicates how readily a task or assignment can be delayed or split during resource leveling. |
| [RegularWork](./regularwork/) | The total amount of non overtime work scheduled to be performed by resources. |
| [RemainingCost](./remainingcost/) | The remaining scheduled expense that will be incurred in completing the remaining scheduled work. |
| [RemainingDuration](./remainingduration/) | The time that is required to complete the unfinished part of a task. |
| [RemainingOvertimeCost](./remainingovertimecost/) | The remaining scheduled overtime expense for a task. |
| [RemainingOvertimeWork](./remainingovertimework/) | The amount of remaining scheduled overtime time. |
| [RemainingWork](./remainingwork/) | The time still required to complete a task or set of tasks. |
| [Resume](./resume/) | The date that the remaining part of a task is scheduled to resume after entering any progress. |
| [Start](./start/) | The scheduled start date of a task. |
| [StartSlackTimeSpan](./startslacktimespan/) | The duration between the Early Start and Late Start dates. |
| [StartText](./starttext/) | Returns the task's start text. |
| [StartVariance](./startvariance/) | The time that represents the difference between a baseline start date of a task or assignment and its currently scheduled start date. |
| [StatusManager](./statusmanager/) | The name of the enterprise resource who is to receive status updates for the current task from resources. |
| [Stop](./stop/) | The date that represents the end of the actual portion of a task. |
| [SubprojectName](./subprojectname/) | The source location of a subproject. |
| [SV](./sv/) | The earned value schedule variance, through the project status date. Schedule variance (SV) is the difference between the BCWP and the BCWS. |
| [TotalSlackTimeSpan](./totalslacktimespan/) | The time a task's finish date can be delayed without delaying the project's finish date. |
| [Type](./type/) | The type of a task. |
| [Uid](./uid/) | The unique Id of a task. |
| [Warning](./warning/) | Represents the flag which indicates that task has schedule discrepancies. |
| [WBS](./wbs/) | Work breakdown structure (WBS) codes. |
| [WBSLevel](./wbslevel/) | The rightmost WBS level of a task. |
| [Work](./work/) | The total time scheduled on a task for all assigned resources. |
| [WorkVariance](./workvariance/) | The difference between baseline work of a task and the currently scheduled work. |

