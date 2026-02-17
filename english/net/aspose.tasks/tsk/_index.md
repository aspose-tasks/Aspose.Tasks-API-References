---
title: Class Tsk
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Tsk class. Represents properties of Task object
type: docs
weight: 2600
url: /net/aspose.tasks/tsk/
---
## Tsk class

Represents properties of [`Task`](../task/) object.

```csharp
public static class Tsk
```

## Fields

| Name | Description |
| --- | --- |
| static readonly [ActivityId](../../aspose.tasks/tsk/activityid/) | Represents activity id field - a task's unique identifier used by Primavera. (only applicable to Primavera projects). |
| static readonly [ActualCost](../../aspose.tasks/tsk/actualcost/) | Costs incurred for work already performed by resources on their tasks, together with any other recorded costs associated with the task. |
| static readonly [ActualDuration](../../aspose.tasks/tsk/actualduration/) | The span of actual working time for a task, based on the scheduled duration and current remaining work or percent complete. |
| static readonly [ActualFinish](../../aspose.tasks/tsk/actualfinish/) | The date when a task was completed. |
| static readonly [ActualOvertimeCost](../../aspose.tasks/tsk/actualovertimecost/) | Costs incurred for overtime work already performed on tasks by assigned resources. |
| static readonly [ActualOvertimeWork](../../aspose.tasks/tsk/actualovertimework/) | The actual amount of overtime work already performed by resources assigned to tasks. |
| static readonly [ActualOvertimeWorkProtected](../../aspose.tasks/tsk/actualovertimeworkprotected/) | The duration through which actual overtime work is protected. |
| static readonly [ActualStart](../../aspose.tasks/tsk/actualstart/) | The date and time that a task actually began. |
| static readonly [ActualWork](../../aspose.tasks/tsk/actualwork/) | The amount of work that has already been done by resources assigned to tasks. |
| static readonly [ActualWorkProtected](../../aspose.tasks/tsk/actualworkprotected/) | The duration through which actual work is protected. Reading supported for XML format only. |
| static readonly [ACWP](../../aspose.tasks/tsk/acwp/) | Costs incurred for work already done on a task, up to the project status date or today's date. |
| static readonly [BCWP](../../aspose.tasks/tsk/bcwp/) | The cumulative value of the task's percent complete multiplied by the time phased baseline costs. |
| static readonly [BCWS](../../aspose.tasks/tsk/bcws/) | The cumulative time phased baseline costs up to the status date or today's date. |
| static readonly [BudgetCost](../../aspose.tasks/tsk/budgetcost/) | Budget costs for budget cost resources. Budget resources are assigned only to the project summary task. |
| static readonly [BudgetWork](../../aspose.tasks/tsk/budgetwork/) | Budget work for budget work and material resources. Budget resources are assigned only to the project summary task. |
| static readonly [Calendar](../../aspose.tasks/tsk/calendar/) | The task calendar. |
| static readonly [CommitmentFinish](../../aspose.tasks/tsk/commitmentfinish/) | The finish date of a delivery.  Reading supported for XML format only. |
| static readonly [CommitmentStart](../../aspose.tasks/tsk/commitmentstart/) | The start date of a delivery. Reading supported for XML format only. |
| static readonly [CommitmentType](../../aspose.tasks/tsk/commitmenttype/) | Determines whether a task has an associated delivery or a dependency on an associated delivery.  Reading supported for XML format only. |
| static readonly [ConstraintDate](../../aspose.tasks/tsk/constraintdate/) | The specific date associated with the constraint type. |
| static readonly [ConstraintType](../../aspose.tasks/tsk/constrainttype/) | Provides choices for the type of constraint that can be applied for scheduling a task. |
| static readonly [Contact](../../aspose.tasks/tsk/contact/) | The name of an individual responsible for a task. |
| static readonly [Cost](../../aspose.tasks/tsk/cost/) | The total scheduled or projected cost for a task based on costs already incurred for work performed by resources assigned to the tasks, in addition to the costs planned for the remaining work. |
| static readonly [CostVariance](../../aspose.tasks/tsk/costvariance/) | The difference between the baseline cost and total cost for a task, resource, or assignment. |
| static readonly [Created](../../aspose.tasks/tsk/created/) | The date when a task was created. |
| static readonly [CV](../../aspose.tasks/tsk/cv/) | The difference between the baseline cost and total cost for a task. Cost Variance = Cost - Baseline Cost |
| static readonly [Deadline](../../aspose.tasks/tsk/deadline/) | A target date that indicates when a task is to be completed. |
| static readonly [DisplayAsSummary](../../aspose.tasks/tsk/displayassummary/) | Determines whether the task should be displayed as a summary task. Reading supported for XML format only. |
| static readonly [DisplayOnTimeline](../../aspose.tasks/tsk/displayontimeline/) | Specifies whether a task should be displayed on a timeline view. |
| static readonly [Duration](../../aspose.tasks/tsk/duration/) | The total span of active working time for a task as entered or as calculated by Microsoft Project based on start date, finish date, calendars, and other scheduling factors. |
| static readonly [DurationText](../../aspose.tasks/tsk/durationtext/) | Returns the task's duration text. |
| static readonly [DurationVariance](../../aspose.tasks/tsk/durationvariance/) | The difference between the baseline duration of a task and the total duration (current estimate) of a task. |
| static readonly [EarlyFinish](../../aspose.tasks/tsk/earlyfinish/) | The earliest date that a task could possibly finish, based on early finish dates of predecessor and successor tasks, other constraints, and any leveling delay. |
| static readonly [EarlyStart](../../aspose.tasks/tsk/earlystart/) | The earliest date that a task could possibly begin, based on the early start dates of predecessor and successor tasks and other constraints. |
| static readonly [EarnedValueMethod](../../aspose.tasks/tsk/earnedvaluemethod/) | Determines whether the % Complete or Physical % Complete field should be used to calculate budgeted cost of work performed (BCWP). |
| static readonly [ExternalId](../../aspose.tasks/tsk/externalid/) | If a task is an external task it contains the task's external Id. |
| static readonly [ExternalTaskProject](../../aspose.tasks/tsk/externaltaskproject/) | The source location and task identifier of an external task. |
| static readonly [ExternalUid](../../aspose.tasks/tsk/externaluid/) | Contains the external task's Unique identifier when the task is external. |
| static readonly [Finish](../../aspose.tasks/tsk/finish/) | The scheduled finish date of a task. |
| static readonly [FinishSlackTimeSpan](../../aspose.tasks/tsk/finishslacktimespan/) | The duration between the Early Finish and Late Finish dates. |
| static readonly [FinishText](../../aspose.tasks/tsk/finishtext/) | Returns the task's finish text. |
| static readonly [FinishVariance](../../aspose.tasks/tsk/finishvariance/) | The time that represents the difference between the baseline finish date of a task or assignment and its current finish date. |
| static readonly [FixedCost](../../aspose.tasks/tsk/fixedcost/) | Shows any non resource task expense. |
| static readonly [FixedCostAccrual](../../aspose.tasks/tsk/fixedcostaccrual/) | Determines choices for how and when fixed costs are to be charged, or accrued, to the cost of a task. |
| static readonly [FreeSlackTimeSpan](../../aspose.tasks/tsk/freeslacktimespan/) | The time that a task can be delayed without delaying any successor tasks. |
| static readonly [Guid](../../aspose.tasks/tsk/guid/) | The generated unique identification codes for a task. |
| static readonly [HasOverallocatedResource](../../aspose.tasks/tsk/hasoverallocatedresource/) | Indicates whether the task has an resource assigned which has more work on assigned tasks than can be completed within normal working capacity. |
| static readonly [HideBar](../../aspose.tasks/tsk/hidebar/) | Determines whether the Gantt bar of a task is hidden when displayed in Microsoft Project. |
| static readonly [Hyperlink](../../aspose.tasks/tsk/hyperlink/) | The title or explanatory text for a hyperlink associated with a task. |
| static readonly [HyperlinkAddress](../../aspose.tasks/tsk/hyperlinkaddress/) | The address for a hyperlink associated with a task. |
| static readonly [HyperlinkSubAddress](../../aspose.tasks/tsk/hyperlinksubaddress/) | The specific location in a document in a hyperlink associated with a task. |
| static readonly [Id](../../aspose.tasks/tsk/id/) | The position identifier of a task within the list of tasks. |
| static readonly [IgnoreResourceCalendar](../../aspose.tasks/tsk/ignoreresourcecalendar/) | Determines whether the scheduling of the task considers the calendars of the resources assigned to the task. |
| static readonly [IgnoreWarnings](../../aspose.tasks/tsk/ignorewarnings/) | Indicates whether to hide the schedule conflict warning indicator in Microsoft Project. |
| static readonly [IsActive](../../aspose.tasks/tsk/isactive/) | Determines whether a task is active. Inactive tasks no longer affect other tasks or the overall Project schedule. |
| static readonly [IsCritical](../../aspose.tasks/tsk/iscritical/) | Determines whether a task is on the critical path. |
| static readonly [IsEffortDriven](../../aspose.tasks/tsk/iseffortdriven/) | Determines whether the scheduling for the task is effort-driven scheduling. |
| static readonly [IsEstimated](../../aspose.tasks/tsk/isestimated/) | Determines whether a task is estimated. |
| static readonly [IsExpanded](../../aspose.tasks/tsk/isexpanded/) | Determines whether a summary task is expanded or not in GanttChart view. |
| static readonly [IsExternalTask](../../aspose.tasks/tsk/isexternaltask/) | Determines whether a task is external. |
| static readonly [IsManual](../../aspose.tasks/tsk/ismanual/) | Determines whether a task is manually scheduled. |
| static readonly [IsMarked](../../aspose.tasks/tsk/ismarked/) | Shows whether a task is marked for further action or identification of some kind. |
| static readonly [IsMilestone](../../aspose.tasks/tsk/ismilestone/) | Determines whether a task is a milestone. |
| static readonly [IsNull](../../aspose.tasks/tsk/isnull/) | Determines whether a task is a null task. |
| static readonly [IsOverallocated](../../aspose.tasks/tsk/isoverallocated/) | Indicates whether any of the assigned resources on a task is assigned to more work on the task than can be done withing the normal working capacity. |
| static readonly [IsPublished](../../aspose.tasks/tsk/ispublished/) | Determines whether the current task should be published to Project Server with the rest of the project. |
| static readonly [IsRecurring](../../aspose.tasks/tsk/isrecurring/) | Determines whether a task is part of a series of recurring tasks. |
| static readonly [IsResumeValid](../../aspose.tasks/tsk/isresumevalid/) | Determines whether a task can be resumed. |
| static readonly [IsRollup](../../aspose.tasks/tsk/isrollup/) | Determines whether information about the subtask Gantt bars will be rolled up to the summary task bar. |
| static readonly [IsSubproject](../../aspose.tasks/tsk/issubproject/) | Determines whether a task is an inserted project. |
| static readonly [IsSubprojectReadOnly](../../aspose.tasks/tsk/issubprojectreadonly/) | Determines whether a subproject is read-only. |
| static readonly [IsSummary](../../aspose.tasks/tsk/issummary/) | Determines whether a task is a summary task. |
| static readonly [LateFinish](../../aspose.tasks/tsk/latefinish/) | The latest date that a task can finish without delaying the finish of the project. |
| static readonly [LateStart](../../aspose.tasks/tsk/latestart/) | The latest date that a task can start without delaying the finish of the project. |
| static readonly [LevelAssignments](../../aspose.tasks/tsk/levelassignments/) | Determines whether the leveling function can delay and split individual assignments in order to resolve over allocations. |
| static readonly [LevelingCanSplit](../../aspose.tasks/tsk/levelingcansplit/) | Determines whether the resource leveling function can cause splits on remaining work on this task. |
| static readonly [LevelingDelay](../../aspose.tasks/tsk/levelingdelay/) | The time that a task is to be delayed from its early start date because of resource leveling. |
| static readonly [ManualDuration](../../aspose.tasks/tsk/manualduration/) | Defines manually scheduled duration of a task. |
| static readonly [ManualFinish](../../aspose.tasks/tsk/manualfinish/) | Defines manually scheduled finish of a task. |
| static readonly [ManualStart](../../aspose.tasks/tsk/manualstart/) | Defines manually scheduled start of a task. |
| static readonly [Name](../../aspose.tasks/tsk/name/) | A task's name. |
| static readonly [NotesRTF](../../aspose.tasks/tsk/notesrtf/) | The text notes in RTF format. Supported for MPP formats only. |
| static readonly [NotesText](../../aspose.tasks/tsk/notestext/) | Notes' plain text extracted from RTF data. |
| static readonly [OutlineLevel](../../aspose.tasks/tsk/outlinelevel/) | The outline level of a task. |
| static readonly [OutlineNumber](../../aspose.tasks/tsk/outlinenumber/) | The number that represents a task's position in the hierarchical outline structure. |
| static readonly [OvertimeCost](../../aspose.tasks/tsk/overtimecost/) | The total overtime cost for a task, for a resource on all assigned tasks, or for a resource assignment. |
| static readonly [OvertimeWork](../../aspose.tasks/tsk/overtimework/) | The amount of overtime scheduled to be performed by all resources assigned to a task. |
| static readonly [PercentComplete](../../aspose.tasks/tsk/percentcomplete/) | The current status of a task, expressed as the percentage of the task's duration that has been completed. |
| static readonly [PercentWorkComplete](../../aspose.tasks/tsk/percentworkcomplete/) | The current status of a task expressed as the percentage of work that has been completed. |
| static readonly [PhysicalPercentComplete](../../aspose.tasks/tsk/physicalpercentcomplete/) | Percent complete value that can be be used as an alternative for calculating budgeted cost of work performed (BCWP). |
| static readonly [PreleveledFinish](../../aspose.tasks/tsk/preleveledfinish/) | The finish date of a task as it was before resource leveling was done. |
| static readonly [PreleveledStart](../../aspose.tasks/tsk/preleveledstart/) | The start date of a task as it was before resource leveling was done. |
| static readonly [Priority](../../aspose.tasks/tsk/priority/) | The level of importance given to a task, which in turn indicates how readily a task or assignment can be delayed or split during resource leveling. |
| static readonly [RegularWork](../../aspose.tasks/tsk/regularwork/) | The total amount of non overtime work scheduled to be performed by resources. |
| static readonly [RemainingCost](../../aspose.tasks/tsk/remainingcost/) | The remaining scheduled expense that will be incurred in completing the remaining scheduled work. |
| static readonly [RemainingDuration](../../aspose.tasks/tsk/remainingduration/) | The time that is required to complete the unfinished part of a task. |
| static readonly [RemainingOvertimeCost](../../aspose.tasks/tsk/remainingovertimecost/) | The remaining scheduled overtime expense for a task. |
| static readonly [RemainingOvertimeWork](../../aspose.tasks/tsk/remainingovertimework/) | The amount of remaining scheduled overtime time. |
| static readonly [RemainingWork](../../aspose.tasks/tsk/remainingwork/) | The time still required to complete a task or set of tasks. |
| static readonly [Resume](../../aspose.tasks/tsk/resume/) | The date that the remaining part of a task is scheduled to resume after entering any progress. |
| static readonly [Start](../../aspose.tasks/tsk/start/) | The scheduled start date of a task. |
| static readonly [StartSlackTimeSpan](../../aspose.tasks/tsk/startslacktimespan/) | The duration between the Early Start and Late Start dates. |
| static readonly [StartText](../../aspose.tasks/tsk/starttext/) | Returns the task's start text. |
| static readonly [StartVariance](../../aspose.tasks/tsk/startvariance/) | The time that represents the difference between a baseline start date of a task or assignment and its currently scheduled start date. |
| static readonly [StatusManager](../../aspose.tasks/tsk/statusmanager/) | The name of the enterprise resource who is to receive status updates for the current task from resources. |
| static readonly [Stop](../../aspose.tasks/tsk/stop/) | The date that represents the end of the actual portion of a task. |
| static readonly [SubprojectName](../../aspose.tasks/tsk/subprojectname/) | The source location of a subproject. |
| static readonly [SV](../../aspose.tasks/tsk/sv/) | The earned value schedule variance, through the project status date. Schedule variance (SV) is the difference between the BCWP and the BCWS. |
| static readonly [TotalSlackTimeSpan](../../aspose.tasks/tsk/totalslacktimespan/) | The time a task's finish date can be delayed without delaying the project's finish date. |
| static readonly [Type](../../aspose.tasks/tsk/type/) | The type of a task. |
| static readonly [Uid](../../aspose.tasks/tsk/uid/) | The unique Id of a task. |
| static readonly [Warning](../../aspose.tasks/tsk/warning/) | Represents the flag which indicates that task has schedule discrepancies. |
| static readonly [WBS](../../aspose.tasks/tsk/wbs/) | Work breakdown structure (WBS) codes. |
| static readonly [WBSLevel](../../aspose.tasks/tsk/wbslevel/) | The rightmost WBS level of a task. |
| static readonly [Work](../../aspose.tasks/tsk/work/) | The total time scheduled on a task for all assigned resources. |
| static readonly [WorkVariance](../../aspose.tasks/tsk/workvariance/) | The difference between baseline work of a task and the currently scheduled work. |

## Examples

Shows how to read/write task properties.

```csharp
var project = new Project();

// Add task and set task properties
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Parse through all the collected tasks
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


