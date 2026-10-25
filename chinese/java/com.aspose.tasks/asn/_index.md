---
title: "Asn"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示对象的属性。"
type: docs
weight: 15
url: /zh/java/com.aspose.tasks/asn/
---

**Inheritance:**
java.lang.Object
```
public class Asn
```

表示 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 对象的属性。
## 字段

| 字段 | 描述 |
| --- | --- |
| [ACTUAL_COST](#ACTUAL-COST) | 在任务分配上实际产生的成本。 |
| [ACTUAL_FINISH](#ACTUAL-FINISH) | 任务分配的实际完成日期。 |
| [ACTUAL_OVERTIME_COST](#ACTUAL-OVERTIME-COST) | 任务分配上实际产生的加班成本。 |
| [ACTUAL_OVERTIME_WORK](#ACTUAL-OVERTIME-WORK) | 任务分配上实际产生的加班工作量。 |
| [ACTUAL_OVERTIME_WORK_PROTECTED](#ACTUAL-OVERTIME-WORK-PROTECTED) | 实际工作受保护的持续时间。 |
| [ACTUAL_START](#ACTUAL-START) | 任务分配的实际开始日期。 |
| [ACTUAL_WORK](#ACTUAL-WORK) | 任务分配上实际产生的工作量。 |
| [ACTUAL_WORK_PROTECTED](#ACTUAL-WORK-PROTECTED) | 实际加班工作受保护的持续时间。 |
| [ACWP](#ACWP) | 截至目前在任务分配上执行的工作的实际成本。 |
| [ASSIGNMENT_OWNER](#ASSIGNMENT-OWNER) | 指派所有者的名称。 |
| [ASSIGNMENT_OWNER_GUID](#ASSIGNMENT-OWNER-GUID) | 任务分配所有者的全局唯一标识符。 |
| [BCWP](#BCWP) | 截至目前在任务分配上执行的工作的预算成本。 |
| [BCWS](#BCWS) | 任务分配上工作的预算成本。 |
| [BOOKING_TYPE](#BOOKING-TYPE) | 任务分配的预订类型。 |
| [BUDGET_COST](#BUDGET-COST) | 任务分配上资源的预算成本。 |
| [BUDGET_WORK](#BUDGET-WORK) | 任务分配上工作或材料资源的预算工作量。 |
| [CONFIRMED](#CONFIRMED) | 确定资源是否已接受其所有任务分配。 |
| [COST](#COST) | 任务分配的预计或计划成本。 |
| [COST_RATE_TABLE_TYPE](#COST-RATE-TABLE-TYPE) | 此任务分配使用的成本费率表。 |
| [COST_VARIANCE](#COST-VARIANCE) | 任务分配的基准成本与总成本之间的差额。 |
| [CREATED](#CREATED) | 任务分配创建的日期。 |
| [CV](#CV) | 已赚价值成本差异。 |
| [DELAY](#DELAY) | 任务的延迟。 |
| [FINISH](#FINISH) | 任务的计划完成日期。 |
| [FINISH_VARIANCE](#FINISH-VARIANCE) | 任务完成日期相对于基准完成日期的差异。 |
| [FIXED_MATERIAL](#FIXED-MATERIAL) | 确定已分配的材料资源的消耗是否以单一、固定的数量发生。 |
| [HAS_FIXED_RATE_UNITS](#HAS-FIXED-RATE-UNITS) | 确定单位是否具有固定费率。 |
| [HYPERLINK](#HYPERLINK) | 与任务关联的超链接的标题或说明文字。 |
| [HYPERLINK_ADDRESS](#HYPERLINK-ADDRESS) | 与任务关联的超链接的地址。 |
| [HYPERLINK_SUB_ADDRESS](#HYPERLINK-SUB-ADDRESS) | 与任务关联的超链接在文档中的具体位置。 |
| [LEVELING_DELAY](#LEVELING-DELAY) | 资源平衡导致的延迟。 |
| [LINKED_FIELDS](#LINKED-FIELDS) | 确定项目是否链接到另一个 OLE 对象。 |
| [MILESTONE](#MILESTONE) | 确定任务是否为里程碑。 |
| [NOTES_RTF](#NOTES-RTF) | RTF 格式的文本备注。 |
| [NOTES_TEXT](#NOTES-TEXT) | 从 RTF 数据中提取的备注纯文本。 |
| [OVERALLOCATED](#OVERALLOCATED) | 确定任务是否超额分配。 |
| [OVERTIME_COST](#OVERTIME-COST) | 任务的实际加班成本与剩余加班成本之和。 |
| [OVERTIME_WORK](#OVERTIME-WORK) | 任务的计划加班工作。 |
| [PEAK_UNITS](#PEAK-UNITS) | 资源为任务分配的最大单位数。 |
| [PERCENT_WORK_COMPLETE](#PERCENT-WORK-COMPLETE) | 任务已完成工作的量。 |
| [RATE_SCALE](#RATE-SCALE) | 材料资源分配使用率的时间单位。 |
| [REGULAR_WORK](#REGULAR-WORK) | 任务计划的非加班工作量。 |
| [REMAINING_COST](#REMAINING-COST) | 完成任务的剩余预计成本。 |
| [REMAINING_OVERTIME_COST](#REMAINING-OVERTIME-COST) | 完成任务的剩余预计加班成本。 |
| [REMAINING_OVERTIME_WORK](#REMAINING-OVERTIME-WORK) | 完成任务计划的剩余加班工作。 |
| [REMAINING_WORK](#REMAINING-WORK) | 完成任务计划的剩余工作。 |
| [RESOURCE](#RESOURCE) | 分配给任务的资源。 |
| [RESPONSE_PENDING](#RESPONSE-PENDING) | 确定是否已收到对 TeamAssign 消息的响应。 |
| [RESUME](#RESUME) | 恢复任务分配的日期。 |
| [START](#START) | 任务分配的计划开始日期。 |
| [START_VARIANCE](#START-VARIANCE) | 任务分配开始日期相对于基准开始日期的偏差。 |
| [STOP](#STOP) | 停止任务分配的日期。 |
| [SUMMARY](#SUMMARY) | 确定任务是否为汇总任务。 |
| [SV](#SV) | 截至项目状态日期的挣值进度偏差。 |
| [TASK](#TASK) | 资源被分配到的任务。 |
| [UID](#UID) | 任务分配的唯一标识符。 |
| [UNITS](#UNITS) | 任务分配的单位数。 |
| [UPDATE_NEEDED](#UPDATE-NEEDED) | 确定分配给任务的资源是否需要根据任务状态进行更新。 |
| [VAC](#VAC) | 基准成本与总成本之间的差额。 |
| [WORK](#WORK) | 任务分配的计划工作量。 |
| [WORK_CONTOUR](#WORK-CONTOUR) | 任务分配的工作轮廓。 |
| [WORK_VARIANCE](#WORK-VARIANCE) | 任务基准工作量与当前计划工作量之间的差异。 |
### ACTUAL_COST {#ACTUAL-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_COST
```


在任务分配上实际产生的成本。

### ACTUAL_FINISH {#ACTUAL-FINISH}
```
public static final Key<Date,Byte> ACTUAL_FINISH
```


任务分配的实际完成日期。

### ACTUAL_OVERTIME_COST {#ACTUAL-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_OVERTIME_COST
```


任务分配上实际产生的加班成本。

### ACTUAL_OVERTIME_WORK {#ACTUAL-OVERTIME-WORK}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK
```


任务分配上实际产生的加班工作量。

### ACTUAL_OVERTIME_WORK_PROTECTED {#ACTUAL-OVERTIME-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK_PROTECTED
```


实际工作受保护的持续时间。

### ACTUAL_START {#ACTUAL-START}
```
public static final Key<Date,Byte> ACTUAL_START
```


任务分配的实际开始日期。

### ACTUAL_WORK {#ACTUAL-WORK}
```
public static final Key<Duration,Byte> ACTUAL_WORK
```


任务分配上实际产生的工作量。

### ACTUAL_WORK_PROTECTED {#ACTUAL-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_WORK_PROTECTED
```


实际加班工作受保护的持续时间。

### ACWP {#ACWP}
```
public static final Key<Double,Byte> ACWP
```


截至目前在任务分配上执行的工作的实际成本。

### ASSIGNMENT_OWNER {#ASSIGNMENT-OWNER}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER
```


指派所有者的名称。

### ASSIGNMENT_OWNER_GUID {#ASSIGNMENT-OWNER-GUID}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER_GUID
```


任务分配所有者的全局唯一标识符。

### BCWP {#BCWP}
```
public static final Key<Double,Byte> BCWP
```


截至目前在任务分配上执行的工作的预算成本。

### BCWS {#BCWS}
```
public static final Key<Double,Byte> BCWS
```


任务分配上工作的预算成本。

### BOOKING_TYPE {#BOOKING-TYPE}
```
public static final Key<Integer,Byte> BOOKING_TYPE
```


任务分配的预订类型。

### BUDGET_COST {#BUDGET-COST}
```
public static final Key<BigDecimal,Byte> BUDGET_COST
```


任务分配上资源的预算成本。

### BUDGET_WORK {#BUDGET-WORK}
```
public static final Key<Duration,Byte> BUDGET_WORK
```


任务分配上工作或材料资源的预算工作量。

### CONFIRMED {#CONFIRMED}
```
public static final Key<Boolean,Byte> CONFIRMED
```


确定资源是否已接受其所有任务分配。

### COST {#COST}
```
public static final Key<BigDecimal,Byte> COST
```


任务分配的预计或计划成本。

### COST_RATE_TABLE_TYPE {#COST-RATE-TABLE-TYPE}
```
public static final Key<Integer,Byte> COST_RATE_TABLE_TYPE
```


此任务分配使用的成本费率表。

### COST_VARIANCE {#COST-VARIANCE}
```
public static final Key<Double,Byte> COST_VARIANCE
```


任务分配的基准成本与总成本之间的差额。

### CREATED {#CREATED}
```
public static final Key<Date,Byte> CREATED
```


任务分配创建的日期。

### CV {#CV}
```
public static final Key<Double,Byte> CV
```


已获价值成本偏差。CV 是任务的 BCWP（已完成工作预算成本）与 ACWP（实际完成工作成本）之间的差额。

### DELAY {#DELAY}
```
public static final Key<Duration,Byte> DELAY
```


任务的延迟。

### FINISH {#FINISH}
```
public static final Key<Date,Byte> FINISH
```


任务的计划完成日期。

### FINISH_VARIANCE {#FINISH-VARIANCE}
```
public static final Key<Duration,Byte> FINISH_VARIANCE
```


任务完成日期相对于基准完成日期的差异。

### FIXED_MATERIAL {#FIXED-MATERIAL}
```
public static final Key<Boolean,Byte> FIXED_MATERIAL
```


确定已分配的材料资源的消耗是否以单一、固定的数量发生。

### HAS_FIXED_RATE_UNITS {#HAS-FIXED-RATE-UNITS}
```
public static final Key<Boolean,Byte> HAS_FIXED_RATE_UNITS
```


确定单位是否具有固定费率。

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


与任务关联的超链接在文档中的具体位置。

--------------------

超链接的完整地址（Microsoft Project 中的 Hyperlink Href）是 HyperlinkAddress 与 HyperlinkSubAddress 的拼接。

### LEVELING_DELAY {#LEVELING-DELAY}
```
public static final Key<Duration,Byte> LEVELING_DELAY
```


资源平衡导致的延迟。

### LINKED_FIELDS {#LINKED-FIELDS}
```
public static final Key<Boolean,Byte> LINKED_FIELDS
```


确定项目是否链接到另一个 OLE 对象。

### MILESTONE {#MILESTONE}
```
public static final Key<Boolean,Byte> MILESTONE
```


确定任务是否为里程碑。

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

### OVERALLOCATED {#OVERALLOCATED}
```
public static final Key<Boolean,Byte> OVERALLOCATED
```


确定任务是否超额分配。

### OVERTIME_COST {#OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> OVERTIME_COST
```


任务的实际加班成本与剩余加班成本之和。

### OVERTIME_WORK {#OVERTIME-WORK}
```
public static final Key<Duration,Byte> OVERTIME_WORK
```


任务的计划加班工作。

### PEAK_UNITS {#PEAK-UNITS}
```
public static final Key<Double,Byte> PEAK_UNITS
```


资源为任务分配的最大单位数。

### PERCENT_WORK_COMPLETE {#PERCENT-WORK-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_WORK_COMPLETE
```


任务已完成工作的量。

### RATE_SCALE {#RATE-SCALE}
```
public static final Key<Integer,Byte> RATE_SCALE
```


物料资源分配使用率的时间单位。如果未定义，返回 0。

### REGULAR_WORK {#REGULAR-WORK}
```
public static final Key<Duration,Byte> REGULAR_WORK
```


任务计划的非加班工作量。

### REMAINING_COST {#REMAINING-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_COST
```


完成任务的剩余预计成本。

### REMAINING_OVERTIME_COST {#REMAINING-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_OVERTIME_COST
```


完成任务的剩余预计加班成本。

### REMAINING_OVERTIME_WORK {#REMAINING-OVERTIME-WORK}
```
public static final Key<Duration,Byte> REMAINING_OVERTIME_WORK
```


完成任务计划的剩余加班工作。

### REMAINING_WORK {#REMAINING-WORK}
```
public static final Key<Duration,Byte> REMAINING_WORK
```


完成任务计划的剩余工作。

### RESOURCE {#RESOURCE}
```
public static final Key<Resource,Byte> RESOURCE
```


分配给任务的资源。

### RESPONSE_PENDING {#RESPONSE-PENDING}
```
public static final Key<Boolean,Byte> RESPONSE_PENDING
```


确定是否已收到对 TeamAssign 消息的响应。

### RESUME {#RESUME}
```
public static final Key<Date,Byte> RESUME
```


恢复任务分配的日期。

### START {#START}
```
public static final Key<Date,Byte> START
```


任务分配的计划开始日期。

### START_VARIANCE {#START-VARIANCE}
```
public static final Key<Duration,Byte> START_VARIANCE
```


任务分配开始日期相对于基准开始日期的偏差。

### STOP {#STOP}
```
public static final Key<Date,Byte> STOP
```


停止任务分配的日期。

### SUMMARY {#SUMMARY}
```
public static final Key<Boolean,Byte> SUMMARY
```


确定任务是否为汇总任务。

### SV {#SV}
```
public static final Key<Double,Byte> SV
```


截至项目状态日期的挣值进度偏差。进度偏差（SV）是 BCWP 与 BCWS 之间的差异。

### TASK {#TASK}
```
public static final Key<Task,Byte> TASK
```


资源被分配到的任务。

### UID {#UID}
```
public static final Key<Integer,Byte> UID
```


任务分配的唯一标识符。

### UNITS {#UNITS}
```
public static final Key<Double,Byte> UNITS
```


任务分配的单位数。

### UPDATE_NEEDED {#UPDATE-NEEDED}
```
public static final Key<Boolean,Byte> UPDATE_NEEDED
```


确定分配给任务的资源是否需要根据任务状态进行更新。

### VAC {#VAC}
```
public static final Key<Double,Byte> VAC
```


基准成本与总成本之间的差额。

### WORK {#WORK}
```
public static final Key<Duration,Byte> WORK
```


任务分配的计划工作量。

### WORK_CONTOUR {#WORK-CONTOUR}
```
public static final Key<Integer,Byte> WORK_CONTOUR
```


任务分配的工作轮廓。

### WORK_VARIANCE {#WORK-VARIANCE}
```
public static final Key<Duration,Byte> WORK_VARIANCE
```


任务基准工作量与当前计划工作量之间的差异。

