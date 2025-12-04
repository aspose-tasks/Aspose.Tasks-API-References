---
title: Prj
second_title: Aspose.Tasks for Java API Reference
description: Represents supported properties of  object.
type: docs
weight: 215
url: /java/com.aspose.tasks/prj/
---

**Inheritance:**
java.lang.Object
```
public class Prj
```

Represents supported properties of [Project](../../com.aspose.tasks/project) object.
## Fields

| Field | Description |
| --- | --- |
| [ACTUALS_IN_SYNC](#ACTUALS-IN-SYNC) | Determines whether all actual works have been synchronized with the project. |
| [ADMIN_PROJECT](#ADMIN-PROJECT) | Determines whether a project is an administrative project. |
| [ARE_EDITABLE_ACTUAL_COSTS](#ARE-EDITABLE-ACTUAL-COSTS) | Determines whether actual costs are editable. |
| [AUTHOR](#AUTHOR) | The author of a project. |
| [AUTOLINK](#AUTOLINK) | Determines whether inserted or moved tasks are auto linked. |
| [AUTO_ADD_NEW_RESOURCES_AND_TASKS](#AUTO-ADD-NEW-RESOURCES-AND-TASKS) | Determines whether new resources or tasks automatically added to a resource or task pool. |
| [AUTO_CALCULATE_ASSIGNMENT_COSTS](#AUTO-CALCULATE-ASSIGNMENT-COSTS) | Determines whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates. |
| [BASELINE_FOR_EARNED_VALUE](#BASELINE-FOR-EARNED-VALUE) | The specific baseline used to calculate Variance values. |
| [CALENDAR](#CALENDAR) | The project calendar. |
| [CATEGORY](#CATEGORY) | The category of a project. |
| [COMMENTS](#COMMENTS) | Project's comments. |
| [COMPANY](#COMPANY) | The company where a project was created. |
| [CREATION_DATE](#CREATION-DATE) | The date and time when a project was created. |
| [CRITICAL_SLACK_LIMIT](#CRITICAL-SLACK-LIMIT) | Tasks are considered critical by MS Project if total slack is less or equal to this number of days. |
| [CURRENCY_CODE](#CURRENCY-CODE) | The three letter currency character code as defined in ISO 4217. |
| [CURRENCY_DIGITS](#CURRENCY-DIGITS) | The number of digits after a decimal symbol. |
| [CURRENCY_SYMBOL](#CURRENCY-SYMBOL) | The currency symbol used in a project. |
| [CURRENCY_SYMBOL_POSITION](#CURRENCY-SYMBOL-POSITION) | The placement of the currency symbol. |
| [CURRENT_DATE](#CURRENT-DATE) | The system date. |
| [CUSTOM_DATE_FORMAT](#CUSTOM-DATE-FORMAT) | Project view custom date format. |
| [DATE_FORMAT](#DATE-FORMAT) | Project view date format. |
| [DAYS_PER_MONTH](#DAYS-PER-MONTH) | The number of days per month. |
| [DEFAULT_FINISH_TIME](#DEFAULT-FINISH-TIME) | The default finish time of new tasks. |
| [DEFAULT_FIXED_COST_ACCRUAL](#DEFAULT-FIXED-COST-ACCRUAL) | The default type when fixed costs are accrued. |
| [DEFAULT_OVERTIME_RATE](#DEFAULT-OVERTIME-RATE) | The default overtime rate for new resources. |
| [DEFAULT_STANDARD_RATE](#DEFAULT-STANDARD-RATE) | The default standard rate for new resources. |
| [DEFAULT_START_TIME](#DEFAULT-START-TIME) | The default start time of new tasks. |
| [DEFAULT_TASK_EV_METHOD](#DEFAULT-TASK-EV-METHOD) | The default earned value method for tasks. |
| [DEFAULT_TASK_TYPE](#DEFAULT-TASK-TYPE) | The default type of new tasks. |
| [DURATION_FORMAT](#DURATION-FORMAT) | The format for expressing the bulk duration. |
| [EARNED_VALUE_METHOD](#EARNED-VALUE-METHOD) | The default method for calculating earned value. |
| [EXTENDED_CREATION_DATE](#EXTENDED-CREATION-DATE) | Date used for calculation and reporting. |
| [FINISH_DATE](#FINISH-DATE) | The finish date of a project. |
| [FISCAL_YEAR_START](#FISCAL-YEAR-START) | Determines whether the fiscal year numbering is used. |
| [FY_START_DATE](#FY-START-DATE) | The month when fiscal year is starting. |
| [GUID](#GUID) | The GUID of the project. |
| [HONOR_CONSTRAINTS](#HONOR-CONSTRAINTS) | Determines whether tasks honor their constraint dates. |
| [HYPERLINK_BASE](#HYPERLINK-BASE) | Project's hyperlink base. |
| [INSERTED_PROJECTS_LIKE_SUMMARY](#INSERTED-PROJECTS-LIKE-SUMMARY) | Determines whether subtasks are calculated as summary tasks. |
| [KEEP_TASK_ON_NEAREST_WORKING_TIME_WHEN_MADE_AUTO_SCHEDULED](#KEEP-TASK-ON-NEAREST-WORKING-TIME-WHEN-MADE-AUTO-SCHEDULED) | Determines whether manual tasks must be kept on nearest working time when made as auto scheduled. |
| [KEYWORDS](#KEYWORDS) | Project's keywords. |
| [LAST_AUTHOR](#LAST-AUTHOR) | Project's last author. |
| [LAST_PRINTED](#LAST-PRINTED) | Project's last print time. |
| [LAST_SAVED](#LAST-SAVED) | The date when a project was saved last time. |
| [MANAGER](#MANAGER) | The manager of a project. |
| [MICROSOFT_PROJECT_SERVER_URL](#MICROSOFT-PROJECT-SERVER-URL) | Determines whether a project was created by a Project Server user as opposed to an NT user. |
| [MINUTES_PER_DAY](#MINUTES-PER-DAY) | The number of minutes per day. |
| [MINUTES_PER_WEEK](#MINUTES-PER-WEEK) | The number of minutes per week. |
| [MOVE_COMPLETED_ENDS_BACK](#MOVE-COMPLETED-ENDS-BACK) | Determines whether the end of completed portions of tasks scheduled to start after the status date but started earlier should be moved back to the status date. |
| [MOVE_COMPLETED_ENDS_FORWARD](#MOVE-COMPLETED-ENDS-FORWARD) | Determines whether the end of completed portions of tasks scheduled to have been completed before the status date but begun later should be moved up to the status date. |
| [MOVE_REMAINING_STARTS_BACK](#MOVE-REMAINING-STARTS-BACK) | Determines whether the beginning of remaining portions of tasks scheduled to start after the status date but started earlier should be moved back to the status date. |
| [MOVE_REMAINING_STARTS_FORWARD](#MOVE-REMAINING-STARTS-FORWARD) | Determines whether the beginning of remaining portions of tasks scheduled to have begun later should be moved up to the status date. |
| [MULTIPLE_CRITICAL_PATHS](#MULTIPLE-CRITICAL-PATHS) | Determines whether multiple critical paths are calculated. |
| [NAME](#NAME) | The name of the project. |
| [NEW_TASKS_ARE_MANUAL](#NEW-TASKS-ARE-MANUAL) | Determines whether new tasks created as manual. |
| [NEW_TASKS_EFFORT_DRIVEN](#NEW-TASKS-EFFORT-DRIVEN) | Determines whether new tasks are effort driven. |
| [NEW_TASKS_ESTIMATED](#NEW-TASKS-ESTIMATED) | Determines whether an estimated duration is shown by default. |
| [NEW_TASK_START_DATE](#NEW-TASK-START-DATE) | The default start date type for new tasks. |
| [PROJECT_EXTERNALLY_EDITED](#PROJECT-EXTERNALLY-EDITED) | Determines whether the project was externally edited. |
| [REMOVE_FILE_PROPERTIES](#REMOVE-FILE-PROPERTIES) | Determines whether all file properties will be removed on save. |
| [REVISION](#REVISION) | The number of times a project was saved. |
| [SAVE_VERSION](#SAVE-VERSION) | The version of Microsoft Office Project from which a project file was saved. |
| [SCHEDULE_FROM_START](#SCHEDULE-FROM-START) | Determines whether to calculate the project schedule forward from the start date. |
| [SHOW_PROJECT_SUMMARY_TASK](#SHOW-PROJECT-SUMMARY-TASK) | Determines whether to display summary information about an entire project on a single row with its own summary task bar at the top of the Gantt Chart view. |
| [SPLITS_IN_PROGRESS_TASKS](#SPLITS-IN-PROGRESS-TASKS) | Determines whether in-progress tasks can be split. |
| [SPREAD_ACTUAL_COST](#SPREAD-ACTUAL-COST) | Determines whether actual costs are spread to the status date. |
| [SPREAD_PERCENT_COMPLETE](#SPREAD-PERCENT-COMPLETE) | Determines whether a percent complete is spread to the status date. |
| [START_DATE](#START-DATE) | The start date of a project. |
| [STATUS_DATE](#STATUS-DATE) | the status date to display progress or to calculate earned value totals. |
| [SUBJECT](#SUBJECT) | The subject of a project. |
| [TASK_UPDATES_RESOURCE](#TASK-UPDATES-RESOURCE) | Determines whether updates to tasks update resources. |
| [TEMPLATE](#TEMPLATE) | Project's template. |
| [TIMESCALE_FINISH](#TIMESCALE-FINISH) | The date that the timescale in the view finishes. |
| [TIMESCALE_START](#TIMESCALE-START) | The date that the timescale in the view starts. |
| [TITLE](#TITLE) | The title of a project. |
| [UID](#UID) | The unique Id of a project. |
| [UPDATE_MANUALLY_SCHEDULED_TASKS_WHEN_EDITING_LINKS](#UPDATE-MANUALLY-SCHEDULED-TASKS-WHEN-EDITING-LINKS) | Determines whether manual tasks must be updated when links were edited. |
| [WEEK_START_DAY](#WEEK-START-DAY) | First day of a week. |
| [WORK_FORMAT](#WORK-FORMAT) | The format used to show the duration of the task. |
### ACTUALS_IN_SYNC {#ACTUALS-IN-SYNC}
```
public static final Key<NullableBool,Byte> ACTUALS_IN_SYNC
```


Determines whether all actual works have been synchronized with the project.

### ADMIN_PROJECT {#ADMIN-PROJECT}
```
public static final Key<NullableBool,Byte> ADMIN_PROJECT
```


Determines whether a project is an administrative project.

### ARE_EDITABLE_ACTUAL_COSTS {#ARE-EDITABLE-ACTUAL-COSTS}
```
public static final Key<NullableBool,Byte> ARE_EDITABLE_ACTUAL_COSTS
```


Determines whether actual costs are editable.

### AUTHOR {#AUTHOR}
```
public static final Key<String,Byte> AUTHOR
```


The author of a project.

### AUTOLINK {#AUTOLINK}
```
public static final Key<NullableBool,Byte> AUTOLINK
```


Determines whether inserted or moved tasks are auto linked.

### AUTO_ADD_NEW_RESOURCES_AND_TASKS {#AUTO-ADD-NEW-RESOURCES-AND-TASKS}
```
public static final Key<NullableBool,Byte> AUTO_ADD_NEW_RESOURCES_AND_TASKS
```


Determines whether new resources or tasks automatically added to a resource or task pool.

### AUTO_CALCULATE_ASSIGNMENT_COSTS {#AUTO-CALCULATE-ASSIGNMENT-COSTS}
```
public static final Key<Boolean,Byte> AUTO_CALCULATE_ASSIGNMENT_COSTS
```


Determines whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates.

### BASELINE_FOR_EARNED_VALUE {#BASELINE-FOR-EARNED-VALUE}
```
public static final Key<Integer,Byte> BASELINE_FOR_EARNED_VALUE
```


The specific baseline used to calculate Variance values.

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Byte> CALENDAR
```


The project calendar.

### CATEGORY {#CATEGORY}
```
public static final Key<String,Byte> CATEGORY
```


The category of a project.

### COMMENTS {#COMMENTS}
```
public static final Key<String,Byte> COMMENTS
```


Project's comments.

### COMPANY {#COMPANY}
```
public static final Key<String,Byte> COMPANY
```


The company where a project was created.

### CREATION_DATE {#CREATION-DATE}
```
public static final Key<Date,Byte> CREATION_DATE
```


The date and time when a project was created.

--------------------

Saved in UTC format in mpp files. java.util.Date type.

### CRITICAL_SLACK_LIMIT {#CRITICAL-SLACK-LIMIT}
```
public static final Key<Integer,Byte> CRITICAL_SLACK_LIMIT
```


Tasks are considered critical by MS Project if total slack is less or equal to this number of days.

### CURRENCY_CODE {#CURRENCY-CODE}
```
public static final Key<String,Byte> CURRENCY_CODE
```


The three letter currency character code as defined in ISO 4217. Example of valid values is "USD".

### CURRENCY_DIGITS {#CURRENCY-DIGITS}
```
public static final Key<Integer,Byte> CURRENCY_DIGITS
```


The number of digits after a decimal symbol.

### CURRENCY_SYMBOL {#CURRENCY-SYMBOL}
```
public static final Key<String,Byte> CURRENCY_SYMBOL
```


The currency symbol used in a project.

### CURRENCY_SYMBOL_POSITION {#CURRENCY-SYMBOL-POSITION}
```
public static final Key<Integer,Byte> CURRENCY_SYMBOL_POSITION
```


The placement of the currency symbol.

### CURRENT_DATE {#CURRENT-DATE}
```
public static final Key<Date,Byte> CURRENT_DATE
```


The system date.

### CUSTOM_DATE_FORMAT {#CUSTOM-DATE-FORMAT}
```
public static final Key<String,Byte> CUSTOM_DATE_FORMAT
```


Project view custom date format. Used to format dates when [DATE\_FORMAT](../../com.aspose.tasks/prj\#DATE-FORMAT) property is set to [DateFormat.Custom](../../com.aspose.tasks/dateformat\#Custom).

### DATE_FORMAT {#DATE-FORMAT}
```
public static final Key<Integer,Byte> DATE_FORMAT
```


Project view date format.

### DAYS_PER_MONTH {#DAYS-PER-MONTH}
```
public static final Key<Integer,Byte> DAYS_PER_MONTH
```


The number of days per month.

### DEFAULT_FINISH_TIME {#DEFAULT-FINISH-TIME}
```
public static final Key<Date,Byte> DEFAULT_FINISH_TIME
```


The default finish time of new tasks.

### DEFAULT_FIXED_COST_ACCRUAL {#DEFAULT-FIXED-COST-ACCRUAL}
```
public static final Key<Integer,Byte> DEFAULT_FIXED_COST_ACCRUAL
```


The default type when fixed costs are accrued.

### DEFAULT_OVERTIME_RATE {#DEFAULT-OVERTIME-RATE}
```
public static final Key<Double,Byte> DEFAULT_OVERTIME_RATE
```


The default overtime rate for new resources.

### DEFAULT_STANDARD_RATE {#DEFAULT-STANDARD-RATE}
```
public static final Key<Double,Byte> DEFAULT_STANDARD_RATE
```


The default standard rate for new resources.

### DEFAULT_START_TIME {#DEFAULT-START-TIME}
```
public static final Key<Date,Byte> DEFAULT_START_TIME
```


The default start time of new tasks.

### DEFAULT_TASK_EV_METHOD {#DEFAULT-TASK-EV-METHOD}
```
public static final Key<Integer,Byte> DEFAULT_TASK_EV_METHOD
```


The default earned value method for tasks.

### DEFAULT_TASK_TYPE {#DEFAULT-TASK-TYPE}
```
public static final Key<Integer,Byte> DEFAULT_TASK_TYPE
```


The default type of new tasks.

### DURATION_FORMAT {#DURATION-FORMAT}
```
public static final Key<Byte,Byte> DURATION_FORMAT
```


The format for expressing the bulk duration. `TimeUnitType` type.

### EARNED_VALUE_METHOD {#EARNED-VALUE-METHOD}
```
public static final Key<Integer,Byte> EARNED_VALUE_METHOD
```


The default method for calculating earned value.

### EXTENDED_CREATION_DATE {#EXTENDED-CREATION-DATE}
```
public static final Key<Date,Byte> EXTENDED_CREATION_DATE
```


Date used for calculation and reporting.

### FINISH_DATE {#FINISH-DATE}
```
public static final Key<Date,Byte> FINISH_DATE
```


The finish date of a project.

### FISCAL_YEAR_START {#FISCAL-YEAR-START}
```
public static final Key<NullableBool,Byte> FISCAL_YEAR_START
```


Determines whether the fiscal year numbering is used.

### FY_START_DATE {#FY-START-DATE}
```
public static final Key<Integer,Byte> FY_START_DATE
```


The month when fiscal year is starting.

### GUID {#GUID}
```
public static final Key<UUID,Byte> GUID
```


The GUID of the project.

### HONOR_CONSTRAINTS {#HONOR-CONSTRAINTS}
```
public static final Key<NullableBool,Byte> HONOR_CONSTRAINTS
```


Determines whether tasks honor their constraint dates.

### HYPERLINK_BASE {#HYPERLINK-BASE}
```
public static final Key<String,Byte> HYPERLINK_BASE
```


Project's hyperlink base.

### INSERTED_PROJECTS_LIKE_SUMMARY {#INSERTED-PROJECTS-LIKE-SUMMARY}
```
public static final Key<NullableBool,Byte> INSERTED_PROJECTS_LIKE_SUMMARY
```


Determines whether subtasks are calculated as summary tasks.

### KEEP_TASK_ON_NEAREST_WORKING_TIME_WHEN_MADE_AUTO_SCHEDULED {#KEEP-TASK-ON-NEAREST-WORKING-TIME-WHEN-MADE-AUTO-SCHEDULED}
```
public static final Key<NullableBool,Byte> KEEP_TASK_ON_NEAREST_WORKING_TIME_WHEN_MADE_AUTO_SCHEDULED
```


Determines whether manual tasks must be kept on nearest working time when made as auto scheduled.

### KEYWORDS {#KEYWORDS}
```
public static final Key<String,Byte> KEYWORDS
```


Project's keywords.

### LAST_AUTHOR {#LAST-AUTHOR}
```
public static final Key<String,Byte> LAST_AUTHOR
```


Project's last author.

### LAST_PRINTED {#LAST-PRINTED}
```
public static final Key<Date,Byte> LAST_PRINTED
```


Project's last print time.

--------------------

Saved in UTC format in mpp files. java.util.Date type.

### LAST_SAVED {#LAST-SAVED}
```
public static final Key<Date,Byte> LAST_SAVED
```


The date when a project was saved last time.

--------------------

Saved in UTC format in mpp files. java.util.Date type.

### MANAGER {#MANAGER}
```
public static final Key<String,Byte> MANAGER
```


The manager of a project.

### MICROSOFT_PROJECT_SERVER_URL {#MICROSOFT-PROJECT-SERVER-URL}
```
public static final Key<NullableBool,Byte> MICROSOFT_PROJECT_SERVER_URL
```


Determines whether a project was created by a Project Server user as opposed to an NT user.

### MINUTES_PER_DAY {#MINUTES-PER-DAY}
```
public static final Key<Integer,Byte> MINUTES_PER_DAY
```


The number of minutes per day.

### MINUTES_PER_WEEK {#MINUTES-PER-WEEK}
```
public static final Key<Integer,Byte> MINUTES_PER_WEEK
```


The number of minutes per week.

### MOVE_COMPLETED_ENDS_BACK {#MOVE-COMPLETED-ENDS-BACK}
```
public static final Key<NullableBool,Byte> MOVE_COMPLETED_ENDS_BACK
```


Determines whether the end of completed portions of tasks scheduled to start after the status date but started earlier should be moved back to the status date.

### MOVE_COMPLETED_ENDS_FORWARD {#MOVE-COMPLETED-ENDS-FORWARD}
```
public static final Key<NullableBool,Byte> MOVE_COMPLETED_ENDS_FORWARD
```


Determines whether the end of completed portions of tasks scheduled to have been completed before the status date but begun later should be moved up to the status date.

### MOVE_REMAINING_STARTS_BACK {#MOVE-REMAINING-STARTS-BACK}
```
public static final Key<NullableBool,Byte> MOVE_REMAINING_STARTS_BACK
```


Determines whether the beginning of remaining portions of tasks scheduled to start after the status date but started earlier should be moved back to the status date.

### MOVE_REMAINING_STARTS_FORWARD {#MOVE-REMAINING-STARTS-FORWARD}
```
public static final Key<NullableBool,Byte> MOVE_REMAINING_STARTS_FORWARD
```


Determines whether the beginning of remaining portions of tasks scheduled to have begun later should be moved up to the status date.

### MULTIPLE_CRITICAL_PATHS {#MULTIPLE-CRITICAL-PATHS}
```
public static final Key<NullableBool,Byte> MULTIPLE_CRITICAL_PATHS
```


Determines whether multiple critical paths are calculated.

### NAME {#NAME}
```
public static final Key<String,Byte> NAME
```


The name of the project.

### NEW_TASKS_ARE_MANUAL {#NEW-TASKS-ARE-MANUAL}
```
public static final Key<NullableBool,Byte> NEW_TASKS_ARE_MANUAL
```


Determines whether new tasks created as manual.

### NEW_TASKS_EFFORT_DRIVEN {#NEW-TASKS-EFFORT-DRIVEN}
```
public static final Key<NullableBool,Byte> NEW_TASKS_EFFORT_DRIVEN
```


Determines whether new tasks are effort driven.

### NEW_TASKS_ESTIMATED {#NEW-TASKS-ESTIMATED}
```
public static final Key<NullableBool,Byte> NEW_TASKS_ESTIMATED
```


Determines whether an estimated duration is shown by default.

### NEW_TASK_START_DATE {#NEW-TASK-START-DATE}
```
public static final Key<Integer,Byte> NEW_TASK_START_DATE
```


The default start date type for new tasks.

### PROJECT_EXTERNALLY_EDITED {#PROJECT-EXTERNALLY-EDITED}
```
public static final Key<NullableBool,Byte> PROJECT_EXTERNALLY_EDITED
```


Determines whether the project was externally edited.

### REMOVE_FILE_PROPERTIES {#REMOVE-FILE-PROPERTIES}
```
public static final Key<NullableBool,Byte> REMOVE_FILE_PROPERTIES
```


Determines whether all file properties will be removed on save.

### REVISION {#REVISION}
```
public static final Key<Integer,Byte> REVISION
```


The number of times a project was saved.

### SAVE_VERSION {#SAVE-VERSION}
```
public static final Key<Integer,Byte> SAVE_VERSION
```


The version of Microsoft Office Project from which a project file was saved.

### SCHEDULE_FROM_START {#SCHEDULE-FROM-START}
```
public static final Key<NullableBool,Byte> SCHEDULE_FROM_START
```


Determines whether to calculate the project schedule forward from the start date.

### SHOW_PROJECT_SUMMARY_TASK {#SHOW-PROJECT-SUMMARY-TASK}
```
public static final Key<Boolean,Byte> SHOW_PROJECT_SUMMARY_TASK
```


Determines whether to display summary information about an entire project on a single row with its own summary task bar at the top of the Gantt Chart view.

### SPLITS_IN_PROGRESS_TASKS {#SPLITS-IN-PROGRESS-TASKS}
```
public static final Key<NullableBool,Byte> SPLITS_IN_PROGRESS_TASKS
```


Determines whether in-progress tasks can be split.

### SPREAD_ACTUAL_COST {#SPREAD-ACTUAL-COST}
```
public static final Key<NullableBool,Byte> SPREAD_ACTUAL_COST
```


Determines whether actual costs are spread to the status date.

### SPREAD_PERCENT_COMPLETE {#SPREAD-PERCENT-COMPLETE}
```
public static final Key<NullableBool,Byte> SPREAD_PERCENT_COMPLETE
```


Determines whether a percent complete is spread to the status date.

### START_DATE {#START-DATE}
```
public static final Key<Date,Byte> START_DATE
```


The start date of a project.

### STATUS_DATE {#STATUS-DATE}
```
public static final Key<Date,Byte> STATUS_DATE
```


the status date to display progress or to calculate earned value totals. The status date is the same as the current date (today's date) unless a different status date is specified.

### SUBJECT {#SUBJECT}
```
public static final Key<String,Byte> SUBJECT
```


The subject of a project.

### TASK_UPDATES_RESOURCE {#TASK-UPDATES-RESOURCE}
```
public static final Key<NullableBool,Byte> TASK_UPDATES_RESOURCE
```


Determines whether updates to tasks update resources.

### TEMPLATE {#TEMPLATE}
```
public static final Key<String,Byte> TEMPLATE
```


Project's template.

### TIMESCALE_FINISH {#TIMESCALE-FINISH}
```
public static final Key<Date,Byte> TIMESCALE_FINISH
```


The date that the timescale in the view finishes.

### TIMESCALE_START {#TIMESCALE-START}
```
public static final Key<Date,Byte> TIMESCALE_START
```


The date that the timescale in the view starts.

### TITLE {#TITLE}
```
public static final Key<String,Byte> TITLE
```


The title of a project.

### UID {#UID}
```
public static final Key<String,Byte> UID
```


The unique Id of a project.

### UPDATE_MANUALLY_SCHEDULED_TASKS_WHEN_EDITING_LINKS {#UPDATE-MANUALLY-SCHEDULED-TASKS-WHEN-EDITING-LINKS}
```
public static final Key<NullableBool,Byte> UPDATE_MANUALLY_SCHEDULED_TASKS_WHEN_EDITING_LINKS
```


Determines whether manual tasks must be updated when links were edited.

### WEEK_START_DAY {#WEEK-START-DAY}
```
public static final Key<Integer,Byte> WEEK_START_DAY
```


First day of a week.

### WORK_FORMAT {#WORK-FORMAT}
```
public static final Key<Byte,Byte> WORK_FORMAT
```


The format used to show the duration of the task.

