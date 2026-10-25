---
title: "Prj"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示对象的受支持属性。"
type: docs
weight: 216
url: /zh/java/com.aspose.tasks/prj/
---

**Inheritance:**
java.lang.Object
```
public class Prj
```

表示 [Project](../../com.aspose.tasks/project) 对象的受支持属性。
## 字段

| 字段 | 描述 |
| --- | --- |
| [ACTUALS_IN_SYNC](#ACTUALS-IN-SYNC) | 确定是否已将所有实际工作与项目同步。 |
| [ADMIN_PROJECT](#ADMIN-PROJECT) | 确定项目是否为管理项目。 |
| [ARE_EDITABLE_ACTUAL_COSTS](#ARE-EDITABLE-ACTUAL-COSTS) | 确定实际成本是否可编辑。 |
| [AUTHOR](#AUTHOR) | 项目的作者。 |
| [AUTOLINK](#AUTOLINK) | 确定插入或移动的任务是否自动链接。 |
| [AUTO_ADD_NEW_RESOURCES_AND_TASKS](#AUTO-ADD-NEW-RESOURCES-AND-TASKS) | 确定是否将新资源或任务自动添加到资源或任务池中。 |
| [AUTO_CALCULATE_ASSIGNMENT_COSTS](#AUTO-CALCULATE-ASSIGNMENT-COSTS) | 确定是否应使用任务的工作量和资源费率自动计算分配成本和剩余成本。 |
| [BASELINE_FOR_EARNED_VALUE](#BASELINE-FOR-EARNED-VALUE) | 用于计算差异值的特定基准线。 |
| [CALENDAR](#CALENDAR) | 项目日历。 |
| [CATEGORY](#CATEGORY) | 项目的类别。 |
| [COMMENTS](#COMMENTS) | 项目的注释。 |
| [COMPANY](#COMPANY) | 创建项目的公司。 |
| [CREATION_DATE](#CREATION-DATE) | 项目创建的日期和时间。 |
| [CRITICAL_SLACK_LIMIT](#CRITICAL-SLACK-LIMIT) | 如果总浮动小于或等于此天数，MS Project 将任务视为关键。 |
| [CURRENCY_CODE](#CURRENCY-CODE) | ISO 4217 中定义的三字母货币代码。 |
| [CURRENCY_DIGITS](#CURRENCY-DIGITS) | 小数点后位数。 |
| [CURRENCY_SYMBOL](#CURRENCY-SYMBOL) | 项目中使用的货币符号。 |
| [CURRENCY_SYMBOL_POSITION](#CURRENCY-SYMBOL-POSITION) | 货币符号的位置。 |
| [CURRENT_DATE](#CURRENT-DATE) | 系统日期。 |
| [CUSTOM_DATE_FORMAT](#CUSTOM-DATE-FORMAT) | 项目视图自定义日期格式。 |
| [DATE_FORMAT](#DATE-FORMAT) | 项目视图日期格式。 |
| [DAYS_PER_MONTH](#DAYS-PER-MONTH) | 每月的天数。 |
| [DEFAULT_FINISH_TIME](#DEFAULT-FINISH-TIME) | 新任务的默认完成时间。 |
| [DEFAULT_FIXED_COST_ACCRUAL](#DEFAULT-FIXED-COST-ACCRUAL) | 固定成本累计时的默认类型。 |
| [DEFAULT_OVERTIME_RATE](#DEFAULT-OVERTIME-RATE) | 新资源的默认加班费率。 |
| [DEFAULT_STANDARD_RATE](#DEFAULT-STANDARD-RATE) | 新资源的默认标准费率。 |
| [DEFAULT_START_TIME](#DEFAULT-START-TIME) | 新任务的默认开始时间。 |
| [DEFAULT_TASK_EV_METHOD](#DEFAULT-TASK-EV-METHOD) | 任务的默认挣值方法。 |
| [DEFAULT_TASK_TYPE](#DEFAULT-TASK-TYPE) | 新任务的默认类型。 |
| [DURATION_FORMAT](#DURATION-FORMAT) | 表示批量持续时间的格式。 |
| [EARNED_VALUE_METHOD](#EARNED-VALUE-METHOD) | 计算挣值的默认方法。 |
| [EXTENDED_CREATION_DATE](#EXTENDED-CREATION-DATE) | 用于计算和报告的日期。 |
| [FINISH_DATE](#FINISH-DATE) | 项目的完成日期。 |
| [FISCAL_YEAR_START](#FISCAL-YEAR-START) | 确定是否使用财政年度编号。 |
| [FY_START_DATE](#FY-START-DATE) | 财政年度开始的月份。 |
| [GUID](#GUID) | 项目的 GUID。 |
| [HONOR_CONSTRAINTS](#HONOR-CONSTRAINTS) | 确定任务是否遵守其约束日期。 |
| [HYPERLINK_BASE](#HYPERLINK-BASE) | 项目的超链接基址。 |
| [INSERTED_PROJECTS_LIKE_SUMMARY](#INSERTED-PROJECTS-LIKE-SUMMARY) | 确定子任务是否被计算为汇总任务。 |
| [KEEP_TASK_ON_NEAREST_WORKING_TIME_WHEN_MADE_AUTO_SCHEDULED](#KEEP-TASK-ON-NEAREST-WORKING-TIME-WHEN-MADE-AUTO-SCHEDULED) | 确定手动任务在设为自动调度时是否必须保留在最近的工作时间。 |
| [KEYWORDS](#KEYWORDS) | 项目的关键字。 |
| [LAST_AUTHOR](#LAST-AUTHOR) | 项目的最后作者。 |
| [LAST_PRINTED](#LAST-PRINTED) | 项目的最后打印时间。 |
| [LAST_SAVED](#LAST-SAVED) | 项目上次保存的日期。 |
| [MANAGER](#MANAGER) | 项目的经理。 |
| [MICROSOFT_PROJECT_SERVER_URL](#MICROSOFT-PROJECT-SERVER-URL) | 确定项目是由 Project Server 用户创建的，而不是 NT 用户。 |
| [MINUTES_PER_DAY](#MINUTES-PER-DAY) | 每天的分钟数。 |
| [MINUTES_PER_WEEK](#MINUTES-PER-WEEK) | 每周的分钟数。 |
| [MOVE_COMPLETED_ENDS_BACK](#MOVE-COMPLETED-ENDS-BACK) | 确定计划在状态日期之后开始但实际提前开始的任务已完成部分的结束时间是否应移回状态日期。 |
| [MOVE_COMPLETED_ENDS_FORWARD](#MOVE-COMPLETED-ENDS-FORWARD) | 确定计划在状态日期之前完成但实际稍后开始的任务已完成部分的结束时间是否应提前到状态日期。 |
| [MOVE_REMAINING_STARTS_BACK](#MOVE-REMAINING-STARTS-BACK) | 确定计划在状态日期之后开始但实际提前开始的任务剩余部分的开始时间是否应移回状态日期。 |
| [MOVE_REMAINING_STARTS_FORWARD](#MOVE-REMAINING-STARTS-FORWARD) | 确定计划稍后开始的任务剩余部分的开始时间是否应提前到状态日期。 |
| [MULTIPLE_CRITICAL_PATHS](#MULTIPLE-CRITICAL-PATHS) | 确定是否计算多条关键路径。 |
| [NAME](#NAME) | 项目的名称。 |
| [NEW_TASKS_ARE_MANUAL](#NEW-TASKS-ARE-MANUAL) | 确定新创建的任务是否为手动任务。 |
| [NEW_TASKS_EFFORT_DRIVEN](#NEW-TASKS-EFFORT-DRIVEN) | 确定新任务是否以工作量为驱动。 |
| [NEW_TASKS_ESTIMATED](#NEW-TASKS-ESTIMATED) | 确定是否默认显示估计工期。 |
| [NEW_TASK_START_DATE](#NEW-TASK-START-DATE) | 新任务的默认开始日期类型。 |
| [PROJECT_EXTERNALLY_EDITED](#PROJECT-EXTERNALLY-EDITED) | 确定项目是否被外部编辑。 |
| [REMOVE_FILE_PROPERTIES](#REMOVE-FILE-PROPERTIES) | 确定在保存时是否会删除所有文件属性。 |
| [REVISION](#REVISION) | 项目保存的次数。 |
| [SAVE_VERSION](#SAVE-VERSION) | 从中保存项目文件的 Microsoft Office Project 版本。 |
| [SCHEDULE_FROM_START](#SCHEDULE-FROM-START) | 确定是否从开始日期向前计算项目进度表。 |
| [SHOW_PROJECT_SUMMARY_TASK](#SHOW-PROJECT-SUMMARY-TASK) | 确定是否在甘特图视图顶部的单行中显示整个项目的摘要信息，并带有其自己的摘要任务栏。 |
| [SPLITS_IN_PROGRESS_TASKS](#SPLITS-IN-PROGRESS-TASKS) | 确定进行中的任务是否可以拆分。 |
| [SPREAD_ACTUAL_COST](#SPREAD-ACTUAL-COST) | 确定实际成本是否分摊到状态日期。 |
| [SPREAD_PERCENT_COMPLETE](#SPREAD-PERCENT-COMPLETE) | 确定完成百分比是否分摊到状态日期。 |
| [START_DATE](#START-DATE) | 项目的开始日期。 |
| [STATUS_DATE](#STATUS-DATE) | 用于显示进度或计算挣值总计的状态日期。 |
| [SUBJECT](#SUBJECT) | 项目的主题。 |
| [TASK_UPDATES_RESOURCE](#TASK-UPDATES-RESOURCE) | 确定对任务的更新是否会更新资源。 |
| [TEMPLATE](#TEMPLATE) | 项目的模板。 |
| [TIMESCALE_FINISH](#TIMESCALE-FINISH) | 视图中时间尺度结束的日期。 |
| [TIMESCALE_START](#TIMESCALE-START) | 视图中时间尺度开始的日期。 |
| [TITLE](#TITLE) | 项目的标题。 |
| [UID](#UID) | 项目的唯一标识符。 |
| [UPDATE_MANUALLY_SCHEDULED_TASKS_WHEN_EDITING_LINKS](#UPDATE-MANUALLY-SCHEDULED-TASKS-WHEN-EDITING-LINKS) | 确定在链接被编辑时是否必须更新手动任务。 |
| [WEEK_START_DAY](#WEEK-START-DAY) | 一周的第一天。 |
| [WORK_FORMAT](#WORK-FORMAT) | 用于显示任务持续时间的格式。 |
### ACTUALS_IN_SYNC {#ACTUALS-IN-SYNC}
```
public static final Key<NullableBool,Byte> ACTUALS_IN_SYNC
```


确定是否已将所有实际工作与项目同步。

### ADMIN_PROJECT {#ADMIN-PROJECT}
```
public static final Key<NullableBool,Byte> ADMIN_PROJECT
```


确定项目是否为管理项目。

### ARE_EDITABLE_ACTUAL_COSTS {#ARE-EDITABLE-ACTUAL-COSTS}
```
public static final Key<NullableBool,Byte> ARE_EDITABLE_ACTUAL_COSTS
```


确定实际成本是否可编辑。

### AUTHOR {#AUTHOR}
```
public static final Key<String,Byte> AUTHOR
```


项目的作者。

### AUTOLINK {#AUTOLINK}
```
public static final Key<NullableBool,Byte> AUTOLINK
```


确定插入或移动的任务是否自动链接。

### AUTO_ADD_NEW_RESOURCES_AND_TASKS {#AUTO-ADD-NEW-RESOURCES-AND-TASKS}
```
public static final Key<NullableBool,Byte> AUTO_ADD_NEW_RESOURCES_AND_TASKS
```


确定是否将新资源或任务自动添加到资源或任务池中。

### AUTO_CALCULATE_ASSIGNMENT_COSTS {#AUTO-CALCULATE-ASSIGNMENT-COSTS}
```
public static final Key<Boolean,Byte> AUTO_CALCULATE_ASSIGNMENT_COSTS
```


确定是否应使用任务的工作量和资源费率自动计算分配成本和剩余成本。

### BASELINE_FOR_EARNED_VALUE {#BASELINE-FOR-EARNED-VALUE}
```
public static final Key<Integer,Byte> BASELINE_FOR_EARNED_VALUE
```


用于计算差异值的特定基准线。

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Byte> CALENDAR
```


项目日历。

### CATEGORY {#CATEGORY}
```
public static final Key<String,Byte> CATEGORY
```


项目的类别。

### COMMENTS {#COMMENTS}
```
public static final Key<String,Byte> COMMENTS
```


项目的注释。

### COMPANY {#COMPANY}
```
public static final Key<String,Byte> COMPANY
```


创建项目的公司。

### CREATION_DATE {#CREATION-DATE}
```
public static final Key<Date,Byte> CREATION_DATE
```


项目创建的日期和时间。

--------------------

以 UTC 格式保存在 mpp 文件中。java.util.Date 类型。

### CRITICAL_SLACK_LIMIT {#CRITICAL-SLACK-LIMIT}
```
public static final Key<Integer,Byte> CRITICAL_SLACK_LIMIT
```


如果总浮动小于或等于此天数，MS Project 将任务视为关键。

### CURRENCY_CODE {#CURRENCY-CODE}
```
public static final Key<String,Byte> CURRENCY_CODE
```


ISO 4217 定义的三字母货币代码。例如有效值为 "USD"。

### CURRENCY_DIGITS {#CURRENCY-DIGITS}
```
public static final Key<Integer,Byte> CURRENCY_DIGITS
```


小数点后位数。

### CURRENCY_SYMBOL {#CURRENCY-SYMBOL}
```
public static final Key<String,Byte> CURRENCY_SYMBOL
```


项目中使用的货币符号。

### CURRENCY_SYMBOL_POSITION {#CURRENCY-SYMBOL-POSITION}
```
public static final Key<Integer,Byte> CURRENCY_SYMBOL_POSITION
```


货币符号的位置。

### CURRENT_DATE {#CURRENT-DATE}
```
public static final Key<Date,Byte> CURRENT_DATE
```


系统日期。

### CUSTOM_DATE_FORMAT {#CUSTOM-DATE-FORMAT}
```
public static final Key<String,Byte> CUSTOM_DATE_FORMAT
```


项目视图自定义日期格式。当 [DATE\_FORMAT](../../com.aspose.tasks/prj\#DATE-FORMAT) 属性设置为 [DateFormat.Custom](../../com.aspose.tasks/dateformat\#Custom) 时用于格式化日期。

### DATE_FORMAT {#DATE-FORMAT}
```
public static final Key<Integer,Byte> DATE_FORMAT
```


项目视图日期格式。

### DAYS_PER_MONTH {#DAYS-PER-MONTH}
```
public static final Key<Integer,Byte> DAYS_PER_MONTH
```


每月的天数。

### DEFAULT_FINISH_TIME {#DEFAULT-FINISH-TIME}
```
public static final Key<Date,Byte> DEFAULT_FINISH_TIME
```


新任务的默认完成时间。

### DEFAULT_FIXED_COST_ACCRUAL {#DEFAULT-FIXED-COST-ACCRUAL}
```
public static final Key<Integer,Byte> DEFAULT_FIXED_COST_ACCRUAL
```


固定成本累计时的默认类型。

### DEFAULT_OVERTIME_RATE {#DEFAULT-OVERTIME-RATE}
```
public static final Key<Double,Byte> DEFAULT_OVERTIME_RATE
```


新资源的默认加班费率。

### DEFAULT_STANDARD_RATE {#DEFAULT-STANDARD-RATE}
```
public static final Key<Double,Byte> DEFAULT_STANDARD_RATE
```


新资源的默认标准费率。

### DEFAULT_START_TIME {#DEFAULT-START-TIME}
```
public static final Key<Date,Byte> DEFAULT_START_TIME
```


新任务的默认开始时间。

### DEFAULT_TASK_EV_METHOD {#DEFAULT-TASK-EV-METHOD}
```
public static final Key<Integer,Byte> DEFAULT_TASK_EV_METHOD
```


任务的默认挣值方法。

### DEFAULT_TASK_TYPE {#DEFAULT-TASK-TYPE}
```
public static final Key<Integer,Byte> DEFAULT_TASK_TYPE
```


新任务的默认类型。

### DURATION_FORMAT {#DURATION-FORMAT}
```
public static final Key<Byte,Byte> DURATION_FORMAT
```


用于表示整体持续时间的格式。`TimeUnitType` 类型。

### EARNED_VALUE_METHOD {#EARNED-VALUE-METHOD}
```
public static final Key<Integer,Byte> EARNED_VALUE_METHOD
```


计算挣值的默认方法。

### EXTENDED_CREATION_DATE {#EXTENDED-CREATION-DATE}
```
public static final Key<Date,Byte> EXTENDED_CREATION_DATE
```


用于计算和报告的日期。

### FINISH_DATE {#FINISH-DATE}
```
public static final Key<Date,Byte> FINISH_DATE
```


项目的完成日期。

### FISCAL_YEAR_START {#FISCAL-YEAR-START}
```
public static final Key<NullableBool,Byte> FISCAL_YEAR_START
```


确定是否使用财政年度编号。

### FY_START_DATE {#FY-START-DATE}
```
public static final Key<Integer,Byte> FY_START_DATE
```


财政年度开始的月份。

### GUID {#GUID}
```
public static final Key<UUID,Byte> GUID
```


项目的 GUID。

### HONOR_CONSTRAINTS {#HONOR-CONSTRAINTS}
```
public static final Key<NullableBool,Byte> HONOR_CONSTRAINTS
```


确定任务是否遵守其约束日期。

### HYPERLINK_BASE {#HYPERLINK-BASE}
```
public static final Key<String,Byte> HYPERLINK_BASE
```


项目的超链接基址。

### INSERTED_PROJECTS_LIKE_SUMMARY {#INSERTED-PROJECTS-LIKE-SUMMARY}
```
public static final Key<NullableBool,Byte> INSERTED_PROJECTS_LIKE_SUMMARY
```


确定子任务是否被计算为汇总任务。

### KEEP_TASK_ON_NEAREST_WORKING_TIME_WHEN_MADE_AUTO_SCHEDULED {#KEEP-TASK-ON-NEAREST-WORKING-TIME-WHEN-MADE-AUTO-SCHEDULED}
```
public static final Key<NullableBool,Byte> KEEP_TASK_ON_NEAREST_WORKING_TIME_WHEN_MADE_AUTO_SCHEDULED
```


确定手动任务在设为自动调度时是否必须保留在最近的工作时间。

### KEYWORDS {#KEYWORDS}
```
public static final Key<String,Byte> KEYWORDS
```


项目的关键字。

### LAST_AUTHOR {#LAST-AUTHOR}
```
public static final Key<String,Byte> LAST_AUTHOR
```


项目的最后作者。

### LAST_PRINTED {#LAST-PRINTED}
```
public static final Key<Date,Byte> LAST_PRINTED
```


项目的最后打印时间。

--------------------

以 UTC 格式保存在 mpp 文件中。java.util.Date 类型。

### LAST_SAVED {#LAST-SAVED}
```
public static final Key<Date,Byte> LAST_SAVED
```


项目上次保存的日期。

--------------------

以 UTC 格式保存在 mpp 文件中。java.util.Date 类型。

### MANAGER {#MANAGER}
```
public static final Key<String,Byte> MANAGER
```


项目的经理。

### MICROSOFT_PROJECT_SERVER_URL {#MICROSOFT-PROJECT-SERVER-URL}
```
public static final Key<NullableBool,Byte> MICROSOFT_PROJECT_SERVER_URL
```


确定项目是由 Project Server 用户创建的，而不是 NT 用户。

### MINUTES_PER_DAY {#MINUTES-PER-DAY}
```
public static final Key<Integer,Byte> MINUTES_PER_DAY
```


每天的分钟数。

### MINUTES_PER_WEEK {#MINUTES-PER-WEEK}
```
public static final Key<Integer,Byte> MINUTES_PER_WEEK
```


每周的分钟数。

### MOVE_COMPLETED_ENDS_BACK {#MOVE-COMPLETED-ENDS-BACK}
```
public static final Key<NullableBool,Byte> MOVE_COMPLETED_ENDS_BACK
```


确定计划在状态日期之后开始但实际提前开始的任务已完成部分的结束时间是否应移回状态日期。

### MOVE_COMPLETED_ENDS_FORWARD {#MOVE-COMPLETED-ENDS-FORWARD}
```
public static final Key<NullableBool,Byte> MOVE_COMPLETED_ENDS_FORWARD
```


确定计划在状态日期之前完成但实际稍后开始的任务已完成部分的结束时间是否应提前到状态日期。

### MOVE_REMAINING_STARTS_BACK {#MOVE-REMAINING-STARTS-BACK}
```
public static final Key<NullableBool,Byte> MOVE_REMAINING_STARTS_BACK
```


确定计划在状态日期之后开始但实际提前开始的任务剩余部分的开始时间是否应移回状态日期。

### MOVE_REMAINING_STARTS_FORWARD {#MOVE-REMAINING-STARTS-FORWARD}
```
public static final Key<NullableBool,Byte> MOVE_REMAINING_STARTS_FORWARD
```


确定计划稍后开始的任务剩余部分的开始时间是否应提前到状态日期。

### MULTIPLE_CRITICAL_PATHS {#MULTIPLE-CRITICAL-PATHS}
```
public static final Key<NullableBool,Byte> MULTIPLE_CRITICAL_PATHS
```


确定是否计算多条关键路径。

### NAME {#NAME}
```
public static final Key<String,Byte> NAME
```


项目的名称。

### NEW_TASKS_ARE_MANUAL {#NEW-TASKS-ARE-MANUAL}
```
public static final Key<NullableBool,Byte> NEW_TASKS_ARE_MANUAL
```


确定新创建的任务是否为手动任务。

### NEW_TASKS_EFFORT_DRIVEN {#NEW-TASKS-EFFORT-DRIVEN}
```
public static final Key<NullableBool,Byte> NEW_TASKS_EFFORT_DRIVEN
```


确定新任务是否以工作量为驱动。

### NEW_TASKS_ESTIMATED {#NEW-TASKS-ESTIMATED}
```
public static final Key<NullableBool,Byte> NEW_TASKS_ESTIMATED
```


确定是否默认显示估计工期。

### NEW_TASK_START_DATE {#NEW-TASK-START-DATE}
```
public static final Key<Integer,Byte> NEW_TASK_START_DATE
```


新任务的默认开始日期类型。

### PROJECT_EXTERNALLY_EDITED {#PROJECT-EXTERNALLY-EDITED}
```
public static final Key<NullableBool,Byte> PROJECT_EXTERNALLY_EDITED
```


确定项目是否被外部编辑。

### REMOVE_FILE_PROPERTIES {#REMOVE-FILE-PROPERTIES}
```
public static final Key<NullableBool,Byte> REMOVE_FILE_PROPERTIES
```


确定在保存时是否会删除所有文件属性。

### REVISION {#REVISION}
```
public static final Key<Integer,Byte> REVISION
```


项目保存的次数。

### SAVE_VERSION {#SAVE-VERSION}
```
public static final Key<Integer,Byte> SAVE_VERSION
```


从中保存项目文件的 Microsoft Office Project 版本。

### SCHEDULE_FROM_START {#SCHEDULE-FROM-START}
```
public static final Key<NullableBool,Byte> SCHEDULE_FROM_START
```


确定是否从开始日期向前计算项目进度表。

### SHOW_PROJECT_SUMMARY_TASK {#SHOW-PROJECT-SUMMARY-TASK}
```
public static final Key<Boolean,Byte> SHOW_PROJECT_SUMMARY_TASK
```


确定是否在甘特图视图顶部的单行中显示整个项目的摘要信息，并带有其自己的摘要任务栏。

### SPLITS_IN_PROGRESS_TASKS {#SPLITS-IN-PROGRESS-TASKS}
```
public static final Key<NullableBool,Byte> SPLITS_IN_PROGRESS_TASKS
```


确定进行中的任务是否可以拆分。

### SPREAD_ACTUAL_COST {#SPREAD-ACTUAL-COST}
```
public static final Key<NullableBool,Byte> SPREAD_ACTUAL_COST
```


确定实际成本是否分摊到状态日期。

### SPREAD_PERCENT_COMPLETE {#SPREAD-PERCENT-COMPLETE}
```
public static final Key<NullableBool,Byte> SPREAD_PERCENT_COMPLETE
```


确定完成百分比是否分摊到状态日期。

### START_DATE {#START-DATE}
```
public static final Key<Date,Byte> START_DATE
```


项目的开始日期。

### STATUS_DATE {#STATUS-DATE}
```
public static final Key<Date,Byte> STATUS_DATE
```


用于显示进度或计算挣值总计的状态日期。除非指定了不同的状态日期，否则状态日期与当前日期（今天的日期）相同。

### SUBJECT {#SUBJECT}
```
public static final Key<String,Byte> SUBJECT
```


项目的主题。

### TASK_UPDATES_RESOURCE {#TASK-UPDATES-RESOURCE}
```
public static final Key<NullableBool,Byte> TASK_UPDATES_RESOURCE
```


确定对任务的更新是否会更新资源。

### TEMPLATE {#TEMPLATE}
```
public static final Key<String,Byte> TEMPLATE
```


项目的模板。

### TIMESCALE_FINISH {#TIMESCALE-FINISH}
```
public static final Key<Date,Byte> TIMESCALE_FINISH
```


视图中时间尺度结束的日期。

### TIMESCALE_START {#TIMESCALE-START}
```
public static final Key<Date,Byte> TIMESCALE_START
```


视图中时间尺度开始的日期。

### TITLE {#TITLE}
```
public static final Key<String,Byte> TITLE
```


项目的标题。

### UID {#UID}
```
public static final Key<String,Byte> UID
```


项目的唯一标识符。

### UPDATE_MANUALLY_SCHEDULED_TASKS_WHEN_EDITING_LINKS {#UPDATE-MANUALLY-SCHEDULED-TASKS-WHEN-EDITING-LINKS}
```
public static final Key<NullableBool,Byte> UPDATE_MANUALLY_SCHEDULED_TASKS_WHEN_EDITING_LINKS
```


确定在链接被编辑时是否必须更新手动任务。

### WEEK_START_DAY {#WEEK-START-DAY}
```
public static final Key<Integer,Byte> WEEK_START_DAY
```


一周的第一天。

### WORK_FORMAT {#WORK-FORMAT}
```
public static final Key<Byte,Byte> WORK_FORMAT
```


用于显示任务持续时间的格式。

