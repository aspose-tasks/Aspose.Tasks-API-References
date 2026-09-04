---
title: "Tsk"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示对象的属性。"
type: docs
weight: 328
url: /zh/java/com.aspose.tasks/tsk/
---

**Inheritance:**
java.lang.Object
```
public class Tsk
```

表示 [Task](../../com.aspose.tasks/task) 对象的属性。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Tsk()](#Tsk--) |  |
## 字段

| 字段 | 描述 |
| --- | --- |
| [ACTIVITY_ID](#ACTIVITY-ID) | 表示活动 ID 字段——Primavera 使用的任务唯一标识符。 |
| [ACTUAL_COST](#ACTUAL-COST) | 已由资源在其任务上完成的工作产生的费用，以及与任务相关的任何其他记录费用。 |
| [ACTUAL_DURATION](#ACTUAL-DURATION) | 基于计划工期和当前剩余工作量或完成百分比的任务实际工作时间跨度。 |
| [ACTUAL_FINISH](#ACTUAL-FINISH) | 任务完成的日期。 |
| [ACTUAL_OVERTIME_COST](#ACTUAL-OVERTIME-COST) | 已由指派资源在任务上完成的加班工作产生的费用。 |
| [ACTUAL_OVERTIME_WORK](#ACTUAL-OVERTIME-WORK) | 已由分配到任务的资源完成的实际加班工作量。 |
| [ACTUAL_OVERTIME_WORK_PROTECTED](#ACTUAL-OVERTIME-WORK-PROTECTED) | 实际加班工作受保护的持续时间。 |
| [ACTUAL_START](#ACTUAL-START) | 任务实际开始的日期和时间。 |
| [ACTUAL_WORK](#ACTUAL-WORK) | 已由分配到任务的资源完成的工作量。 |
| [ACTUAL_WORK_PROTECTED](#ACTUAL-WORK-PROTECTED) | 实际工作受保护的持续时间。 |
| [ACWP](#ACWP) | 截至状态日期或今天的任务已完成工作产生的费用。 |
| [BCWP](#BCWP) | 任务完成百分比乘以时间分阶段基准成本的累计值。 |
| [BCWS](#BCWS) | 截至状态日期或今天的累计时间分阶段基准成本。 |
| [BUDGET_COST](#BUDGET-COST) | 预算成本资源的预算费用. |
| [BUDGET_WORK](#BUDGET-WORK) | 用于预算工作和材料资源的预算工作。 |
| [CALENDAR](#CALENDAR) | 任务日历。 |
| [COMMITMENT_FINISH](#COMMITMENT-FINISH) | 交付的完成日期。 |
| [COMMITMENT_START](#COMMITMENT-START) | 交付的开始日期。 |
| [COMMITMENT_TYPE](#COMMITMENT-TYPE) | 确定任务是否具有关联的交付或对关联交付的依赖。 |
| [CONSTRAINT_DATE](#CONSTRAINT-DATE) | 与约束类型关联的具体日期。 |
| [CONSTRAINT_TYPE](#CONSTRAINT-TYPE) | 提供可用于任务调度的约束类型选项。 |
| [CONTACT](#CONTACT) | 负责任务的个人姓名。 |
| [COST](#COST) | 任务的总计划或预测成本，基于已分配资源完成工作已产生的成本以及剩余工作计划的成本。 |
| [COST_VARIANCE](#COST-VARIANCE) | 任务、资源或分配的基准成本与总成本之间的差额。 |
| [CREATED](#CREATED) | 任务创建的日期。 |
| [CV](#CV) | 任务的基准成本与总成本之间的差额。 |
| [DEADLINE](#DEADLINE) | 指示任务完成时间的目标日期。 |
| [DISPLAY_AS_SUMMARY](#DISPLAY-AS-SUMMARY) | 确定任务是否应显示为汇总任务。 |
| [DISPLAY_ON_TIMELINE](#DISPLAY-ON-TIMELINE) | 指定任务是否应在时间轴视图中显示。 |
| [DURATION](#DURATION) | 任务的总活跃工作时间跨度，按输入或 Microsoft Project 根据开始日期、结束日期、日历和其他调度因素计算得出。 |
| [DURATION_TEXT](#DURATION-TEXT) | 返回任务的持续时间文本。 |
| [DURATION_VARIANCE](#DURATION-VARIANCE) | 任务的基准持续时间与总持续时间（当前估计）之间的差异。 |
| [EARLY_FINISH](#EARLY-FINISH) | 任务可能完成的最早日期，基于前置和后续任务的最早完成日期、其他约束以及任何平衡延迟。 |
| [EARLY_START](#EARLY-START) | 任务可能开始的最早日期，基于前置和后续任务的最早开始日期以及其他约束。 |
| [EARNED_VALUE_METHOD](#EARNED-VALUE-METHOD) | 确定应使用“% 完成”还是“物理 % 完成”字段来计算已完成工作预算成本（BCWP）。 |
| [EXTERNAL_ID](#EXTERNAL-ID) | 如果任务是外部任务，则包含该任务的外部 ID。 |
| [EXTERNAL_TASK_PROJECT](#EXTERNAL-TASK-PROJECT) | 外部任务的来源位置和任务标识符。 |
| [EXTERNAL_UID](#EXTERNAL-UID) | 当任务为外部任务时，包含外部任务的唯一标识符。 |
| [FINISH](#FINISH) | 任务的计划完成日期。 |
| [FINISH_SLACK_TIME_SPAN](#FINISH-SLACK-TIME-SPAN) | 最早完成日期和最迟完成日期之间的持续时间（秒）。 |
| [FINISH_TEXT](#FINISH-TEXT) | 返回任务的完成文本。 |
| [FINISH_VARIANCE](#FINISH-VARIANCE) | 表示任务或分配的基准完成日期与当前完成日期之间差异的时间。 |
| [FIXED_COST](#FIXED-COST) | 显示任何非资源任务费用。 |
| [FIXED_COST_ACCRUAL](#FIXED-COST-ACCRUAL) | 确定固定成本何时以及如何计入任务成本，或计提的选项。 |
| [FREE_SLACK_TIME_SPAN](#FREE-SLACK-TIME-SPAN) | 任务可以延迟的时间（秒），且不会导致任何后继任务延迟。 |
| [GUID](#GUID) | 为任务生成的唯一标识代码。 |
| [HAS_OVERALLOCATED_RESOURCE](#HAS-OVERALLOCATED-RESOURCE) | 指示任务是否分配了资源，该资源在已分配任务上的工作量超过正常工作容量。 |
| [HIDE_BAR](#HIDE-BAR) | 确定在 Microsoft Project 中显示时，任务的甘特条是否隐藏。 |
| [HYPERLINK](#HYPERLINK) | 与任务关联的超链接的标题或说明文字。 |
| [HYPERLINK_ADDRESS](#HYPERLINK-ADDRESS) | 与任务关联的超链接的地址。 |
| [HYPERLINK_SUB_ADDRESS](#HYPERLINK-SUB-ADDRESS) | 与任务关联的超链接中文档的具体位置. |
| [ID](#ID) | 任务在任务列表中的位置标识符。 |
| [IGNORE_RESOURCE_CALENDAR](#IGNORE-RESOURCE-CALENDAR) | 确定任务的调度是否考虑分配给该任务的资源日历。 |
| [IGNORE_WARNINGS](#IGNORE-WARNINGS) | 指示是否在 Microsoft Project 中隐藏调度冲突警告指示器。 |
| [IS_ACTIVE](#IS-ACTIVE) | 确定任务是否处于活动状态。 |
| [IS_CRITICAL](#IS-CRITICAL) | 确定任务是否位于关键路径上。 |
| [IS_EFFORT_DRIVEN](#IS-EFFORT-DRIVEN) | 确定任务的调度是否为基于工作量的调度。 |
| [IS_ESTIMATED](#IS-ESTIMATED) | 确定任务是否为估算任务。 |
| [IS_EXPANDED](#IS-EXPANDED) | 确定在甘特图视图中汇总任务是否展开。 |
| [IS_EXTERNAL_TASK](#IS-EXTERNAL-TASK) | 确定任务是否为外部任务。 |
| [IS_MANUAL](#IS-MANUAL) | 确定任务是否为手动调度。 |
| [IS_MARKED](#IS-MARKED) | 显示任务是否被标记为需要进一步操作或某种标识。 |
| [IS_MILESTONE](#IS-MILESTONE) | 确定任务是否为里程碑。 |
| [IS_NULL](#IS-NULL) | 确定任务是否为空任务。 |
| [IS_OVERALLOCATED](#IS-OVERALLOCATED) | 指示任务上分配的任何资源是否承担了超过正常工作容量的工作量。 |
| [IS_PUBLISHED](#IS-PUBLISHED) | 确定当前任务是否应与项目的其他部分一起发布到 Project Server。 |
| [IS_RECURRING](#IS-RECURRING) | 确定任务是否属于一系列循环任务。 |
| [IS_RESUME_VALID](#IS-RESUME-VALID) | 确定任务是否可以恢复。 |
| [IS_ROLLUP](#IS-ROLLUP) | 确定子任务甘特条的信息是否会汇总到汇总任务条中。 |
| [IS_SUBPROJECT](#IS-SUBPROJECT) | 确定任务是否为插入的项目。 |
| [IS_SUBPROJECT_READ_ONLY](#IS-SUBPROJECT-READ-ONLY) | 确定子项目是否为只读。 |
| [IS_SUMMARY](#IS-SUMMARY) | 确定任务是否为汇总任务。 |
| [LATE_FINISH](#LATE-FINISH) | 任务可以完成而不延迟项目完成的最迟日期。 |
| [LATE_START](#LATE-START) | 任务可以开始而不延迟项目完成的最迟日期。 |
| [LEVELING_CAN_SPLIT](#LEVELING-CAN-SPLIT) | 确定资源平衡功能是否会导致此任务剩余工作被拆分。 |
| [LEVELING_DELAY](#LEVELING-DELAY) | 由于资源平衡，任务从其最早开始日期被延迟的时间。 |
| [LEVEL_ASSIGNMENTS](#LEVEL-ASSIGNMENTS) | 确定平衡功能是否可以延迟并拆分各个分配以解决资源超额分配。 |
| [MANUAL_DURATION](#MANUAL-DURATION) | 定义任务的手动计划工期。 |
| [MANUAL_FINISH](#MANUAL-FINISH) | 定义任务的手动计划完成时间。 |
| [MANUAL_START](#MANUAL-START) | 定义任务的手动计划开始时间。 |
| [NAME](#NAME) | 任务名称。 |
| [NOTES_RTF](#NOTES-RTF) | RTF 格式的文本备注。 |
| [NOTES_TEXT](#NOTES-TEXT) | 从 RTF 数据中提取的备注纯文本。 |
| [OUTLINE_LEVEL](#OUTLINE-LEVEL) | 任务的大纲层级。 |
| [OUTLINE_NUMBER](#OUTLINE-NUMBER) | 表示任务在层次大纲结构中位置的编号。 |
| [OVERTIME_COST](#OVERTIME-COST) | 任务、资源在所有分配任务上或资源分配的加班总费用。 |
| [OVERTIME_WORK](#OVERTIME-WORK) | 分配给任务的所有资源计划执行的加班量。 |
| [PERCENT_COMPLETE](#PERCENT-COMPLETE) | 任务的当前状态，以已完成的任务工期百分比表示。 |
| [PERCENT_WORK_COMPLETE](#PERCENT-WORK-COMPLETE) | 任务的当前状态，以已完成的工作百分比表示。 |
| [PHYSICAL_PERCENT_COMPLETE](#PHYSICAL-PERCENT-COMPLETE) | 可用作计算已完成工作预算成本（BCWP）的替代值的完成百分比。 |
| [PRELEVELED_FINISH](#PRELEVELED-FINISH) | 资源平衡前任务的完成日期。 |
| [PRELEVELED_START](#PRELEVELED-START) | 资源平衡前任务的开始日期。 |
| [PRIORITY](#PRIORITY) | 任务的重要性等级，它指示在资源平衡期间任务或分配被延迟或拆分的可能性。 |
| [REGULAR_WORK](#REGULAR-WORK) | 资源计划执行的非加班工作总量。 |
| [REMAINING_COST](#REMAINING-COST) | 完成剩余计划工作将产生的剩余计划费用。 |
| [REMAINING_DURATION](#REMAINING-DURATION) | 完成任务未完成部分所需的时间。 |
| [REMAINING_OVERTIME_COST](#REMAINING-OVERTIME-COST) | 任务剩余的计划加班费用。 |
| [REMAINING_OVERTIME_WORK](#REMAINING-OVERTIME-WORK) | 剩余计划加班时间的数量。 |
| [REMAINING_WORK](#REMAINING-WORK) | 完成任务或任务集仍需的时间。 |
| [RESUME](#RESUME) | 任务剩余部分在进入任何进度后计划恢复的日期。 |
| [START](#START) | 任务的计划开始日期。 |
| [START_SLACK_TIME_SPAN](#START-SLACK-TIME-SPAN) | 提前开始日期和最迟开始日期之间的持续时间（秒）。 |
| [START_TEXT](#START-TEXT) | 返回任务的开始文本。 |
| [START_VARIANCE](#START-VARIANCE) | 表示任务或分配的基准开始日期与当前计划开始日期之间差异的时间。 |
| [STATUS_MANAGER](#STATUS-MANAGER) | 应从资源接收当前任务状态更新的企业资源的名称。 |
| [STOP](#STOP) | 表示任务实际部分结束的日期。 |
| [SUBPROJECT_NAME](#SUBPROJECT-NAME) | 子项目的源位置。 |
| [SV](#SV) | 截至项目状态日期的挣值进度偏差。 |
| [TOTAL_SLACK_TIME_SPAN](#TOTAL-SLACK-TIME-SPAN) | 任务完成日期可延迟而不影响项目完成日期的时间。 |
| [TYPE](#TYPE) | 任务的类型。 |
| [UID](#UID) | 任务的唯一标识符。 |
| [WARNING](#WARNING) | 表示 指示任务存在进度差异的标志。 |
| [WBS](#WBS) | 工作分解结构（WBS）代码。 |
| [WBS_LEVEL](#WBS-LEVEL) | 任务最右侧的 WBS 层级。 |
| [WORK](#WORK) | 为所有已分配资源在任务上计划的总时间。 |
| [WORK_VARIANCE](#WORK-VARIANCE) | 任务基准工作量与当前计划工作量之间的差异。 |
### Tsk() {#Tsk--}
```
public Tsk()
```


### ACTIVITY_ID {#ACTIVITY-ID}
```
public static final Key<String,Byte> ACTIVITY_ID
```


表示活动 ID 字段——Primavera 使用的任务唯一标识符。（仅适用于 Primavera 项目）

### ACTUAL_COST {#ACTUAL-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_COST
```


已由资源在其任务上完成的工作产生的费用，以及与任务相关的任何其他记录费用。

### ACTUAL_DURATION {#ACTUAL-DURATION}
```
public static final Key<Duration,Byte> ACTUAL_DURATION
```


基于计划工期和当前剩余工作量或完成百分比的任务实际工作时间跨度。

### ACTUAL_FINISH {#ACTUAL-FINISH}
```
public static final Key<Date,Byte> ACTUAL_FINISH
```


任务完成的日期。

### ACTUAL_OVERTIME_COST {#ACTUAL-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_OVERTIME_COST
```


已由指派资源在任务上完成的加班工作产生的费用。

### ACTUAL_OVERTIME_WORK {#ACTUAL-OVERTIME-WORK}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK
```


已由分配到任务的资源完成的实际加班工作量。

### ACTUAL_OVERTIME_WORK_PROTECTED {#ACTUAL-OVERTIME-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK_PROTECTED
```


实际加班工作受保护的持续时间。

### ACTUAL_START {#ACTUAL-START}
```
public static final Key<Date,Byte> ACTUAL_START
```


任务实际开始的日期和时间。

### ACTUAL_WORK {#ACTUAL-WORK}
```
public static final Key<Duration,Byte> ACTUAL_WORK
```


已由分配到任务的资源完成的工作量。

### ACTUAL_WORK_PROTECTED {#ACTUAL-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_WORK_PROTECTED
```


实际工作受保护的持续时间。

--------------------

仅支持读取 XML 格式。

### ACWP {#ACWP}
```
public static final Key<Double,Byte> ACWP
```


截至状态日期或今天的任务已完成工作产生的费用。

### BCWP {#BCWP}
```
public static final Key<Double,Byte> BCWP
```


任务完成百分比乘以时间分阶段基准成本的累计值。

### BCWS {#BCWS}
```
public static final Key<Double,Byte> BCWS
```


截至状态日期或今天的累计时间分阶段基准成本。

### BUDGET_COST {#BUDGET-COST}
```
public static final Key<BigDecimal,Byte> BUDGET_COST
```


预算成本资源的预算费用。预算资源仅分配给项目汇总任务。

### BUDGET_WORK {#BUDGET-WORK}
```
public static final Key<Duration,Byte> BUDGET_WORK
```


预算工作用于预算工作和物料资源。预算资源仅分配给项目汇总任务。

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Byte> CALENDAR
```


任务日历。

### COMMITMENT_FINISH {#COMMITMENT-FINISH}
```
public static final Key<Date,Byte> COMMITMENT_FINISH
```


交付的完成日期。

--------------------

仅支持读取 XML 格式。

### COMMITMENT_START {#COMMITMENT-START}
```
public static final Key<Date,Byte> COMMITMENT_START
```


交付的开始日期。

--------------------

仅支持读取 XML 格式。

### COMMITMENT_TYPE {#COMMITMENT-TYPE}
```
public static final Key<Integer,Byte> COMMITMENT_TYPE
```


确定任务是否具有关联的交付或对关联交付的依赖。

--------------------

仅支持读取 XML 格式。

### CONSTRAINT_DATE {#CONSTRAINT-DATE}
```
public static final Key<Date,Byte> CONSTRAINT_DATE
```


与约束类型关联的具体日期。

### CONSTRAINT_TYPE {#CONSTRAINT-TYPE}
```
public static final Key<Integer,Byte> CONSTRAINT_TYPE
```


提供可用于任务调度的约束类型选项。

### CONTACT {#CONTACT}
```
public static final Key<String,Byte> CONTACT
```


负责任务的个人姓名。

### COST {#COST}
```
public static final Key<BigDecimal,Byte> COST
```


任务的总计划或预测成本，基于已分配资源完成工作已产生的成本以及剩余工作计划的成本。

### COST_VARIANCE {#COST-VARIANCE}
```
public static final Key<Double,Byte> COST_VARIANCE
```


任务、资源或分配的基准成本与总成本之间的差额。

### CREATED {#CREATED}
```
public static final Key<Date,Byte> CREATED
```


任务创建的日期。

### CV {#CV}
```
public static final Key<Double,Byte> CV
```


任务的基准成本与总成本之间的差异。成本差异 = 成本 - 基准成本。

### DEADLINE {#DEADLINE}
```
public static final Key<Date,Byte> DEADLINE
```


指示任务完成时间的目标日期。

### DISPLAY_AS_SUMMARY {#DISPLAY-AS-SUMMARY}
```
public static final Key<NullableBool,Byte> DISPLAY_AS_SUMMARY
```


确定任务是否应显示为汇总任务。

--------------------

仅支持读取 XML 格式。

### DISPLAY_ON_TIMELINE {#DISPLAY-ON-TIMELINE}
```
public static final Key<Boolean,Byte> DISPLAY_ON_TIMELINE
```


指定任务是否应在时间轴视图中显示。

### DURATION {#DURATION}
```
public static final Key<Duration,Byte> DURATION
```


任务的总活跃工作时间跨度，按输入或 Microsoft Project 根据开始日期、结束日期、日历和其他调度因素计算得出。

### DURATION_TEXT {#DURATION-TEXT}
```
public static final Key<String,Byte> DURATION_TEXT
```


返回任务的持续时间文本。

### DURATION_VARIANCE {#DURATION-VARIANCE}
```
public static final Key<Duration,Byte> DURATION_VARIANCE
```


任务的基准持续时间与总持续时间（当前估计）之间的差异。

### EARLY_FINISH {#EARLY-FINISH}
```
public static final Key<Date,Byte> EARLY_FINISH
```


任务可能完成的最早日期，基于前置和后续任务的最早完成日期、其他约束以及任何平衡延迟。

### EARLY_START {#EARLY-START}
```
public static final Key<Date,Byte> EARLY_START
```


任务可能开始的最早日期，基于前置和后续任务的最早开始日期以及其他约束。

### EARNED_VALUE_METHOD {#EARNED-VALUE-METHOD}
```
public static final Key<Integer,Byte> EARNED_VALUE_METHOD
```


确定应使用“% 完成”还是“物理 % 完成”字段来计算已完成工作预算成本（BCWP）。

### EXTERNAL_ID {#EXTERNAL-ID}
```
public static final Key<Integer,Byte> EXTERNAL_ID
```


如果任务是外部任务，则包含该任务的外部 ID。

### EXTERNAL_TASK_PROJECT {#EXTERNAL-TASK-PROJECT}
```
public static final Key<String,Byte> EXTERNAL_TASK_PROJECT
```


外部任务的来源位置和任务标识符。

### EXTERNAL_UID {#EXTERNAL-UID}
```
public static final Key<Integer,Byte> EXTERNAL_UID
```


当任务为外部任务时，包含外部任务的唯一标识符。

### FINISH {#FINISH}
```
public static final Key<Date,Byte> FINISH
```


任务的计划完成日期。

### FINISH_SLACK_TIME_SPAN {#FINISH-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> FINISH_SLACK_TIME_SPAN
```


最早完成日期和最迟完成日期之间的持续时间（秒）。

### FINISH_TEXT {#FINISH-TEXT}
```
public static final Key<String,Byte> FINISH_TEXT
```


返回任务的完成文本。

### FINISH_VARIANCE {#FINISH-VARIANCE}
```
public static final Key<Duration,Byte> FINISH_VARIANCE
```


表示任务或分配的基准完成日期与当前完成日期之间差异的时间。

### FIXED_COST {#FIXED-COST}
```
public static final Key<Double,Byte> FIXED_COST
```


显示任何非资源任务费用。

### FIXED_COST_ACCRUAL {#FIXED-COST-ACCRUAL}
```
public static final Key<Integer,Byte> FIXED_COST_ACCRUAL
```


确定固定成本何时以及如何计入任务成本，或计提的选项。

### FREE_SLACK_TIME_SPAN {#FREE-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> FREE_SLACK_TIME_SPAN
```


任务可以延迟的时间（秒），且不会导致任何后继任务延迟。

### GUID {#GUID}
```
public static final Key<String,Byte> GUID
```


为任务生成的唯一标识代码。

### HAS_OVERALLOCATED_RESOURCE {#HAS-OVERALLOCATED-RESOURCE}
```
public static final Key<NullableBool,Byte> HAS_OVERALLOCATED_RESOURCE
```


指示任务是否分配了资源，该资源在已分配任务上的工作量超过正常工作容量。

### HIDE_BAR {#HIDE-BAR}
```
public static final Key<NullableBool,Byte> HIDE_BAR
```


确定在 Microsoft Project 中显示时，任务的甘特条是否隐藏。

### HYPERLINK {#HYPERLINK}
```
public static final Key<String,Byte> HYPERLINK
```


与任务关联的超链接的标题或说明文字。

### HYPERLINK_ADDRESS {#HYPERLINK-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_ADDRESS
```


与任务关联的超链接的地址。

--------------------

超链接的完整地址（Microsoft Project 中的 Hyperlink Href）是 HyperlinkAddress 与 HyperlinkSubAddress 的拼接。

### HYPERLINK_SUB_ADDRESS {#HYPERLINK-SUB-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_SUB_ADDRESS
```


与任务关联的超链接中文档的具体位置.

--------------------

超链接的完整地址（Microsoft Project 中的 Hyperlink Href）是 HyperlinkAddress 与 HyperlinkSubAddress 的拼接。

### ID {#ID}
```
public static final Key<Integer,Byte> ID
```


任务在任务列表中的位置标识符。

### IGNORE_RESOURCE_CALENDAR {#IGNORE-RESOURCE-CALENDAR}
```
public static final Key<NullableBool,Byte> IGNORE_RESOURCE_CALENDAR
```


确定任务的调度是否考虑分配给该任务的资源日历。

### IGNORE_WARNINGS {#IGNORE-WARNINGS}
```
public static final Key<Boolean,Byte> IGNORE_WARNINGS
```


指示是否在 Microsoft Project 中隐藏调度冲突警告指示器。

### IS_ACTIVE {#IS-ACTIVE}
```
public static final Key<NullableBool,Byte> IS_ACTIVE
```


确定任务是否处于活动状态。非活动任务不再影响其他任务或整体项目进度。

### IS_CRITICAL {#IS-CRITICAL}
```
public static final Key<NullableBool,Byte> IS_CRITICAL
```


确定任务是否位于关键路径上。

### IS_EFFORT_DRIVEN {#IS-EFFORT-DRIVEN}
```
public static final Key<NullableBool,Byte> IS_EFFORT_DRIVEN
```


确定任务的调度是否为基于工作量的调度。

### IS_ESTIMATED {#IS-ESTIMATED}
```
public static final Key<NullableBool,Byte> IS_ESTIMATED
```


确定任务是否为估算任务。

### IS_EXPANDED {#IS-EXPANDED}
```
public static final Key<NullableBool,Byte> IS_EXPANDED
```


确定在甘特图视图中汇总任务是否展开。

### IS_EXTERNAL_TASK {#IS-EXTERNAL-TASK}
```
public static final Key<Boolean,Byte> IS_EXTERNAL_TASK
```


确定任务是否为外部任务。

### IS_MANUAL {#IS-MANUAL}
```
public static final Key<NullableBool,Byte> IS_MANUAL
```


确定任务是否为手动调度。

### IS_MARKED {#IS-MARKED}
```
public static final Key<Boolean,Byte> IS_MARKED
```


显示任务是否被标记为需要进一步操作或某种标识。

--------------------

仅适用于 mpp 文件格式。

### IS_MILESTONE {#IS-MILESTONE}
```
public static final Key<NullableBool,Byte> IS_MILESTONE
```


确定任务是否为里程碑。

### IS_NULL {#IS-NULL}
```
public static final Key<NullableBool,Byte> IS_NULL
```


确定任务是否为空任务。

### IS_OVERALLOCATED {#IS-OVERALLOCATED}
```
public static final Key<NullableBool,Byte> IS_OVERALLOCATED
```


指示任务上分配的任何资源是否承担了超过正常工作容量的工作量。

### IS_PUBLISHED {#IS-PUBLISHED}
```
public static final Key<NullableBool,Byte> IS_PUBLISHED
```


确定当前任务是否应与项目的其他部分一起发布到 Project Server。

### IS_RECURRING {#IS-RECURRING}
```
public static final Key<NullableBool,Byte> IS_RECURRING
```


确定任务是否属于一系列循环任务。

### IS_RESUME_VALID {#IS-RESUME-VALID}
```
public static final Key<NullableBool,Byte> IS_RESUME_VALID
```


确定任务是否可以恢复。

### IS_ROLLUP {#IS-ROLLUP}
```
public static final Key<NullableBool,Byte> IS_ROLLUP
```


确定子任务甘特条的信息是否会汇总到汇总任务条中。

### IS_SUBPROJECT {#IS-SUBPROJECT}
```
public static final Key<Boolean,Byte> IS_SUBPROJECT
```


确定任务是否为插入的项目。

### IS_SUBPROJECT_READ_ONLY {#IS-SUBPROJECT-READ-ONLY}
```
public static final Key<NullableBool,Byte> IS_SUBPROJECT_READ_ONLY
```


确定子项目是否为只读。

### IS_SUMMARY {#IS-SUMMARY}
```
public static final Key<Boolean,Byte> IS_SUMMARY
```


确定任务是否为汇总任务。

### LATE_FINISH {#LATE-FINISH}
```
public static final Key<Date,Byte> LATE_FINISH
```


任务可以完成而不延迟项目完成的最迟日期。

### LATE_START {#LATE-START}
```
public static final Key<Date,Byte> LATE_START
```


任务可以开始而不延迟项目完成的最迟日期。

### LEVELING_CAN_SPLIT {#LEVELING-CAN-SPLIT}
```
public static final Key<NullableBool,Byte> LEVELING_CAN_SPLIT
```


确定资源平衡功能是否会导致此任务剩余工作被拆分。

### LEVELING_DELAY {#LEVELING-DELAY}
```
public static final Key<Duration,Byte> LEVELING_DELAY
```


由于资源平衡，任务从其最早开始日期被延迟的时间。

### LEVEL_ASSIGNMENTS {#LEVEL-ASSIGNMENTS}
```
public static final Key<NullableBool,Byte> LEVEL_ASSIGNMENTS
```


确定平衡功能是否可以延迟并拆分各个分配以解决资源超额分配。

### MANUAL_DURATION {#MANUAL-DURATION}
```
public static final Key<Duration,Byte> MANUAL_DURATION
```


定义任务的手动计划工期。

### MANUAL_FINISH {#MANUAL-FINISH}
```
public static final Key<Date,Byte> MANUAL_FINISH
```


定义任务的手动计划完成时间。

### MANUAL_START {#MANUAL-START}
```
public static final Key<Date,Byte> MANUAL_START
```


定义任务的手动计划开始时间。

### NAME {#NAME}
```
public static final Key<String,Byte> NAME
```


任务名称。

### NOTES_RTF {#NOTES-RTF}
```
public static final Key<String,Byte> NOTES_RTF
```


RTF 格式的文本备注。

--------------------

仅支持 MPP 格式。

### NOTES_TEXT {#NOTES-TEXT}
```
public static final Key<String,Byte> NOTES_TEXT
```


从 RTF 数据中提取的备注纯文本。

### OUTLINE_LEVEL {#OUTLINE-LEVEL}
```
public static final Key<Integer,Byte> OUTLINE_LEVEL
```


任务的大纲层级。

### OUTLINE_NUMBER {#OUTLINE-NUMBER}
```
public static final Key<String,Byte> OUTLINE_NUMBER
```


表示任务在层次大纲结构中位置的编号。

### OVERTIME_COST {#OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> OVERTIME_COST
```


任务、资源在所有分配任务上或资源分配的加班总费用。

### OVERTIME_WORK {#OVERTIME-WORK}
```
public static final Key<Duration,Byte> OVERTIME_WORK
```


分配给任务的所有资源计划执行的加班量。

### PERCENT_COMPLETE {#PERCENT-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_COMPLETE
```


任务的当前状态，以已完成的任务工期百分比表示。

### PERCENT_WORK_COMPLETE {#PERCENT-WORK-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_WORK_COMPLETE
```


任务的当前状态，以已完成的工作百分比表示。

### PHYSICAL_PERCENT_COMPLETE {#PHYSICAL-PERCENT-COMPLETE}
```
public static final Key<Integer,Byte> PHYSICAL_PERCENT_COMPLETE
```


可用作计算已完成工作预算成本（BCWP）的替代值的完成百分比。

### PRELEVELED_FINISH {#PRELEVELED-FINISH}
```
public static final Key<Date,Byte> PRELEVELED_FINISH
```


资源平衡前任务的完成日期。

### PRELEVELED_START {#PRELEVELED-START}
```
public static final Key<Date,Byte> PRELEVELED_START
```


资源平衡前任务的开始日期。

### PRIORITY {#PRIORITY}
```
public static final Key<Integer,Byte> PRIORITY
```


任务的重要性等级，它指示在资源平衡期间任务或分配被延迟或拆分的可能性。

### REGULAR_WORK {#REGULAR-WORK}
```
public static final Key<Duration,Byte> REGULAR_WORK
```


资源计划执行的非加班工作总量。

### REMAINING_COST {#REMAINING-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_COST
```


完成剩余计划工作将产生的剩余计划费用。

### REMAINING_DURATION {#REMAINING-DURATION}
```
public static final Key<Duration,Byte> REMAINING_DURATION
```


完成任务未完成部分所需的时间。

### REMAINING_OVERTIME_COST {#REMAINING-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_OVERTIME_COST
```


任务剩余的计划加班费用。

### REMAINING_OVERTIME_WORK {#REMAINING-OVERTIME-WORK}
```
public static final Key<Duration,Byte> REMAINING_OVERTIME_WORK
```


剩余计划加班时间的数量。

### REMAINING_WORK {#REMAINING-WORK}
```
public static final Key<Duration,Byte> REMAINING_WORK
```


完成任务或任务集仍需的时间。

### RESUME {#RESUME}
```
public static final Key<Date,Byte> RESUME
```


任务剩余部分在进入任何进度后计划恢复的日期。

### START {#START}
```
public static final Key<Date,Byte> START
```


任务的计划开始日期。

### START_SLACK_TIME_SPAN {#START-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> START_SLACK_TIME_SPAN
```


提前开始日期和最迟开始日期之间的持续时间（秒）。

### START_TEXT {#START-TEXT}
```
public static final Key<String,Byte> START_TEXT
```


返回任务的开始文本。

### START_VARIANCE {#START-VARIANCE}
```
public static final Key<Duration,Byte> START_VARIANCE
```


表示任务或分配的基准开始日期与当前计划开始日期之间差异的时间。

### STATUS_MANAGER {#STATUS-MANAGER}
```
public static final Key<String,Byte> STATUS_MANAGER
```


应从资源接收当前任务状态更新的企业资源的名称。

### STOP {#STOP}
```
public static final Key<Date,Byte> STOP
```


表示任务实际部分结束的日期。

### SUBPROJECT_NAME {#SUBPROJECT-NAME}
```
public static final Key<String,Byte> SUBPROJECT_NAME
```


子项目的源位置。

### SV {#SV}
```
public static final Key<Double,Byte> SV
```


截至项目状态日期的挣值进度偏差。进度偏差（SV）是 BCWP 与 BCWS 之间的差异。

### TOTAL_SLACK_TIME_SPAN {#TOTAL-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> TOTAL_SLACK_TIME_SPAN
```


任务完成日期可延迟而不影响项目完成日期的时间。

### TYPE {#TYPE}
```
public static final Key<Integer,Byte> TYPE
```


任务的类型。

### UID {#UID}
```
public static final Key<Integer,Byte> UID
```


任务的唯一标识符。

### WARNING {#WARNING}
```
public static final Key<Boolean,Byte> WARNING
```


表示 指示任务存在进度差异的标志。

### WBS {#WBS}
```
public static final Key<String,Byte> WBS
```


工作分解结构（WBS）代码。

### WBS_LEVEL {#WBS-LEVEL}
```
public static final Key<String,Byte> WBS_LEVEL
```


任务最右侧的 WBS 层级。

### WORK {#WORK}
```
public static final Key<Duration,Byte> WORK
```


为所有已分配资源在任务上计划的总时间。

### WORK_VARIANCE {#WORK-VARIANCE}
```
public static final Key<Duration,Byte> WORK_VARIANCE
```


任务基准工作量与当前计划工作量之间的差异。

