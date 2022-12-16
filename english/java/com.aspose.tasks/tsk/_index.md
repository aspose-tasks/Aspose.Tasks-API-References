---
title: Tsk
second_title: Aspose.Tasks for Java API Reference
description: Represents properties of  object.
type: docs
weight: 298
url: /java/com.aspose.tasks/tsk/
---

**Inheritance:**
java.lang.Object
```
public class Tsk
```

Represents properties of [Task](../../com.aspose.tasks/task) object.
## Constructors

| Constructor | Description |
| --- | --- |
| [Tsk()](#Tsk--) |  |
## Fields

| Field | Description |
| --- | --- |
| [ACTIVITY_ID](#ACTIVITY-ID) | Represents activity id field - a task's unique identifier used by Primavera. |
| [ACTUAL_COST](#ACTUAL-COST) | Costs incurred for work already performed by resources on their tasks, together with any other recorded costs associated with the task. |
| [ACTUAL_DURATION](#ACTUAL-DURATION) | The span of actual working time for a task, based on the scheduled duration and current remaining work or percent complete. |
| [ACTUAL_FINISH](#ACTUAL-FINISH) | The date when a task was completed. |
| [ACTUAL_OVERTIME_COST](#ACTUAL-OVERTIME-COST) | Costs incurred for overtime work already performed on tasks by assigned resources. |
| [ACTUAL_OVERTIME_WORK](#ACTUAL-OVERTIME-WORK) | The actual amount of overtime work already performed by resources assigned to tasks. |
| [ACTUAL_OVERTIME_WORK_PROTECTED](#ACTUAL-OVERTIME-WORK-PROTECTED) | The duration through which actual overtime work is protected. |
| [ACTUAL_START](#ACTUAL-START) | The date and time that a task actually began. |
| [ACTUAL_WORK](#ACTUAL-WORK) | The amount of work that has already been done by resources assigned to tasks. |
| [ACTUAL_WORK_PROTECTED](#ACTUAL-WORK-PROTECTED) | The duration through which actual work is protected. |
| [ACWP](#ACWP) | Costs incurred for work already done on a task, up to the project status date or today's date. |
| [BCWP](#BCWP) | The cumulative value of the task's percent complete multiplied by the time phased baseline costs. |
| [BCWS](#BCWS) | The cumulative time phased baseline costs up to the status date or today's date. |
| [BUDGET_COST](#BUDGET-COST) | Budget costs for budget cost resources. |
| [BUDGET_WORK](#BUDGET-WORK) | Budget work for budget work and material resources. |
| [CALENDAR](#CALENDAR) | The task calendar. |
| [COMMITMENT_FINISH](#COMMITMENT-FINISH) | The finish date of a delivery. |
| [COMMITMENT_START](#COMMITMENT-START) | The start date of a delivery. |
| [COMMITMENT_TYPE](#COMMITMENT-TYPE) | Determines whether a task has an associated delivery or a dependency on an associated delivery. |
| [CONSTRAINT_DATE](#CONSTRAINT-DATE) | The specific date associated with the constraint type. |
| [CONSTRAINT_TYPE](#CONSTRAINT-TYPE) | Provides choices for the type of constraint that can be applied for scheduling a task. |
| [CONTACT](#CONTACT) | The name of an individual responsible for a task. |
| [COST](#COST) | The total scheduled or projected cost for a task based on costs already incurred for work performed by resources assigned to the tasks, in addition to the costs planned for the remaining work. |
| [COST_VARIANCE](#COST-VARIANCE) | The difference between the baseline cost and total cost for a task, resource, or assignment. |
| [CREATED](#CREATED) | The date when a task was created. |
| [CV](#CV) | The difference between the baseline cost and total cost for a task. |
| [DEADLINE](#DEADLINE) | A target date that indicates when a task is to be completed. |
| [DISPLAY_AS_SUMMARY](#DISPLAY-AS-SUMMARY) | Determines whether the task should be displayed as a summary task. |
| [DISPLAY_ON_TIMELINE](#DISPLAY-ON-TIMELINE) | Specifies whether a task should be displayed on a timeline view. |
| [DURATION](#DURATION) | The total span of active working time for a task as entered or as calculated by Microsoft Project based on start date, finish date, calendars, and other scheduling factors. |
| [DURATION_FORMAT](#DURATION-FORMAT) | Task duration format. |
| [DURATION_TEXT](#DURATION-TEXT) | Returns the task's duration text. |
| [DURATION_VARIANCE](#DURATION-VARIANCE) | The difference between the baseline duration of a task and the total duration (current estimate) of a task. |
| [EARLY_FINISH](#EARLY-FINISH) | The earliest date that a task could possibly finish, based on early finish dates of predecessor and successor tasks, other constraints, and any leveling delay. |
| [EARLY_START](#EARLY-START) | The earliest date that a task could possibly begin, based on the early start dates of predecessor and successor tasks and other constraints. |
| [EARNED_VALUE_METHOD](#EARNED-VALUE-METHOD) | Determines whether the % Complete or Physical % Complete field should be used to calculate budgeted cost of work performed (BCWP). |
| [EXTERNAL_ID](#EXTERNAL-ID) | If a task is an external task it contains the task's external Id. |
| [EXTERNAL_TASK_PROJECT](#EXTERNAL-TASK-PROJECT) | The source location and task identifier of an external task. |
| [EXTERNAL_UID](#EXTERNAL-UID) | Contains the external task's Unique identifier when the task is external. |
| [FINISH](#FINISH) | The scheduled finish date of a task. |
| [FINISH_SLACK_TIME_SPAN](#FINISH-SLACK-TIME-SPAN) | The duration (in seconds) between the Early Finish and Late Finish dates. |
| [FINISH_TEXT](#FINISH-TEXT) | Returns the task's finish text. |
| [FINISH_VARIANCE](#FINISH-VARIANCE) | The time that represents the difference between the baseline finish date of a task or assignment and its current finish date. |
| [FIXED_COST](#FIXED-COST) | Shows any non resource task expense. |
| [FIXED_COST_ACCRUAL](#FIXED-COST-ACCRUAL) | Determines choices for how and when fixed costs are to be charged, or accrued, to the cost of a task. |
| [FREE_SLACK_TIME_SPAN](#FREE-SLACK-TIME-SPAN) | The time (in seconds) that a task can be delayed without delaying any successor tasks. |
| [GUID](#GUID) | The generated unique identification codes for a task. |
| [HAS_OVERALLOCATED_RESOURCE](#HAS-OVERALLOCATED-RESOURCE) | Indicates whether the task has an resource assigned which has more work on assigned tasks than can be completed within normal working capacity. |
| [HIDE_BAR](#HIDE-BAR) | Determines whether the Gantt bar of a task is hidden when displayed in Microsoft Project. |
| [HYPERLINK](#HYPERLINK) | The title or explanatory text for a hyperlink associated with a task. |
| [HYPERLINK_ADDRESS](#HYPERLINK-ADDRESS) | The address for a hyperlink associated with a task. |
| [HYPERLINK_SUB_ADDRESS](#HYPERLINK-SUB-ADDRESS) | The specific location in a document in a hyperlink associated with a task. |
| [ID](#ID) | The position identifier of a task within the list of tasks. |
| [IGNORE_RESOURCE_CALENDAR](#IGNORE-RESOURCE-CALENDAR) | Determines whether the scheduling of the task considers the calendars of the resources assigned to the task. |
| [IGNORE_WARNINGS](#IGNORE-WARNINGS) | Indicates whether to hide the schedule conflict warning indicator in Microsoft Project. |
| [IS_ACTIVE](#IS-ACTIVE) | Determines whether a task is active. |
| [IS_CRITICAL](#IS-CRITICAL) | Determines whether a task is on the critical path. |
| [IS_EFFORT_DRIVEN](#IS-EFFORT-DRIVEN) | Determines whether the scheduling for the task is effort-driven scheduling. |
| [IS_ESTIMATED](#IS-ESTIMATED) | Determines whether a task is estimated. |
| [IS_EXPANDED](#IS-EXPANDED) | Determines whether a summary task is expanded or not in GanttChart view. |
| [IS_EXTERNAL_TASK](#IS-EXTERNAL-TASK) | Determines whether a task is external. |
| [IS_MANUAL](#IS-MANUAL) | Determines whether a task is manually scheduled. |
| [IS_MARKED](#IS-MARKED) | Shows whether a task is marked for further action or identification of some kind. |
| [IS_MILESTONE](#IS-MILESTONE) | Determines whether a task is a milestone. |
| [IS_NULL](#IS-NULL) | Determines whether a task is a null task. |
| [IS_OVERALLOCATED](#IS-OVERALLOCATED) | Indicates whether any of the assigned resources on a task is assigned to more work on the task than can be done withing the normal working capacity. |
| [IS_PUBLISHED](#IS-PUBLISHED) | Determines whether the current task should be published to Project Server with the rest of the project. |
| [IS_RECURRING](#IS-RECURRING) | Determines whether a task is part of a series of recurring tasks. |
| [IS_RESUME_VALID](#IS-RESUME-VALID) | Determines whether a task can be resumed. |
| [IS_ROLLUP](#IS-ROLLUP) | Determines whether information about the subtask Gantt bars will be rolled up to the summary task bar. |
| [IS_SUBPROJECT](#IS-SUBPROJECT) | Determines whether a task is an inserted project. |
| [IS_SUBPROJECT_READ_ONLY](#IS-SUBPROJECT-READ-ONLY) | Determines whether a subproject is read-only. |
| [IS_SUMMARY](#IS-SUMMARY) | Determines whether a task is a summary task. |
| [LATE_FINISH](#LATE-FINISH) | The latest date that a task can finish without delaying the finish of the project. |
| [LATE_START](#LATE-START) | The latest date that a task can start without delaying the finish of the project. |
| [LEVELING_CAN_SPLIT](#LEVELING-CAN-SPLIT) | Determines whether the resource leveling function can cause splits on remaining work on this task. |
| [LEVELING_DELAY](#LEVELING-DELAY) | The time that a task is to be delayed from its early start date because of resource leveling. |
| [LEVELING_DELAY_FORMAT](#LEVELING-DELAY-FORMAT) | The format of expressing the duration of a delay. |
| [LEVEL_ASSIGNMENTS](#LEVEL-ASSIGNMENTS) | Determines whether the leveling function can delay and split individual assignments in order to resolve over allocations. |
| [MANUAL_DURATION](#MANUAL-DURATION) | Defines manually scheduled duration of a task. |
| [MANUAL_FINISH](#MANUAL-FINISH) | Defines manually scheduled finish of a task. |
| [MANUAL_START](#MANUAL-START) | Defines manually scheduled start of a task. |
| [NAME](#NAME) | A task's name. |
| [NOTES_RTF](#NOTES-RTF) | The text notes in RTF format. |
| [NOTES_TEXT](#NOTES-TEXT) | Notes' plain text extracted from RTF data. |
| [OUTLINE_LEVEL](#OUTLINE-LEVEL) | The outline level of a task. |
| [OUTLINE_NUMBER](#OUTLINE-NUMBER) | The number that represents a task's position in the hierarchical outline structure. |
| [OVERTIME_COST](#OVERTIME-COST) | The total overtime cost for a task, for a resource on all assigned tasks, or for a resource assignment. |
| [OVERTIME_WORK](#OVERTIME-WORK) | The amount of overtime scheduled to be performed by all resources assigned to a task. |
| [PERCENT_COMPLETE](#PERCENT-COMPLETE) | The current status of a task, expressed as the percentage of the task's duration that has been completed. |
| [PERCENT_WORK_COMPLETE](#PERCENT-WORK-COMPLETE) | The current status of a task expressed as the percentage of work that has been completed. |
| [PHYSICAL_PERCENT_COMPLETE](#PHYSICAL-PERCENT-COMPLETE) | Percent complete value that can be be used as an alternative for calculating budgeted cost of work performed (BCWP). |
| [PRELEVELED_FINISH](#PRELEVELED-FINISH) | The finish date of a task as it was before resource leveling was done. |
| [PRELEVELED_START](#PRELEVELED-START) | The start date of a task as it was before resource leveling was done. |
| [PRIORITY](#PRIORITY) | The level of importance given to a task, which in turn indicates how readily a task or assignment can be delayed or split during resource leveling. |
| [REGULAR_WORK](#REGULAR-WORK) | The total amount of non overtime work scheduled to be performed by resources. |
| [REMAINING_COST](#REMAINING-COST) | The remaining scheduled expense that will be incurred in completing the remaining scheduled work. |
| [REMAINING_DURATION](#REMAINING-DURATION) | The time that is required to complete the unfinished part of a task. |
| [REMAINING_OVERTIME_COST](#REMAINING-OVERTIME-COST) | The remaining scheduled overtime expense for a task. |
| [REMAINING_OVERTIME_WORK](#REMAINING-OVERTIME-WORK) | The amount of remaining scheduled overtime time. |
| [REMAINING_WORK](#REMAINING-WORK) | The time still required to complete a task or set of tasks. |
| [RESUME](#RESUME) | The date that the remaining part of a task is scheduled to resume after entering any progress. |
| [START](#START) | The scheduled start date of a task. |
| [START_SLACK_TIME_SPAN](#START-SLACK-TIME-SPAN) | The duration (in seconds) between the Early Start and Late Start dates. |
| [START_TEXT](#START-TEXT) | Returns the task's start text. |
| [START_VARIANCE](#START-VARIANCE) | The time that represents the difference between a baseline start date of a task or assignment and its currently scheduled start date. |
| [STATUS_MANAGER](#STATUS-MANAGER) | The name of the enterprise resource who is to receive status updates for the current task from resources. |
| [STOP](#STOP) | The date that represents the end of the actual portion of a task. |
| [SUBPROJECT_NAME](#SUBPROJECT-NAME) | The source location of a subproject. |
| [SV](#SV) | The earned value schedule variance, through the project status date. |
| [TOTAL_SLACK_TIME_SPAN](#TOTAL-SLACK-TIME-SPAN) | The time a task's finish date can be delayed without delaying the project's finish date. |
| [TYPE](#TYPE) | The type of a task. |
| [UID](#UID) | The unique Id of a task. |
| [WARNING](#WARNING) | Represents the flag which indicates that task has schedule discrepancies. |
| [WBS](#WBS) | Work breakdown structure (WBS) codes. |
| [WBS_LEVEL](#WBS-LEVEL) | The rightmost WBS level of a task. |
| [WORK](#WORK) | The total time scheduled on a task for all assigned resources. |
| [WORK_VARIANCE](#WORK-VARIANCE) | The difference between baseline work of a task and the currently scheduled work. |
### Tsk() {#Tsk--}
```
public Tsk()
```


### ACTIVITY_ID {#ACTIVITY-ID}
```
public static final Key<String,Integer> ACTIVITY_ID
```


Represents activity id field - a task's unique identifier used by Primavera. (only applicable to Primavera projects).

### ACTUAL_COST {#ACTUAL-COST}
```
public static final Key<BigDecimal,Integer> ACTUAL_COST
```


Costs incurred for work already performed by resources on their tasks, together with any other recorded costs associated with the task.

### ACTUAL_DURATION {#ACTUAL-DURATION}
```
public static final Key<Duration,Integer> ACTUAL_DURATION
```


The span of actual working time for a task, based on the scheduled duration and current remaining work or percent complete.

### ACTUAL_FINISH {#ACTUAL-FINISH}
```
public static final Key<Date,Integer> ACTUAL_FINISH
```


The date when a task was completed.

### ACTUAL_OVERTIME_COST {#ACTUAL-OVERTIME-COST}
```
public static final Key<BigDecimal,Integer> ACTUAL_OVERTIME_COST
```


Costs incurred for overtime work already performed on tasks by assigned resources.

### ACTUAL_OVERTIME_WORK {#ACTUAL-OVERTIME-WORK}
```
public static final Key<Duration,Integer> ACTUAL_OVERTIME_WORK
```


The actual amount of overtime work already performed by resources assigned to tasks.

### ACTUAL_OVERTIME_WORK_PROTECTED {#ACTUAL-OVERTIME-WORK-PROTECTED}
```
public static final Key<Duration,Integer> ACTUAL_OVERTIME_WORK_PROTECTED
```


The duration through which actual overtime work is protected.

### ACTUAL_START {#ACTUAL-START}
```
public static final Key<Date,Integer> ACTUAL_START
```


The date and time that a task actually began.

### ACTUAL_WORK {#ACTUAL-WORK}
```
public static final Key<Duration,Integer> ACTUAL_WORK
```


The amount of work that has already been done by resources assigned to tasks.

### ACTUAL_WORK_PROTECTED {#ACTUAL-WORK-PROTECTED}
```
public static final Key<Duration,Integer> ACTUAL_WORK_PROTECTED
```


The duration through which actual work is protected.

--------------------

Reading supported for XML format only.

### ACWP {#ACWP}
```
public static final Key<Double,Integer> ACWP
```


Costs incurred for work already done on a task, up to the project status date or today's date.

### BCWP {#BCWP}
```
public static final Key<Double,Integer> BCWP
```


The cumulative value of the task's percent complete multiplied by the time phased baseline costs.

### BCWS {#BCWS}
```
public static final Key<Double,Integer> BCWS
```


The cumulative time phased baseline costs up to the status date or today's date.

### BUDGET_COST {#BUDGET-COST}
```
public static final Key<BigDecimal,Integer> BUDGET_COST
```


Budget costs for budget cost resources. Budget resources are assigned only to the project summary task.

### BUDGET_WORK {#BUDGET-WORK}
```
public static final Key<Duration,Integer> BUDGET_WORK
```


Budget work for budget work and material resources. Budget resources are assigned only to the project summary task.

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Integer> CALENDAR
```


The task calendar.

### COMMITMENT_FINISH {#COMMITMENT-FINISH}
```
public static final Key<Date,Integer> COMMITMENT_FINISH
```


The finish date of a delivery.

--------------------

Reading supported for XML format only.

### COMMITMENT_START {#COMMITMENT-START}
```
public static final Key<Date,Integer> COMMITMENT_START
```


The start date of a delivery.

--------------------

Reading supported for XML format only.

### COMMITMENT_TYPE {#COMMITMENT-TYPE}
```
public static final Key<Integer,Integer> COMMITMENT_TYPE
```


Determines whether a task has an associated delivery or a dependency on an associated delivery.

--------------------

Reading supported for XML format only.

### CONSTRAINT_DATE {#CONSTRAINT-DATE}
```
public static final Key<Date,Integer> CONSTRAINT_DATE
```


The specific date associated with the constraint type.

### CONSTRAINT_TYPE {#CONSTRAINT-TYPE}
```
public static final Key<Integer,Integer> CONSTRAINT_TYPE
```


Provides choices for the type of constraint that can be applied for scheduling a task.

### CONTACT {#CONTACT}
```
public static final Key<String,Integer> CONTACT
```


The name of an individual responsible for a task.

### COST {#COST}
```
public static final Key<BigDecimal,Integer> COST
```


The total scheduled or projected cost for a task based on costs already incurred for work performed by resources assigned to the tasks, in addition to the costs planned for the remaining work.

### COST_VARIANCE {#COST-VARIANCE}
```
public static final Key<Double,Integer> COST_VARIANCE
```


The difference between the baseline cost and total cost for a task, resource, or assignment.

### CREATED {#CREATED}
```
public static final Key<Date,Integer> CREATED
```


The date when a task was created.

### CV {#CV}
```
public static final Key<Double,Integer> CV
```


The difference between the baseline cost and total cost for a task. Cost Variance = Cost - Baseline Cost

### DEADLINE {#DEADLINE}
```
public static final Key<Date,Integer> DEADLINE
```


A target date that indicates when a task is to be completed.

### DISPLAY_AS_SUMMARY {#DISPLAY-AS-SUMMARY}
```
public static final Key<NullableBool,Integer> DISPLAY_AS_SUMMARY
```


Determines whether the task should be displayed as a summary task.

--------------------

Reading supported for XML format only.

### DISPLAY_ON_TIMELINE {#DISPLAY-ON-TIMELINE}
```
public static final Key<Boolean,Integer> DISPLAY_ON_TIMELINE
```


Specifies whether a task should be displayed on a timeline view.

### DURATION {#DURATION}
```
public static final Key<Duration,Integer> DURATION
```


The total span of active working time for a task as entered or as calculated by Microsoft Project based on start date, finish date, calendars, and other scheduling factors.

### DURATION_FORMAT {#DURATION-FORMAT}
```
public static final Key<Integer,Integer> DURATION_FORMAT
```


Task duration format.

### DURATION_TEXT {#DURATION-TEXT}
```
public static final Key<String,Integer> DURATION_TEXT
```


Returns the task's duration text.

### DURATION_VARIANCE {#DURATION-VARIANCE}
```
public static final Key<Duration,Integer> DURATION_VARIANCE
```


The difference between the baseline duration of a task and the total duration (current estimate) of a task.

### EARLY_FINISH {#EARLY-FINISH}
```
public static final Key<Date,Integer> EARLY_FINISH
```


The earliest date that a task could possibly finish, based on early finish dates of predecessor and successor tasks, other constraints, and any leveling delay.

### EARLY_START {#EARLY-START}
```
public static final Key<Date,Integer> EARLY_START
```


The earliest date that a task could possibly begin, based on the early start dates of predecessor and successor tasks and other constraints.

### EARNED_VALUE_METHOD {#EARNED-VALUE-METHOD}
```
public static final Key<Integer,Integer> EARNED_VALUE_METHOD
```


Determines whether the % Complete or Physical % Complete field should be used to calculate budgeted cost of work performed (BCWP).

### EXTERNAL_ID {#EXTERNAL-ID}
```
public static final Key<Integer,Integer> EXTERNAL_ID
```


If a task is an external task it contains the task's external Id.

### EXTERNAL_TASK_PROJECT {#EXTERNAL-TASK-PROJECT}
```
public static final Key<String,Integer> EXTERNAL_TASK_PROJECT
```


The source location and task identifier of an external task.

### EXTERNAL_UID {#EXTERNAL-UID}
```
public static final Key<Integer,Integer> EXTERNAL_UID
```


Contains the external task's Unique identifier when the task is external.

### FINISH {#FINISH}
```
public static final Key<Date,Integer> FINISH
```


The scheduled finish date of a task.

### FINISH_SLACK_TIME_SPAN {#FINISH-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Integer> FINISH_SLACK_TIME_SPAN
```


The duration (in seconds) between the Early Finish and Late Finish dates.

### FINISH_TEXT {#FINISH-TEXT}
```
public static final Key<String,Integer> FINISH_TEXT
```


Returns the task's finish text.

### FINISH_VARIANCE {#FINISH-VARIANCE}
```
public static final Key<Duration,Integer> FINISH_VARIANCE
```


The time that represents the difference between the baseline finish date of a task or assignment and its current finish date.

### FIXED_COST {#FIXED-COST}
```
public static final Key<Double,Integer> FIXED_COST
```


Shows any non resource task expense.

### FIXED_COST_ACCRUAL {#FIXED-COST-ACCRUAL}
```
public static final Key<Integer,Integer> FIXED_COST_ACCRUAL
```


Determines choices for how and when fixed costs are to be charged, or accrued, to the cost of a task.

### FREE_SLACK_TIME_SPAN {#FREE-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Integer> FREE_SLACK_TIME_SPAN
```


The time (in seconds) that a task can be delayed without delaying any successor tasks.

### GUID {#GUID}
```
public static final Key<String,Integer> GUID
```


The generated unique identification codes for a task.

### HAS_OVERALLOCATED_RESOURCE {#HAS-OVERALLOCATED-RESOURCE}
```
public static final Key<NullableBool,Integer> HAS_OVERALLOCATED_RESOURCE
```


Indicates whether the task has an resource assigned which has more work on assigned tasks than can be completed within normal working capacity.

### HIDE_BAR {#HIDE-BAR}
```
public static final Key<NullableBool,Integer> HIDE_BAR
```


Determines whether the Gantt bar of a task is hidden when displayed in Microsoft Project.

### HYPERLINK {#HYPERLINK}
```
public static final Key<String,Integer> HYPERLINK
```


The title or explanatory text for a hyperlink associated with a task.

### HYPERLINK_ADDRESS {#HYPERLINK-ADDRESS}
```
public static final Key<String,Integer> HYPERLINK_ADDRESS
```


The address for a hyperlink associated with a task.

### HYPERLINK_SUB_ADDRESS {#HYPERLINK-SUB-ADDRESS}
```
public static final Key<String,Integer> HYPERLINK_SUB_ADDRESS
```


The specific location in a document in a hyperlink associated with a task.

### ID {#ID}
```
public static final Key<Integer,Integer> ID
```


The position identifier of a task within the list of tasks.

### IGNORE_RESOURCE_CALENDAR {#IGNORE-RESOURCE-CALENDAR}
```
public static final Key<NullableBool,Integer> IGNORE_RESOURCE_CALENDAR
```


Determines whether the scheduling of the task considers the calendars of the resources assigned to the task.

### IGNORE_WARNINGS {#IGNORE-WARNINGS}
```
public static final Key<Boolean,Integer> IGNORE_WARNINGS
```


Indicates whether to hide the schedule conflict warning indicator in Microsoft Project.

### IS_ACTIVE {#IS-ACTIVE}
```
public static final Key<NullableBool,Integer> IS_ACTIVE
```


Determines whether a task is active. Inactive tasks no longer affect other tasks or the overall Project schedule.

### IS_CRITICAL {#IS-CRITICAL}
```
public static final Key<NullableBool,Integer> IS_CRITICAL
```


Determines whether a task is on the critical path.

### IS_EFFORT_DRIVEN {#IS-EFFORT-DRIVEN}
```
public static final Key<NullableBool,Integer> IS_EFFORT_DRIVEN
```


Determines whether the scheduling for the task is effort-driven scheduling.

### IS_ESTIMATED {#IS-ESTIMATED}
```
public static final Key<NullableBool,Integer> IS_ESTIMATED
```


Determines whether a task is estimated.

### IS_EXPANDED {#IS-EXPANDED}
```
public static final Key<NullableBool,Integer> IS_EXPANDED
```


Determines whether a summary task is expanded or not in GanttChart view.

### IS_EXTERNAL_TASK {#IS-EXTERNAL-TASK}
```
public static final Key<Boolean,Integer> IS_EXTERNAL_TASK
```


Determines whether a task is external.

### IS_MANUAL {#IS-MANUAL}
```
public static final Key<NullableBool,Integer> IS_MANUAL
```


Determines whether a task is manually scheduled.

### IS_MARKED {#IS-MARKED}
```
public static final Key<Boolean,Integer> IS_MARKED
```


Shows whether a task is marked for further action or identification of some kind.

--------------------

Applies to mpp file format only.

### IS_MILESTONE {#IS-MILESTONE}
```
public static final Key<NullableBool,Integer> IS_MILESTONE
```


Determines whether a task is a milestone.

### IS_NULL {#IS-NULL}
```
public static final Key<NullableBool,Integer> IS_NULL
```


Determines whether a task is a null task.

### IS_OVERALLOCATED {#IS-OVERALLOCATED}
```
public static final Key<NullableBool,Integer> IS_OVERALLOCATED
```


Indicates whether any of the assigned resources on a task is assigned to more work on the task than can be done withing the normal working capacity.

### IS_PUBLISHED {#IS-PUBLISHED}
```
public static final Key<NullableBool,Integer> IS_PUBLISHED
```


Determines whether the current task should be published to Project Server with the rest of the project.

### IS_RECURRING {#IS-RECURRING}
```
public static final Key<NullableBool,Integer> IS_RECURRING
```


Determines whether a task is part of a series of recurring tasks.

### IS_RESUME_VALID {#IS-RESUME-VALID}
```
public static final Key<NullableBool,Integer> IS_RESUME_VALID
```


Determines whether a task can be resumed.

### IS_ROLLUP {#IS-ROLLUP}
```
public static final Key<NullableBool,Integer> IS_ROLLUP
```


Determines whether information about the subtask Gantt bars will be rolled up to the summary task bar.

### IS_SUBPROJECT {#IS-SUBPROJECT}
```
public static final Key<Boolean,Integer> IS_SUBPROJECT
```


Determines whether a task is an inserted project.

### IS_SUBPROJECT_READ_ONLY {#IS-SUBPROJECT-READ-ONLY}
```
public static final Key<NullableBool,Integer> IS_SUBPROJECT_READ_ONLY
```


Determines whether a subproject is read-only.

### IS_SUMMARY {#IS-SUMMARY}
```
public static final Key<Boolean,Integer> IS_SUMMARY
```


Determines whether a task is a summary task.

### LATE_FINISH {#LATE-FINISH}
```
public static final Key<Date,Integer> LATE_FINISH
```


The latest date that a task can finish without delaying the finish of the project.

### LATE_START {#LATE-START}
```
public static final Key<Date,Integer> LATE_START
```


The latest date that a task can start without delaying the finish of the project.

### LEVELING_CAN_SPLIT {#LEVELING-CAN-SPLIT}
```
public static final Key<NullableBool,Integer> LEVELING_CAN_SPLIT
```


Determines whether the resource leveling function can cause splits on remaining work on this task.

### LEVELING_DELAY {#LEVELING-DELAY}
```
public static final Key<Duration,Integer> LEVELING_DELAY
```


The time that a task is to be delayed from its early start date because of resource leveling.

### LEVELING_DELAY_FORMAT {#LEVELING-DELAY-FORMAT}
```
public static final Key<Integer,Integer> LEVELING_DELAY_FORMAT
```


The format of expressing the duration of a delay.

### LEVEL_ASSIGNMENTS {#LEVEL-ASSIGNMENTS}
```
public static final Key<NullableBool,Integer> LEVEL_ASSIGNMENTS
```


Determines whether the leveling function can delay and split individual assignments in order to resolve over allocations.

### MANUAL_DURATION {#MANUAL-DURATION}
```
public static final Key<Duration,Integer> MANUAL_DURATION
```


Defines manually scheduled duration of a task.

### MANUAL_FINISH {#MANUAL-FINISH}
```
public static final Key<Date,Integer> MANUAL_FINISH
```


Defines manually scheduled finish of a task.

### MANUAL_START {#MANUAL-START}
```
public static final Key<Date,Integer> MANUAL_START
```


Defines manually scheduled start of a task.

### NAME {#NAME}
```
public static final Key<String,Integer> NAME
```


A task's name.

### NOTES_RTF {#NOTES-RTF}
```
public static final Key<String,Integer> NOTES_RTF
```


The text notes in RTF format.

### NOTES_TEXT {#NOTES-TEXT}
```
public static final Key<String,Integer> NOTES_TEXT
```


Notes' plain text extracted from RTF data.

### OUTLINE_LEVEL {#OUTLINE-LEVEL}
```
public static final Key<Integer,Integer> OUTLINE_LEVEL
```


The outline level of a task.

### OUTLINE_NUMBER {#OUTLINE-NUMBER}
```
public static final Key<String,Integer> OUTLINE_NUMBER
```


The number that represents a task's position in the hierarchical outline structure.

### OVERTIME_COST {#OVERTIME-COST}
```
public static final Key<BigDecimal,Integer> OVERTIME_COST
```


The total overtime cost for a task, for a resource on all assigned tasks, or for a resource assignment.

### OVERTIME_WORK {#OVERTIME-WORK}
```
public static final Key<Duration,Integer> OVERTIME_WORK
```


The amount of overtime scheduled to be performed by all resources assigned to a task.

### PERCENT_COMPLETE {#PERCENT-COMPLETE}
```
public static final Key<Integer,Integer> PERCENT_COMPLETE
```


The current status of a task, expressed as the percentage of the task's duration that has been completed.

### PERCENT_WORK_COMPLETE {#PERCENT-WORK-COMPLETE}
```
public static final Key<Integer,Integer> PERCENT_WORK_COMPLETE
```


The current status of a task expressed as the percentage of work that has been completed.

### PHYSICAL_PERCENT_COMPLETE {#PHYSICAL-PERCENT-COMPLETE}
```
public static final Key<Integer,Integer> PHYSICAL_PERCENT_COMPLETE
```


Percent complete value that can be be used as an alternative for calculating budgeted cost of work performed (BCWP).

### PRELEVELED_FINISH {#PRELEVELED-FINISH}
```
public static final Key<Date,Integer> PRELEVELED_FINISH
```


The finish date of a task as it was before resource leveling was done.

### PRELEVELED_START {#PRELEVELED-START}
```
public static final Key<Date,Integer> PRELEVELED_START
```


The start date of a task as it was before resource leveling was done.

### PRIORITY {#PRIORITY}
```
public static final Key<Integer,Integer> PRIORITY
```


The level of importance given to a task, which in turn indicates how readily a task or assignment can be delayed or split during resource leveling.

### REGULAR_WORK {#REGULAR-WORK}
```
public static final Key<Duration,Integer> REGULAR_WORK
```


The total amount of non overtime work scheduled to be performed by resources.

### REMAINING_COST {#REMAINING-COST}
```
public static final Key<BigDecimal,Integer> REMAINING_COST
```


The remaining scheduled expense that will be incurred in completing the remaining scheduled work.

### REMAINING_DURATION {#REMAINING-DURATION}
```
public static final Key<Duration,Integer> REMAINING_DURATION
```


The time that is required to complete the unfinished part of a task.

### REMAINING_OVERTIME_COST {#REMAINING-OVERTIME-COST}
```
public static final Key<BigDecimal,Integer> REMAINING_OVERTIME_COST
```


The remaining scheduled overtime expense for a task.

### REMAINING_OVERTIME_WORK {#REMAINING-OVERTIME-WORK}
```
public static final Key<Duration,Integer> REMAINING_OVERTIME_WORK
```


The amount of remaining scheduled overtime time.

### REMAINING_WORK {#REMAINING-WORK}
```
public static final Key<Duration,Integer> REMAINING_WORK
```


The time still required to complete a task or set of tasks.

### RESUME {#RESUME}
```
public static final Key<Date,Integer> RESUME
```


The date that the remaining part of a task is scheduled to resume after entering any progress.

### START {#START}
```
public static final Key<Date,Integer> START
```


The scheduled start date of a task.

### START_SLACK_TIME_SPAN {#START-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Integer> START_SLACK_TIME_SPAN
```


The duration (in seconds) between the Early Start and Late Start dates.

### START_TEXT {#START-TEXT}
```
public static final Key<String,Integer> START_TEXT
```


Returns the task's start text.

### START_VARIANCE {#START-VARIANCE}
```
public static final Key<Duration,Integer> START_VARIANCE
```


The time that represents the difference between a baseline start date of a task or assignment and its currently scheduled start date.

### STATUS_MANAGER {#STATUS-MANAGER}
```
public static final Key<String,Integer> STATUS_MANAGER
```


The name of the enterprise resource who is to receive status updates for the current task from resources.

### STOP {#STOP}
```
public static final Key<Date,Integer> STOP
```


The date that represents the end of the actual portion of a task.

### SUBPROJECT_NAME {#SUBPROJECT-NAME}
```
public static final Key<String,Integer> SUBPROJECT_NAME
```


The source location of a subproject.

### SV {#SV}
```
public static final Key<Double,Integer> SV
```


The earned value schedule variance, through the project status date. Schedule variance (SV) is the difference between the BCWP and the BCWS.

### TOTAL_SLACK_TIME_SPAN {#TOTAL-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Integer> TOTAL_SLACK_TIME_SPAN
```


The time a task's finish date can be delayed without delaying the project's finish date.

### TYPE {#TYPE}
```
public static final Key<Integer,Integer> TYPE
```


The type of a task.

### UID {#UID}
```
public static final Key<Integer,Integer> UID
```


The unique Id of a task.

### WARNING {#WARNING}
```
public static final Key<Boolean,Integer> WARNING
```


Represents the flag which indicates that task has schedule discrepancies.

### WBS {#WBS}
```
public static final Key<String,Integer> WBS
```


Work breakdown structure (WBS) codes.

### WBS_LEVEL {#WBS-LEVEL}
```
public static final Key<String,Integer> WBS_LEVEL
```


The rightmost WBS level of a task.

### WORK {#WORK}
```
public static final Key<Duration,Integer> WORK
```


The total time scheduled on a task for all assigned resources.

### WORK_VARIANCE {#WORK-VARIANCE}
```
public static final Key<Duration,Integer> WORK_VARIANCE
```


The difference between baseline work of a task and the currently scheduled work.

