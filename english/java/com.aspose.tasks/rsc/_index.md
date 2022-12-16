---
title: Rsc
second_title: Aspose.Tasks for Java API Reference
description: Represents supported properties of Resource object.
type: docs
weight: 245
url: /java/com.aspose.tasks/rsc/
---

**Inheritance:**
java.lang.Object
```
public class Rsc
```

Represents supported properties of  Resource  object.
## Fields

| Field | Description |
| --- | --- |
| [ACCRUE_AT](#ACCRUE-AT) | Determines how and when resource standard and overtime costs are to be charged, or accrued, to the cost of a task. |
| [ACTIVE_DIRECTORY_GUID](#ACTIVE-DIRECTORY-GUID) | The Active Directory Guid for a resource. |
| [ACTUAL_COST](#ACTUAL-COST) | Costs incurred for work already performed by resources on their tasks, along with any other recorded costs associated with the task. |
| [ACTUAL_OVERTIME_COST](#ACTUAL-OVERTIME-COST) | Costs incurred for overtime work already performed on tasks by assigned resources. |
| [ACTUAL_OVERTIME_WORK](#ACTUAL-OVERTIME-WORK) | The actual amount of overtime work already performed by resource assigned to tasks. |
| [ACTUAL_OVERTIME_WORK_PROTECTED](#ACTUAL-OVERTIME-WORK-PROTECTED) | The amount of work through which actual overtime work is protected. |
| [ACTUAL_WORK](#ACTUAL-WORK) | The amount of work that has already been done by resource assigned to tasks. |
| [ACTUAL_WORK_PROTECTED](#ACTUAL-WORK-PROTECTED) | The amount of work through which actual work is protected. |
| [ACWP](#ACWP) | The actual cost of a work performed by a resource for the project to-date. |
| [ASSIGNMENT_OWNER](#ASSIGNMENT-OWNER) | The name of an assignment owner. |
| [ASSIGNMENT_OWNER_GUID](#ASSIGNMENT-OWNER-GUID) | The GUID of an assignment owner. |
| [AVAILABLE_FROM](#AVAILABLE-FROM) | The starting date that a resource is available for work at the units specified for the current time period. |
| [AVAILABLE_TO](#AVAILABLE-TO) | The end date that a resource is available for work at the units specified for the current time period. |
| [BCWP](#BCWP) | The budgeted cost of a work performed by a resource for the project to-date. |
| [BCWS](#BCWS) | The budget cost of a work scheduled for a resource. |
| [BOOKING_TYPE](#BOOKING-TYPE) | The booking type of a resource. |
| [BUDGET_COST](#BUDGET-COST) | Budget costs for budget cost resources. |
| [BUDGET_WORK](#BUDGET-WORK) | budget work for budget work and material resources. |
| [CALENDAR](#CALENDAR) | The calendar of a resource. |
| [CAN_LEVEL](#CAN-LEVEL) | Determines whether resource leveling can be done on a resource. |
| [CODE](#CODE) | The code or other information about a resource. |
| [COST](#COST) | The total scheduled or projected cost for a resource, based on costs already incurred for work performed by resources assigned to the tasks, in addition to the costs planned for the remaining work. |
| [COST_CENTER](#COST-CENTER) | Indicates which cost center the costs accrued by the resource should be charged to. |
| [COST_PER_USE](#COST-PER-USE) | The cost that accrues every time that a resource is used. |
| [COST_VARIANCE](#COST-VARIANCE) | The difference between the baseline cost and total cost for a resource. |
| [CREATED](#CREATED) | The date and time when a resource was added to the project. |
| [CV](#CV) | The earned value cost variance, through the project status date. |
| [E_MAIL_ADDRESS](#E-MAIL-ADDRESS) | The email address of a resource. |
| [FINISH](#FINISH) | The date when a resource is scheduled to complete work on all assigned tasks. |
| [GROUP](#GROUP) | The group to which a resource belongs. |
| [GUID](#GUID) | Contains the generated unique identification code for the resource. |
| [HYPERLINK](#HYPERLINK) | The title of a hyperlink associated with a resource. |
| [HYPERLINK_ADDRESS](#HYPERLINK-ADDRESS) | The hyperlink associated with a resource. |
| [HYPERLINK_SUB_ADDRESS](#HYPERLINK-SUB-ADDRESS) | The document bookmark of a hyperlink associated with a resource. |
| [ID](#ID) | The position identifier of a resource within the list of resources. |
| [INACTIVE](#INACTIVE) | Determines whether a resource was made inactive by a user who has administrative rights. |
| [INITIALS](#INITIALS) | The initials of a resource. |
| [IS_BUDGET](#IS-BUDGET) | Determines whether a work, material, or cost resource is a budget resource. |
| [IS_COST_RESOURCE](#IS-COST-RESOURCE) | Determines whether a resource is a cost resource. |
| [IS_ENTERPRISE](#IS-ENTERPRISE) | Shows whether a resource is from the enterprise resource pool (true) or the local resource pool (false). |
| [IS_GENERIC](#IS-GENERIC) | Determines whether a resource is generic or not. |
| [IS_NULL](#IS-NULL) | Determines whether a resource is null. |
| [IS_TEAM_ASSIGNMENT_POOL](#IS-TEAM-ASSIGNMENT-POOL) | Shows whether the current resource is a team resource. |
| [MATERIAL_LABEL](#MATERIAL-LABEL) | The unit of measure for the material resource. |
| [MAX_UNITS](#MAX-UNITS) | The maximum number of units representing the maximum capacity for which a resource is available to accomplish any tasks during the current time period. |
| [NAME](#NAME) | The name of a resource. |
| [NOTES](#NOTES) | The text notes associated with a resource. |
| [NOTES_RTF](#NOTES-RTF) | The text notes in RTF format. |
| [NOTES_TEXT](#NOTES-TEXT) | Notes' plain text extracted from RTF data. |
| [OVERALLOCATED](#OVERALLOCATED) | Indicates whether a resource is assigned to more work on a specific task or all tasks than can be completed within normal working capacity. |
| [OVERTIME_COST](#OVERTIME-COST) | The total overtime cost for a resource on all assigned tasks. |
| [OVERTIME_RATE](#OVERTIME-RATE) | The rate of pay for overtime work performed by a resource. |
| [OVERTIME_RATE_FORMAT](#OVERTIME-RATE-FORMAT) | The units used by Microsoft Project to display the overtime rate. |
| [OVERTIME_WORK](#OVERTIME-WORK) | The amount of overtime scheduled to be performed by a resource on a task and charged at the overtime rates of the resources involved. |
| [PEAK_UNITS](#PEAK-UNITS) | The maximum assignment unit for a resource at any one point in time for all tasks to which the resource is assigned. |
| [PERCENT_WORK_COMPLETE](#PERCENT-WORK-COMPLETE) | The percentage of work completed across all tasks. |
| [PHONETICS](#PHONETICS) | The phonetic spelling of the resource name. |
| [REGULAR_WORK](#REGULAR-WORK) | The total amount of non overtime work scheduled to be performed by resource. |
| [REMAINING_COST](#REMAINING-COST) | The remaining scheduled expense that will be incurred in completing the remaining scheduled work. |
| [REMAINING_OVERTIME_COST](#REMAINING-OVERTIME-COST) | The remaining scheduled overtime expense for a resource. |
| [REMAINING_OVERTIME_WORK](#REMAINING-OVERTIME-WORK) | The amount of remaining scheduled overtime. |
| [REMAINING_WORK](#REMAINING-WORK) | The time still required to complete a task or set of tasks. |
| [STANDARD_RATE](#STANDARD-RATE) | The rate of pay for regular, non-overtime work performed by a resource. |
| [STANDARD_RATE_FORMAT](#STANDARD-RATE-FORMAT) | The units used by Microsoft Project to display the standard rate. |
| [START](#START) | The date when an assigned resource is scheduled to begin working on a task. |
| [SV](#SV) | The earned value schedule variance, through the project status date. |
| [TYPE](#TYPE) | The type of a resource. |
| [UID](#UID) | The unique identifier of a resource. |
| [WINDOWS_USER_ACCOUNT](#WINDOWS-USER-ACCOUNT) | The NT account associated with a resource. |
| [WORK](#WORK) | The total amount of time scheduled for a resource on a task. |
| [WORKGROUP](#WORKGROUP) | The type of a workgroup to which a resource belongs. |
| [WORK_VARIANCE](#WORK-VARIANCE) | The difference between baseline work of a resource and the currently scheduled work. |
### ACCRUE_AT {#ACCRUE-AT}
```
public static final Key<Integer,Integer> ACCRUE_AT
```


Determines how and when resource standard and overtime costs are to be charged, or accrued, to the cost of a task.

### ACTIVE_DIRECTORY_GUID {#ACTIVE-DIRECTORY-GUID}
```
public static final Key<String,Integer> ACTIVE_DIRECTORY_GUID
```


The Active Directory Guid for a resource.

### ACTUAL_COST {#ACTUAL-COST}
```
public static final Key<BigDecimal,Integer> ACTUAL_COST
```


Costs incurred for work already performed by resources on their tasks, along with any other recorded costs associated with the task.

### ACTUAL_OVERTIME_COST {#ACTUAL-OVERTIME-COST}
```
public static final Key<BigDecimal,Integer> ACTUAL_OVERTIME_COST
```


Costs incurred for overtime work already performed on tasks by assigned resources.

### ACTUAL_OVERTIME_WORK {#ACTUAL-OVERTIME-WORK}
```
public static final Key<Duration,Integer> ACTUAL_OVERTIME_WORK
```


The actual amount of overtime work already performed by resource assigned to tasks.

### ACTUAL_OVERTIME_WORK_PROTECTED {#ACTUAL-OVERTIME-WORK-PROTECTED}
```
public static final Key<Duration,Integer> ACTUAL_OVERTIME_WORK_PROTECTED
```


The amount of work through which actual overtime work is protected.

### ACTUAL_WORK {#ACTUAL-WORK}
```
public static final Key<Duration,Integer> ACTUAL_WORK
```


The amount of work that has already been done by resource assigned to tasks.

### ACTUAL_WORK_PROTECTED {#ACTUAL-WORK-PROTECTED}
```
public static final Key<Duration,Integer> ACTUAL_WORK_PROTECTED
```


The amount of work through which actual work is protected.

### ACWP {#ACWP}
```
public static final Key<Double,Integer> ACWP
```


The actual cost of a work performed by a resource for the project to-date.

### ASSIGNMENT_OWNER {#ASSIGNMENT-OWNER}
```
public static final Key<String,Integer> ASSIGNMENT_OWNER
```


The name of an assignment owner.

### ASSIGNMENT_OWNER_GUID {#ASSIGNMENT-OWNER-GUID}
```
public static final Key<String,Integer> ASSIGNMENT_OWNER_GUID
```


The GUID of an assignment owner.

### AVAILABLE_FROM {#AVAILABLE-FROM}
```
public static final Key<Date,Integer> AVAILABLE_FROM
```


The starting date that a resource is available for work at the units specified for the current time period.

### AVAILABLE_TO {#AVAILABLE-TO}
```
public static final Key<Date,Integer> AVAILABLE_TO
```


The end date that a resource is available for work at the units specified for the current time period.

### BCWP {#BCWP}
```
public static final Key<Double,Integer> BCWP
```


The budgeted cost of a work performed by a resource for the project to-date.

### BCWS {#BCWS}
```
public static final Key<Double,Integer> BCWS
```


The budget cost of a work scheduled for a resource.

### BOOKING_TYPE {#BOOKING-TYPE}
```
public static final Key<Integer,Integer> BOOKING_TYPE
```


The booking type of a resource.

### BUDGET_COST {#BUDGET-COST}
```
public static final Key<BigDecimal,Integer> BUDGET_COST
```


Budget costs for budget cost resources. Budget resources are assigned only to the project summary task.

### BUDGET_WORK {#BUDGET-WORK}
```
public static final Key<Duration,Integer> BUDGET_WORK
```


budget work for budget work and material resources. Budget resources are assigned only to the project summary task.

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Integer> CALENDAR
```


The calendar of a resource.

### CAN_LEVEL {#CAN-LEVEL}
```
public static final Key<NullableBool,Integer> CAN_LEVEL
```


Determines whether resource leveling can be done on a resource.

### CODE {#CODE}
```
public static final Key<String,Integer> CODE
```


The code or other information about a resource.

### COST {#COST}
```
public static final Key<BigDecimal,Integer> COST
```


The total scheduled or projected cost for a resource, based on costs already incurred for work performed by resources assigned to the tasks, in addition to the costs planned for the remaining work.

### COST_CENTER {#COST-CENTER}
```
public static final Key<String,Integer> COST_CENTER
```


Indicates which cost center the costs accrued by the resource should be charged to.

### COST_PER_USE {#COST-PER-USE}
```
public static final Key<BigDecimal,Integer> COST_PER_USE
```


The cost that accrues every time that a resource is used.

### COST_VARIANCE {#COST-VARIANCE}
```
public static final Key<Double,Integer> COST_VARIANCE
```


The difference between the baseline cost and total cost for a resource.

### CREATED {#CREATED}
```
public static final Key<Date,Integer> CREATED
```


The date and time when a resource was added to the project.

### CV {#CV}
```
public static final Key<Double,Integer> CV
```


The earned value cost variance, through the project status date. CV is the difference between the task's BCWP (budgeted cost of work performed) and ACWP (actual cost of work performed).

### E_MAIL_ADDRESS {#E-MAIL-ADDRESS}
```
public static final Key<String,Integer> E_MAIL_ADDRESS
```


The email address of a resource.

### FINISH {#FINISH}
```
public static final Key<Date,Integer> FINISH
```


The date when a resource is scheduled to complete work on all assigned tasks.

### GROUP {#GROUP}
```
public static final Key<String,Integer> GROUP
```


The group to which a resource belongs.

### GUID {#GUID}
```
public static final Key<String,Integer> GUID
```


Contains the generated unique identification code for the resource.

### HYPERLINK {#HYPERLINK}
```
public static final Key<String,Integer> HYPERLINK
```


The title of a hyperlink associated with a resource.

### HYPERLINK_ADDRESS {#HYPERLINK-ADDRESS}
```
public static final Key<String,Integer> HYPERLINK_ADDRESS
```


The hyperlink associated with a resource.

### HYPERLINK_SUB_ADDRESS {#HYPERLINK-SUB-ADDRESS}
```
public static final Key<String,Integer> HYPERLINK_SUB_ADDRESS
```


The document bookmark of a hyperlink associated with a resource.

### ID {#ID}
```
public static final Key<Integer,Integer> ID
```


The position identifier of a resource within the list of resources.

### INACTIVE {#INACTIVE}
```
public static final Key<NullableBool,Integer> INACTIVE
```


Determines whether a resource was made inactive by a user who has administrative rights.

### INITIALS {#INITIALS}
```
public static final Key<String,Integer> INITIALS
```


The initials of a resource.

### IS_BUDGET {#IS-BUDGET}
```
public static final Key<NullableBool,Integer> IS_BUDGET
```


Determines whether a work, material, or cost resource is a budget resource.

### IS_COST_RESOURCE {#IS-COST-RESOURCE}
```
public static final Key<NullableBool,Integer> IS_COST_RESOURCE
```


Determines whether a resource is a cost resource.

### IS_ENTERPRISE {#IS-ENTERPRISE}
```
public static final Key<NullableBool,Integer> IS_ENTERPRISE
```


Shows whether a resource is from the enterprise resource pool (true) or the local resource pool (false).

### IS_GENERIC {#IS-GENERIC}
```
public static final Key<NullableBool,Integer> IS_GENERIC
```


Determines whether a resource is generic or not.

### IS_NULL {#IS-NULL}
```
public static final Key<NullableBool,Integer> IS_NULL
```


Determines whether a resource is null.

### IS_TEAM_ASSIGNMENT_POOL {#IS-TEAM-ASSIGNMENT-POOL}
```
public static final Key<Boolean,Integer> IS_TEAM_ASSIGNMENT_POOL
```


Shows whether the current resource is a team resource.

### MATERIAL_LABEL {#MATERIAL-LABEL}
```
public static final Key<String,Integer> MATERIAL_LABEL
```


The unit of measure for the material resource.

### MAX_UNITS {#MAX-UNITS}
```
public static final Key<Double,Integer> MAX_UNITS
```


The maximum number of units representing the maximum capacity for which a resource is available to accomplish any tasks during the current time period.

### NAME {#NAME}
```
public static final Key<String,Integer> NAME
```


The name of a resource.

### NOTES {#NOTES}
```
public static final Key<String,Integer> NOTES
```


The text notes associated with a resource.

### NOTES_RTF {#NOTES-RTF}
```
public static final Key<String,Integer> NOTES_RTF
```


The text notes in RTF format.

--------------------

Supported for MPP formats only.

### NOTES_TEXT {#NOTES-TEXT}
```
public static final Key<String,Integer> NOTES_TEXT
```


Notes' plain text extracted from RTF data.

### OVERALLOCATED {#OVERALLOCATED}
```
public static final Key<NullableBool,Integer> OVERALLOCATED
```


Indicates whether a resource is assigned to more work on a specific task or all tasks than can be completed within normal working capacity.

### OVERTIME_COST {#OVERTIME-COST}
```
public static final Key<BigDecimal,Integer> OVERTIME_COST
```


The total overtime cost for a resource on all assigned tasks.

### OVERTIME_RATE {#OVERTIME-RATE}
```
public static final Key<BigDecimal,Integer> OVERTIME_RATE
```


The rate of pay for overtime work performed by a resource.

### OVERTIME_RATE_FORMAT {#OVERTIME-RATE-FORMAT}
```
public static final Key<Integer,Integer> OVERTIME_RATE_FORMAT
```


The units used by Microsoft Project to display the overtime rate.

### OVERTIME_WORK {#OVERTIME-WORK}
```
public static final Key<Duration,Integer> OVERTIME_WORK
```


The amount of overtime scheduled to be performed by a resource on a task and charged at the overtime rates of the resources involved.

### PEAK_UNITS {#PEAK-UNITS}
```
public static final Key<Double,Integer> PEAK_UNITS
```


The maximum assignment unit for a resource at any one point in time for all tasks to which the resource is assigned.

### PERCENT_WORK_COMPLETE {#PERCENT-WORK-COMPLETE}
```
public static final Key<Integer,Integer> PERCENT_WORK_COMPLETE
```


The percentage of work completed across all tasks.

### PHONETICS {#PHONETICS}
```
public static final Key<String,Integer> PHONETICS
```


The phonetic spelling of the resource name. For use with Japanese only.

### REGULAR_WORK {#REGULAR-WORK}
```
public static final Key<Duration,Integer> REGULAR_WORK
```


The total amount of non overtime work scheduled to be performed by resource.

### REMAINING_COST {#REMAINING-COST}
```
public static final Key<BigDecimal,Integer> REMAINING_COST
```


The remaining scheduled expense that will be incurred in completing the remaining scheduled work.

### REMAINING_OVERTIME_COST {#REMAINING-OVERTIME-COST}
```
public static final Key<BigDecimal,Integer> REMAINING_OVERTIME_COST
```


The remaining scheduled overtime expense for a resource.

### REMAINING_OVERTIME_WORK {#REMAINING-OVERTIME-WORK}
```
public static final Key<Duration,Integer> REMAINING_OVERTIME_WORK
```


The amount of remaining scheduled overtime.

### REMAINING_WORK {#REMAINING-WORK}
```
public static final Key<Duration,Integer> REMAINING_WORK
```


The time still required to complete a task or set of tasks.

### STANDARD_RATE {#STANDARD-RATE}
```
public static final Key<BigDecimal,Integer> STANDARD_RATE
```


The rate of pay for regular, non-overtime work performed by a resource.

### STANDARD_RATE_FORMAT {#STANDARD-RATE-FORMAT}
```
public static final Key<Integer,Integer> STANDARD_RATE_FORMAT
```


The units used by Microsoft Project to display the standard rate.

### START {#START}
```
public static final Key<Date,Integer> START
```


The date when an assigned resource is scheduled to begin working on a task.

### SV {#SV}
```
public static final Key<Double,Integer> SV
```


The earned value schedule variance, through the project status date. SV is the difference between budgeted cost of work performed (BCWP) and budgeted cost of work scheduled (BCWS).

### TYPE {#TYPE}
```
public static final Key<Integer,Integer> TYPE
```


The type of a resource.

### UID {#UID}
```
public static final Key<Integer,Integer> UID
```


The unique identifier of a resource.

### WINDOWS_USER_ACCOUNT {#WINDOWS-USER-ACCOUNT}
```
public static final Key<String,Integer> WINDOWS_USER_ACCOUNT
```


The NT account associated with a resource.

### WORK {#WORK}
```
public static final Key<Duration,Integer> WORK
```


The total amount of time scheduled for a resource on a task.

### WORKGROUP {#WORKGROUP}
```
public static final Key<Integer,Integer> WORKGROUP
```


The type of a workgroup to which a resource belongs.

### WORK_VARIANCE {#WORK-VARIANCE}
```
public static final Key<Double,Integer> WORK_VARIANCE
```


The difference between baseline work of a resource and the currently scheduled work.
