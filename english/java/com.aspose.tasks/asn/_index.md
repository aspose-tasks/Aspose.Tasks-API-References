---
title: Asn
second_title: Aspose.Tasks for Java API Reference
description: Represents properties of  object.
type: docs
weight: 15
url: /java/com.aspose.tasks/asn/
---

**Inheritance:**
java.lang.Object
```
public class Asn
```

Represents properties of [ResourceAssignment](../../com.aspose.tasks/resourceassignment) object.
## Fields

| Field | Description |
| --- | --- |
| [ACTUAL_COST](#ACTUAL-COST) | The actual cost incurred on an assignment. |
| [ACTUAL_FINISH](#ACTUAL-FINISH) | The actual finish date of an assignment. |
| [ACTUAL_OVERTIME_COST](#ACTUAL-OVERTIME-COST) | The actual overtime cost incurred on an assignment. |
| [ACTUAL_OVERTIME_WORK](#ACTUAL-OVERTIME-WORK) | The actual amount of an overtime work incurred on an assignment. |
| [ACTUAL_OVERTIME_WORK_PROTECTED](#ACTUAL-OVERTIME-WORK-PROTECTED) | The duration through which actual work is protected. |
| [ACTUAL_START](#ACTUAL-START) | The actual start date of an assignment. |
| [ACTUAL_WORK](#ACTUAL-WORK) | The actual amount of a work incurred on an assignment. |
| [ACTUAL_WORK_PROTECTED](#ACTUAL-WORK-PROTECTED) | The duration through which actual overtime work is protected. |
| [ACWP](#ACWP) | The actual cost of a work performed on an assignment to-date. |
| [ASSIGNMENT_OWNER](#ASSIGNMENT-OWNER) | The name of an assignment owner. |
| [ASSIGNMENT_OWNER_GUID](#ASSIGNMENT-OWNER-GUID) | The globally unique identifier of an assignment owner. |
| [BCWP](#BCWP) | The budgeted cost of a work performed on assignment to-date. |
| [BCWS](#BCWS) | The budgeted cost of a work on assignment. |
| [BOOKING_TYPE](#BOOKING-TYPE) | The booking type of an assignment. |
| [BUDGET_COST](#BUDGET-COST) | The budgeted cost of resources on an assignment. |
| [BUDGET_WORK](#BUDGET-WORK) | The budgeted work amount for a work or material resources on an assignment. |
| [CONFIRMED](#CONFIRMED) | Determines whether a resource has accepted all of its assignments. |
| [COST](#COST) | The projected or scheduled cost of an assignment. |
| [COST_RATE_TABLE_TYPE](#COST-RATE-TABLE-TYPE) | The cost rate table used for this assignment. |
| [COST_VARIANCE](#COST-VARIANCE) | The difference between the baseline cost and total cost for an assignment. |
| [CREATED](#CREATED) | The date that the assignment was created. |
| [CV](#CV) | The earned value cost variance. |
| [DELAY](#DELAY) | The delay of an assignment. |
| [FINISH](#FINISH) | The scheduled finish date of an assignment. |
| [FINISH_VARIANCE](#FINISH-VARIANCE) | The variance of an assignment finish date from a baseline finish date. |
| [FIXED_MATERIAL](#FIXED-MATERIAL) | Determines whether the consumption of an assigned material resource occurs in a single, fixed amount. |
| [HAS_FIXED_RATE_UNITS](#HAS-FIXED-RATE-UNITS) | Determines whether the Units have Fixed Rate. |
| [HYPERLINK](#HYPERLINK) | The title or explanatory text of a hyperlink associated with an assignment. |
| [HYPERLINK_ADDRESS](#HYPERLINK-ADDRESS) | The address for a hyperlink associated with assignment. |
| [HYPERLINK_SUB_ADDRESS](#HYPERLINK-SUB-ADDRESS) | The specific location in a document in a hyperlink associated with an assignment. |
| [LEVELING_DELAY](#LEVELING-DELAY) | The delay caused by leveling. |
| [LEVELING_DELAY_FORMAT](#LEVELING-DELAY-FORMAT) | The duration format of a delay. |
| [LINKED_FIELDS](#LINKED-FIELDS) | Determines whether the Project is linked to another OLE object. |
| [MILESTONE](#MILESTONE) | Determines whether the assignment is a milestone. |
| [NOTES](#NOTES) | The text notes associated with an assignment. |
| [NOTES_RTF](#NOTES-RTF) | The text notes in RTF format. |
| [NOTES_TEXT](#NOTES-TEXT) | Notes' plain text extracted from RTF data. |
| [OVERALLOCATED](#OVERALLOCATED) | Determines whether the assignment is over-allocated. |
| [OVERTIME_COST](#OVERTIME-COST) | The sum of the actual and remaining overtime cost of an assignment. |
| [OVERTIME_WORK](#OVERTIME-WORK) | The scheduled overtime work of an assignment. |
| [PEAK_UNITS](#PEAK-UNITS) | The maximum number of units that a resource is assigned for a task. |
| [PERCENT_WORK_COMPLETE](#PERCENT-WORK-COMPLETE) | The amount of a work completed on an assignment. |
| [RATE_SCALE](#RATE-SCALE) | The time unit for the usage rate of the material resource assignment. |
| [REGULAR_WORK](#REGULAR-WORK) | The amount of a non-overtime work scheduled for an assignment. |
| [REMAINING_COST](#REMAINING-COST) | The remaining projected cost of completing an assignment. |
| [REMAINING_OVERTIME_COST](#REMAINING-OVERTIME-COST) | The remaining projected overtime cost of completing an assignment. |
| [REMAINING_OVERTIME_WORK](#REMAINING-OVERTIME-WORK) | The remaining overtime work scheduled to complete an assignment. |
| [REMAINING_WORK](#REMAINING-WORK) | The remaining work scheduled to complete an assignment. |
| [RESOURCE](#RESOURCE) | The resource assigned to a task. |
| [RESPONSE_PENDING](#RESPONSE-PENDING) | Determines whether the response has been received for a TeamAssign message. |
| [RESUME](#RESUME) | The date when assignment is resumed. |
| [START](#START) | The scheduled start date of an assignment. |
| [START_VARIANCE](#START-VARIANCE) | The variance of an assignment start date from a baseline start date. |
| [STOP](#STOP) | The date when assignment is stopped. |
| [SUMMARY](#SUMMARY) | Determines whether the task is a summary task. |
| [SV](#SV) | The earned value schedule variance, through the project status date. |
| [TASK](#TASK) | The task to which a resource is assigned. |
| [UID](#UID) | The unique identifier of an assignment. |
| [UNITS](#UNITS) | The number of units for an assignment. |
| [UPDATE_NEEDED](#UPDATE-NEEDED) | Determines whether the resource assigned to a task needs to be updated as to the status of the task. |
| [VAC](#VAC) | The difference between baseline cost and total cost. |
| [WORK](#WORK) | The amount of scheduled work for an assignment. |
| [WORK_CONTOUR](#WORK-CONTOUR) | The work contour of an assignment. |
| [WORK_VARIANCE](#WORK-VARIANCE) | The difference between baseline work of a task and the currently scheduled work. |
### ACTUAL_COST {#ACTUAL-COST}
```
public static final Key<BigDecimal,Integer> ACTUAL_COST
```


The actual cost incurred on an assignment.

### ACTUAL_FINISH {#ACTUAL-FINISH}
```
public static final Key<Date,Integer> ACTUAL_FINISH
```


The actual finish date of an assignment.

### ACTUAL_OVERTIME_COST {#ACTUAL-OVERTIME-COST}
```
public static final Key<BigDecimal,Integer> ACTUAL_OVERTIME_COST
```


The actual overtime cost incurred on an assignment.

### ACTUAL_OVERTIME_WORK {#ACTUAL-OVERTIME-WORK}
```
public static final Key<Duration,Integer> ACTUAL_OVERTIME_WORK
```


The actual amount of an overtime work incurred on an assignment.

### ACTUAL_OVERTIME_WORK_PROTECTED {#ACTUAL-OVERTIME-WORK-PROTECTED}
```
public static final Key<Duration,Integer> ACTUAL_OVERTIME_WORK_PROTECTED
```


The duration through which actual work is protected.

### ACTUAL_START {#ACTUAL-START}
```
public static final Key<Date,Integer> ACTUAL_START
```


The actual start date of an assignment.

### ACTUAL_WORK {#ACTUAL-WORK}
```
public static final Key<Duration,Integer> ACTUAL_WORK
```


The actual amount of a work incurred on an assignment.

### ACTUAL_WORK_PROTECTED {#ACTUAL-WORK-PROTECTED}
```
public static final Key<Duration,Integer> ACTUAL_WORK_PROTECTED
```


The duration through which actual overtime work is protected.

### ACWP {#ACWP}
```
public static final Key<Double,Integer> ACWP
```


The actual cost of a work performed on an assignment to-date.

### ASSIGNMENT_OWNER {#ASSIGNMENT-OWNER}
```
public static final Key<String,Integer> ASSIGNMENT_OWNER
```


The name of an assignment owner.

### ASSIGNMENT_OWNER_GUID {#ASSIGNMENT-OWNER-GUID}
```
public static final Key<String,Integer> ASSIGNMENT_OWNER_GUID
```


The globally unique identifier of an assignment owner.

### BCWP {#BCWP}
```
public static final Key<Double,Integer> BCWP
```


The budgeted cost of a work performed on assignment to-date.

### BCWS {#BCWS}
```
public static final Key<Double,Integer> BCWS
```


The budgeted cost of a work on assignment.

### BOOKING_TYPE {#BOOKING-TYPE}
```
public static final Key<Integer,Integer> BOOKING_TYPE
```


The booking type of an assignment.

### BUDGET_COST {#BUDGET-COST}
```
public static final Key<BigDecimal,Integer> BUDGET_COST
```


The budgeted cost of resources on an assignment.

### BUDGET_WORK {#BUDGET-WORK}
```
public static final Key<Duration,Integer> BUDGET_WORK
```


The budgeted work amount for a work or material resources on an assignment.

### CONFIRMED {#CONFIRMED}
```
public static final Key<Boolean,Integer> CONFIRMED
```


Determines whether a resource has accepted all of its assignments.

### COST {#COST}
```
public static final Key<BigDecimal,Integer> COST
```


The projected or scheduled cost of an assignment.

### COST_RATE_TABLE_TYPE {#COST-RATE-TABLE-TYPE}
```
public static final Key<Integer,Integer> COST_RATE_TABLE_TYPE
```


The cost rate table used for this assignment.

### COST_VARIANCE {#COST-VARIANCE}
```
public static final Key<Double,Integer> COST_VARIANCE
```


The difference between the baseline cost and total cost for an assignment.

### CREATED {#CREATED}
```
public static final Key<Date,Integer> CREATED
```


The date that the assignment was created.

### CV {#CV}
```
public static final Key<Double,Integer> CV
```


The earned value cost variance. CV is the difference between the assignment's BCWP (budgeted cost of work performed) and ACWP (actual cost of work performed).

### DELAY {#DELAY}
```
public static final Key<Duration,Integer> DELAY
```


The delay of an assignment.

### FINISH {#FINISH}
```
public static final Key<Date,Integer> FINISH
```


The scheduled finish date of an assignment.

### FINISH_VARIANCE {#FINISH-VARIANCE}
```
public static final Key<Duration,Integer> FINISH_VARIANCE
```


The variance of an assignment finish date from a baseline finish date.

### FIXED_MATERIAL {#FIXED-MATERIAL}
```
public static final Key<Boolean,Integer> FIXED_MATERIAL
```


Determines whether the consumption of an assigned material resource occurs in a single, fixed amount.

### HAS_FIXED_RATE_UNITS {#HAS-FIXED-RATE-UNITS}
```
public static final Key<Boolean,Integer> HAS_FIXED_RATE_UNITS
```


Determines whether the Units have Fixed Rate.

### HYPERLINK {#HYPERLINK}
```
public static final Key<String,Integer> HYPERLINK
```


The title or explanatory text of a hyperlink associated with an assignment.

### HYPERLINK_ADDRESS {#HYPERLINK-ADDRESS}
```
public static final Key<String,Integer> HYPERLINK_ADDRESS
```


The address for a hyperlink associated with assignment.

--------------------

The full address (Hyperlink Href in Microsoft Project) of the hyperlink is a concatenation of HyperlinkAddress and HyperlinkSubAddress.

### HYPERLINK_SUB_ADDRESS {#HYPERLINK-SUB-ADDRESS}
```
public static final Key<String,Integer> HYPERLINK_SUB_ADDRESS
```


The specific location in a document in a hyperlink associated with an assignment.

--------------------

The full address (Hyperlink Href in Microsoft Project) of the hyperlink is a concatenation of HyperlinkAddress and HyperlinkSubAddress.

### LEVELING_DELAY {#LEVELING-DELAY}
```
public static final Key<Duration,Integer> LEVELING_DELAY
```


The delay caused by leveling.

### LEVELING_DELAY_FORMAT {#LEVELING-DELAY-FORMAT}
```
public static final Key<Integer,Integer> LEVELING_DELAY_FORMAT
```


The duration format of a delay.

### LINKED_FIELDS {#LINKED-FIELDS}
```
public static final Key<Boolean,Integer> LINKED_FIELDS
```


Determines whether the Project is linked to another OLE object.

### MILESTONE {#MILESTONE}
```
public static final Key<Boolean,Integer> MILESTONE
```


Determines whether the assignment is a milestone.

### NOTES {#NOTES}
```
public static final Key<String,Integer> NOTES
```


The text notes associated with an assignment.

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
public static final Key<Boolean,Integer> OVERALLOCATED
```


Determines whether the assignment is over-allocated.

### OVERTIME_COST {#OVERTIME-COST}
```
public static final Key<BigDecimal,Integer> OVERTIME_COST
```


The sum of the actual and remaining overtime cost of an assignment.

### OVERTIME_WORK {#OVERTIME-WORK}
```
public static final Key<Duration,Integer> OVERTIME_WORK
```


The scheduled overtime work of an assignment.

### PEAK_UNITS {#PEAK-UNITS}
```
public static final Key<Double,Integer> PEAK_UNITS
```


The maximum number of units that a resource is assigned for a task.

### PERCENT_WORK_COMPLETE {#PERCENT-WORK-COMPLETE}
```
public static final Key<Integer,Integer> PERCENT_WORK_COMPLETE
```


The amount of a work completed on an assignment.

### RATE_SCALE {#RATE-SCALE}
```
public static final Key<Integer,Integer> RATE_SCALE
```


The time unit for the usage rate of the material resource assignment. Returns 0 if not defined.

### REGULAR_WORK {#REGULAR-WORK}
```
public static final Key<Duration,Integer> REGULAR_WORK
```


The amount of a non-overtime work scheduled for an assignment.

### REMAINING_COST {#REMAINING-COST}
```
public static final Key<BigDecimal,Integer> REMAINING_COST
```


The remaining projected cost of completing an assignment.

### REMAINING_OVERTIME_COST {#REMAINING-OVERTIME-COST}
```
public static final Key<BigDecimal,Integer> REMAINING_OVERTIME_COST
```


The remaining projected overtime cost of completing an assignment.

### REMAINING_OVERTIME_WORK {#REMAINING-OVERTIME-WORK}
```
public static final Key<Duration,Integer> REMAINING_OVERTIME_WORK
```


The remaining overtime work scheduled to complete an assignment.

### REMAINING_WORK {#REMAINING-WORK}
```
public static final Key<Duration,Integer> REMAINING_WORK
```


The remaining work scheduled to complete an assignment.

### RESOURCE {#RESOURCE}
```
public static final Key<Resource,Integer> RESOURCE
```


The resource assigned to a task.

### RESPONSE_PENDING {#RESPONSE-PENDING}
```
public static final Key<Boolean,Integer> RESPONSE_PENDING
```


Determines whether the response has been received for a TeamAssign message.

### RESUME {#RESUME}
```
public static final Key<Date,Integer> RESUME
```


The date when assignment is resumed.

### START {#START}
```
public static final Key<Date,Integer> START
```


The scheduled start date of an assignment.

### START_VARIANCE {#START-VARIANCE}
```
public static final Key<Duration,Integer> START_VARIANCE
```


The variance of an assignment start date from a baseline start date.

### STOP {#STOP}
```
public static final Key<Date,Integer> STOP
```


The date when assignment is stopped.

### SUMMARY {#SUMMARY}
```
public static final Key<Boolean,Integer> SUMMARY
```


Determines whether the task is a summary task.

### SV {#SV}
```
public static final Key<Double,Integer> SV
```


The earned value schedule variance, through the project status date. Schedule variance (SV) is the difference between the BCWP and the BCWS.

### TASK {#TASK}
```
public static final Key<Task,Integer> TASK
```


The task to which a resource is assigned.

### UID {#UID}
```
public static final Key<Integer,Integer> UID
```


The unique identifier of an assignment.

### UNITS {#UNITS}
```
public static final Key<Double,Integer> UNITS
```


The number of units for an assignment.

### UPDATE_NEEDED {#UPDATE-NEEDED}
```
public static final Key<Boolean,Integer> UPDATE_NEEDED
```


Determines whether the resource assigned to a task needs to be updated as to the status of the task.

### VAC {#VAC}
```
public static final Key<Double,Integer> VAC
```


The difference between baseline cost and total cost.

### WORK {#WORK}
```
public static final Key<Duration,Integer> WORK
```


The amount of scheduled work for an assignment.

### WORK_CONTOUR {#WORK-CONTOUR}
```
public static final Key<Integer,Integer> WORK_CONTOUR
```


The work contour of an assignment.

### WORK_VARIANCE {#WORK-VARIANCE}
```
public static final Key<Duration,Integer> WORK_VARIANCE
```


The difference between baseline work of a task and the currently scheduled work.

