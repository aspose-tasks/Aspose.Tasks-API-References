---
title: "Rsc"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示 Resource 对象的受支持属性。"
type: docs
weight: 271
url: /zh/java/com.aspose.tasks/rsc/
---

**Inheritance:**
java.lang.Object
```
public class Rsc
```

表示 `Resource` 对象支持的属性。
## 字段

| 字段 | 描述 |
| --- | --- |
| [ACCRUE_AT](#ACCRUE-AT) | 确定资源的标准成本和加班成本何时以及如何计入任务成本，或计提。 |
| [ACTIVE_DIRECTORY_GUID](#ACTIVE-DIRECTORY-GUID) | 资源的 Active Directory Guid。 |
| [ACTUAL_COST](#ACTUAL-COST) | 已由资源在其任务上完成的工作产生的费用，以及与任务相关的任何其他记录费用。 |
| [ACTUAL_OVERTIME_COST](#ACTUAL-OVERTIME-COST) | 已由指派资源在任务上完成的加班工作产生的费用。 |
| [ACTUAL_OVERTIME_WORK](#ACTUAL-OVERTIME-WORK) | 指派给任务的资源已完成的实际加班工作量。 |
| [ACTUAL_OVERTIME_WORK_PROTECTED](#ACTUAL-OVERTIME-WORK-PROTECTED) | 实际加班工作受到保护的工作量。 |
| [ACTUAL_WORK](#ACTUAL-WORK) | 指派给任务的资源已完成的工作量。 |
| [ACTUAL_WORK_PROTECTED](#ACTUAL-WORK-PROTECTED) | 实际工作受到保护的工作量。 |
| [ACWP](#ACWP) | 资源截至目前为项目完成的工作的实际成本。 |
| [ASSIGNMENT_OWNER](#ASSIGNMENT-OWNER) | 指派所有者的名称。 |
| [ASSIGNMENT_OWNER_GUID](#ASSIGNMENT-OWNER-GUID) | 指派所有者的 GUID。 |
| [AVAILABLE_FROM](#AVAILABLE-FROM) | 资源在当前时间段内按指定单位可供工作的开始日期。 |
| [AVAILABLE_TO](#AVAILABLE-TO) | 资源在当前时间段指定单位内可工作的结束日期. |
| [BCWP](#BCWP) | 截至目前资源为项目执行的工作的预算成本. |
| [BCWS](#BCWS) | 为资源计划的工作的预算成本. |
| [BOOKING_TYPE](#BOOKING-TYPE) | 资源的预订类型. |
| [BUDGET_COST](#BUDGET-COST) | 预算成本资源的预算费用. |
| [BUDGET_WORK](#BUDGET-WORK) | 预算工作用于预算工作和材料资源. |
| [CALENDAR](#CALENDAR) | 资源的日历. |
| [CAN_LEVEL](#CAN-LEVEL) | 确定是否可以对资源进行资源平衡. |
| [CODE](#CODE) | 资源的代码或其他信息. |
| [COST](#COST) | 资源的总计划或预计成本，基于已分配给任务的资源执行工作已产生的成本，以及剩余工作计划的成本. |
| [COST_CENTER](#COST-CENTER) | 指示资源产生的费用应计入的成本中心. |
| [COST_PER_USE](#COST-PER-USE) | 每次使用资源时产生的费用. |
| [COST_VARIANCE](#COST-VARIANCE) | 资源的基准成本与总成本之间的差额. |
| [CREATED](#CREATED) | 资源添加到项目的日期和时间. |
| [CV](#CV) | 截至项目状态日期的挣值成本差异. |
| [E_MAIL_ADDRESS](#E-MAIL-ADDRESS) | 资源的电子邮件地址. |
| [FINISH](#FINISH) | 资源计划完成所有分配任务工作的日期. |
| [GROUP](#GROUP) | 资源所属的组. |
| [GUID](#GUID) | 包含为资源生成的唯一标识代码. |
| [HYPERLINK](#HYPERLINK) | 与资源关联的超链接的标题或说明文字. |
| [HYPERLINK_ADDRESS](#HYPERLINK-ADDRESS) | 与资源关联的超链接的地址. |
| [HYPERLINK_SUB_ADDRESS](#HYPERLINK-SUB-ADDRESS) | 与任务关联的超链接中文档的具体位置. |
| [ID](#ID) | 资源在资源列表中的位置标识符. |
| [INACTIVE](#INACTIVE) | 确定资源是否被具有管理员权限的用户设为非活动状态. |
| [INITIALS](#INITIALS) | 资源的缩写. |
| [IS_BUDGET](#IS-BUDGET) | 确定工作、材料或成本资源是否为预算资源。 |
| [IS_COST_RESOURCE](#IS-COST-RESOURCE) | 确定资源是否为成本资源。 |
| [IS_ENTERPRISE](#IS-ENTERPRISE) | 显示资源是来自企业资源池（true）还是本地资源池（false）。 |
| [IS_GENERIC](#IS-GENERIC) | 确定资源是否为通用资源。 |
| [IS_NULL](#IS-NULL) | 确定资源是否为 null。 |
| [IS_TEAM_ASSIGNMENT_POOL](#IS-TEAM-ASSIGNMENT-POOL) | 显示当前资源是否为团队资源。 |
| [MATERIAL_LABEL](#MATERIAL-LABEL) | 材料资源的计量单位。 |
| [MAX_UNITS](#MAX-UNITS) | 表示资源在当前时间段内可用于完成任何任务的最大容量的最大单位数。 |
| [NAME](#NAME) | 资源的名称。 |
| [NOTES_RTF](#NOTES-RTF) | RTF 格式的文本备注。 |
| [NOTES_TEXT](#NOTES-TEXT) | 从 RTF 数据中提取的备注纯文本。 |
| [OVERALLOCATED](#OVERALLOCATED) | 指示资源在特定任务或所有任务上分配的工作是否超过正常工作容量能够完成的范围。 |
| [OVERTIME_COST](#OVERTIME-COST) | 资源在所有分配任务上的加班总成本。 |
| [OVERTIME_RATE](#OVERTIME-RATE) | 资源执行的加班工作的工资率。 |
| [OVERTIME_RATE_FORMAT](#OVERTIME-RATE-FORMAT) | Microsoft Project 用于显示加班率的单位。 |
| [OVERTIME_WORK](#OVERTIME-WORK) | 计划由资源在任务上执行的加班量，并按相关资源的加班费率计费。 |
| [PEAK_UNITS](#PEAK-UNITS) | 资源在任何时刻对其分配的所有任务的最大分配单位。 |
| [PERCENT_WORK_COMPLETE](#PERCENT-WORK-COMPLETE) | 所有任务已完成工作的百分比。 |
| [PHONETICS](#PHONETICS) | 资源名称的音标拼写。 |
| [REGULAR_WORK](#REGULAR-WORK) | 资源计划执行的非加班工作总量。 |
| [REMAINING_COST](#REMAINING-COST) | 完成剩余计划工作将产生的剩余计划费用。 |
| [REMAINING_OVERTIME_COST](#REMAINING-OVERTIME-COST) | 资源剩余的计划加班费用。 |
| [REMAINING_OVERTIME_WORK](#REMAINING-OVERTIME-WORK) | 剩余计划加班的数量。 |
| [REMAINING_WORK](#REMAINING-WORK) | 完成任务或任务集仍需的时间。 |
| [STANDARD_RATE](#STANDARD-RATE) | 资源执行的常规非加班工作的工资率。 |
| [STANDARD_RATE_FORMAT](#STANDARD-RATE-FORMAT) | Microsoft Project 用于显示标准费率的单位。 |
| [START](#START) | 已分配资源计划开始在任务上工作的日期。 |
| [SV](#SV) | 截至项目状态日期的挣值进度偏差。 |
| [TYPE](#TYPE) | 资源的类型。 |
| [UID](#UID) | 资源的唯一标识符。 |
| [WINDOWS_USER_ACCOUNT](#WINDOWS-USER-ACCOUNT) | 与资源关联的 NT 帐户。 |
| [WORK](#WORK) | 资源在任务上计划的总时间量。 |
| [WORKGROUP](#WORKGROUP) | 资源所属工作组的类型。 |
| [WORK_VARIANCE](#WORK-VARIANCE) | 资源基线工作与当前计划工作之间的差异。 |
### ACCRUE_AT {#ACCRUE-AT}
```
public static final Key<Integer,Byte> ACCRUE_AT
```


确定资源的标准成本和加班成本何时以及如何计入任务成本，或计提。

### ACTIVE_DIRECTORY_GUID {#ACTIVE-DIRECTORY-GUID}
```
public static final Key<String,Byte> ACTIVE_DIRECTORY_GUID
```


资源的 Active Directory Guid。

### ACTUAL_COST {#ACTUAL-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_COST
```


已由资源在其任务上完成的工作产生的费用，以及与任务相关的任何其他记录费用。

### ACTUAL_OVERTIME_COST {#ACTUAL-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_OVERTIME_COST
```


已由指派资源在任务上完成的加班工作产生的费用。

### ACTUAL_OVERTIME_WORK {#ACTUAL-OVERTIME-WORK}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK
```


指派给任务的资源已完成的实际加班工作量。

### ACTUAL_OVERTIME_WORK_PROTECTED {#ACTUAL-OVERTIME-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK_PROTECTED
```


实际加班工作受到保护的工作量。

### ACTUAL_WORK {#ACTUAL-WORK}
```
public static final Key<Duration,Byte> ACTUAL_WORK
```


指派给任务的资源已完成的工作量。

### ACTUAL_WORK_PROTECTED {#ACTUAL-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_WORK_PROTECTED
```


实际工作受到保护的工作量。

### ACWP {#ACWP}
```
public static final Key<Double,Byte> ACWP
```


资源截至目前为项目完成的工作的实际成本。

### ASSIGNMENT_OWNER {#ASSIGNMENT-OWNER}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER
```


指派所有者的名称。

### ASSIGNMENT_OWNER_GUID {#ASSIGNMENT-OWNER-GUID}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER_GUID
```


指派所有者的 GUID。

### AVAILABLE_FROM {#AVAILABLE-FROM}
```
public static final Key<Date,Byte> AVAILABLE_FROM
```


资源在当前时间段内按指定单位可供工作的开始日期。

### AVAILABLE_TO {#AVAILABLE-TO}
```
public static final Key<Date,Byte> AVAILABLE_TO
```


资源在当前时间段指定单位内可工作的结束日期.

### BCWP {#BCWP}
```
public static final Key<Double,Byte> BCWP
```


截至目前资源为项目执行的工作的预算成本.

### BCWS {#BCWS}
```
public static final Key<Double,Byte> BCWS
```


为资源计划的工作的预算成本.

### BOOKING_TYPE {#BOOKING-TYPE}
```
public static final Key<Integer,Byte> BOOKING_TYPE
```


资源的预订类型.

### BUDGET_COST {#BUDGET-COST}
```
public static final Key<BigDecimal,Byte> BUDGET_COST
```


预算成本资源的预算费用。预算资源仅分配给项目汇总任务。

### BUDGET_WORK {#BUDGET-WORK}
```
public static final Key<Duration,Byte> BUDGET_WORK
```


预算工作用于预算工作和材料资源。预算资源仅分配给项目汇总任务。

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Byte> CALENDAR
```


资源的日历.

### CAN_LEVEL {#CAN-LEVEL}
```
public static final Key<NullableBool,Byte> CAN_LEVEL
```


确定是否可以对资源进行资源平衡.

### CODE {#CODE}
```
public static final Key<String,Byte> CODE
```


资源的代码或其他信息.

### COST {#COST}
```
public static final Key<BigDecimal,Byte> COST
```


资源的总计划或预计成本，基于已分配给任务的资源执行工作已产生的成本，以及剩余工作计划的成本.

### COST_CENTER {#COST-CENTER}
```
public static final Key<String,Byte> COST_CENTER
```


指示资源产生的费用应计入的成本中心.

### COST_PER_USE {#COST-PER-USE}
```
public static final Key<BigDecimal,Byte> COST_PER_USE
```


每次使用资源时产生的费用.

### COST_VARIANCE {#COST-VARIANCE}
```
public static final Key<Double,Byte> COST_VARIANCE
```


资源的基准成本与总成本之间的差额.

### CREATED {#CREATED}
```
public static final Key<Date,Byte> CREATED
```


资源添加到项目的日期和时间.

### CV {#CV}
```
public static final Key<Double,Byte> CV
```


截至项目状态日期的挣值成本偏差。CV 是任务的 BCWP（已完成工作预算成本）与 ACWP（实际完成工作成本）之间的差异。

### E_MAIL_ADDRESS {#E-MAIL-ADDRESS}
```
public static final Key<String,Byte> E_MAIL_ADDRESS
```


资源的电子邮件地址.

### FINISH {#FINISH}
```
public static final Key<Date,Byte> FINISH
```


资源计划完成所有分配任务工作的日期.

### GROUP {#GROUP}
```
public static final Key<String,Byte> GROUP
```


资源所属的组.

### GUID {#GUID}
```
public static final Key<String,Byte> GUID
```


包含为资源生成的唯一标识代码.

### HYPERLINK {#HYPERLINK}
```
public static final Key<String,Byte> HYPERLINK
```


与资源关联的超链接的标题或说明文字.

### HYPERLINK_ADDRESS {#HYPERLINK-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_ADDRESS
```


与资源关联的超链接的地址.

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


资源在资源列表中的位置标识符.

### INACTIVE {#INACTIVE}
```
public static final Key<NullableBool,Byte> INACTIVE
```


确定资源是否被具有管理员权限的用户设为非活动状态.

### INITIALS {#INITIALS}
```
public static final Key<String,Byte> INITIALS
```


资源的缩写.

### IS_BUDGET {#IS-BUDGET}
```
public static final Key<NullableBool,Byte> IS_BUDGET
```


确定工作、材料或成本资源是否为预算资源。

### IS_COST_RESOURCE {#IS-COST-RESOURCE}
```
public static final Key<NullableBool,Byte> IS_COST_RESOURCE
```


确定资源是否为成本资源。

### IS_ENTERPRISE {#IS-ENTERPRISE}
```
public static final Key<NullableBool,Byte> IS_ENTERPRISE
```


显示资源是来自企业资源池（true）还是本地资源池（false）。

### IS_GENERIC {#IS-GENERIC}
```
public static final Key<NullableBool,Byte> IS_GENERIC
```


确定资源是否为通用资源。

### IS_NULL {#IS-NULL}
```
public static final Key<NullableBool,Byte> IS_NULL
```


确定资源是否为 null。

### IS_TEAM_ASSIGNMENT_POOL {#IS-TEAM-ASSIGNMENT-POOL}
```
public static final Key<Boolean,Byte> IS_TEAM_ASSIGNMENT_POOL
```


显示当前资源是否为团队资源。

### MATERIAL_LABEL {#MATERIAL-LABEL}
```
public static final Key<String,Byte> MATERIAL_LABEL
```


材料资源的计量单位。

### MAX_UNITS {#MAX-UNITS}
```
public static final Key<Double,Byte> MAX_UNITS
```


表示资源在当前时间段内可用于完成任何任务的最大容量的最大单位数。

### NAME {#NAME}
```
public static final Key<String,Byte> NAME
```


资源的名称。

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
public static final Key<NullableBool,Byte> OVERALLOCATED
```


指示资源在特定任务或所有任务上分配的工作是否超过正常工作容量能够完成的范围。

### OVERTIME_COST {#OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> OVERTIME_COST
```


资源在所有分配任务上的加班总成本。

### OVERTIME_RATE {#OVERTIME-RATE}
```
public static final Key<BigDecimal,Byte> OVERTIME_RATE
```


资源执行的加班工作的工资率。

### OVERTIME_RATE_FORMAT {#OVERTIME-RATE-FORMAT}
```
public static final Key<Integer,Byte> OVERTIME_RATE_FORMAT
```


Microsoft Project 用于显示加班率的单位。

### OVERTIME_WORK {#OVERTIME-WORK}
```
public static final Key<Duration,Byte> OVERTIME_WORK
```


计划由资源在任务上执行的加班量，并按相关资源的加班费率计费。

### PEAK_UNITS {#PEAK-UNITS}
```
public static final Key<Double,Byte> PEAK_UNITS
```


资源在任何时刻对其分配的所有任务的最大分配单位。

### PERCENT_WORK_COMPLETE {#PERCENT-WORK-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_WORK_COMPLETE
```


所有任务已完成工作的百分比。

### PHONETICS {#PHONETICS}
```
public static final Key<String,Byte> PHONETICS
```


资源名称的音标拼写。仅用于日语。

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

### REMAINING_OVERTIME_COST {#REMAINING-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_OVERTIME_COST
```


资源剩余的计划加班费用。

### REMAINING_OVERTIME_WORK {#REMAINING-OVERTIME-WORK}
```
public static final Key<Duration,Byte> REMAINING_OVERTIME_WORK
```


剩余计划加班的数量。

### REMAINING_WORK {#REMAINING-WORK}
```
public static final Key<Duration,Byte> REMAINING_WORK
```


完成任务或任务集仍需的时间。

### STANDARD_RATE {#STANDARD-RATE}
```
public static final Key<BigDecimal,Byte> STANDARD_RATE
```


资源执行的常规非加班工作的工资率。

### STANDARD_RATE_FORMAT {#STANDARD-RATE-FORMAT}
```
public static final Key<Integer,Byte> STANDARD_RATE_FORMAT
```


Microsoft Project 用于显示标准费率的单位。

### START {#START}
```
public static final Key<Date,Byte> START
```


已分配资源计划开始在任务上工作的日期。

### SV {#SV}
```
public static final Key<Double,Byte> SV
```


截至项目状态日期的挣值进度偏差。SV 是已完成工作预算成本 (BCWP) 与已计划工作预算成本 (BCWS) 之间的差异。

### TYPE {#TYPE}
```
public static final Key<Integer,Byte> TYPE
```


资源的类型。

### UID {#UID}
```
public static final Key<Integer,Byte> UID
```


资源的唯一标识符。

### WINDOWS_USER_ACCOUNT {#WINDOWS-USER-ACCOUNT}
```
public static final Key<String,Byte> WINDOWS_USER_ACCOUNT
```


与资源关联的 NT 帐户。

### WORK {#WORK}
```
public static final Key<Duration,Byte> WORK
```


资源在任务上计划的总时间量。

### WORKGROUP {#WORKGROUP}
```
public static final Key<Integer,Byte> WORKGROUP
```


资源所属工作组的类型。

### WORK_VARIANCE {#WORK-VARIANCE}
```
public static final Key<Double,Byte> WORK_VARIANCE
```


资源基线工作与当前计划工作之间的差异。

