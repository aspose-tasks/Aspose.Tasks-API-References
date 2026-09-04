---
title: "PrimaveraTaskProperties"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示从 Primavera 文件 XER 或 P6XML 读取的任务的 Primavera 特定属性。"
type: docs
weight: 209
url: /zh/java/com.aspose.tasks/primaverataskproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraTaskProperties
```

表示从 Primavera 文件（XER 或 P6XML）读取的任务的 Primavera 特定属性。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getActivityId()](#getActivityId--) | 获取活动 ID 字段——Primavera 使用的任务唯一标识符。 |
| [getActivityType()](#getActivityType--) | 获取 'Activity Type' 字段的值。 |
| [getActualExpenseCost()](#getActualExpenseCost--) | 获取实际费用成本的值。 |
| [getActualLaborCost()](#getActualLaborCost--) | 获取实际人工成本的值。 |
| [getActualLaborUnits()](#getActualLaborUnits--) | 获取实际人工单位的值。 |
| [getActualMaterialCost()](#getActualMaterialCost--) | 获取实际材料成本的值。 |
| [getActualNonLaborUnits()](#getActualNonLaborUnits--) | 获取实际非人工单位的值。 |
| [getActualNonlaborCost()](#getActualNonlaborCost--) | 获取实际非人工成本的值。 |
| [getActualTotalCost()](#getActualTotalCost--) | 获取实际成本的总值。 |
| [getBudgetedExpenseCost()](#getBudgetedExpenseCost--) | 获取预算（或计划）费用成本的值。 |
| [getBudgetedLaborCost()](#getBudgetedLaborCost--) | 获取预算（或计划）人工成本的值。 |
| [getBudgetedMaterialCost()](#getBudgetedMaterialCost--) | 获取预算（或计划）材料成本的值。 |
| [getBudgetedNonlaborCost()](#getBudgetedNonlaborCost--) | 获取预算（或计划）非人工成本的值。 |
| [getBudgetedTotalCost()](#getBudgetedTotalCost--) | 获取预算（或计划）成本的总值。 |
| [getDurationPercentComplete()](#getDurationPercentComplete--) | 获取持续时间完成百分比的值。 |
| [getDurationType()](#getDurationType--) | 获取活动的 'Duration Type' 字段的值。 |
| [getPercentCompleteType()](#getPercentCompleteType--) | 获取活动的 '% Complete Type' 字段的值。 |
| [getPhysicalPercentComplete()](#getPhysicalPercentComplete--) | 获取实际完成百分比的值。 |
| [getPlannedDuration()](#getPlannedDuration--) | 获取原始或计划的持续时间——从任务计划开始日期到计划完成日期的总工作时间。 |
| [getPrimaryConstraintDate()](#getPrimaryConstraintDate--) | 获取主要约束的日期。 |
| [getPrimaryConstraintType()](#getPrimaryConstraintType--) | 获取主要约束的类型。 |
| [getRawActivityType()](#getRawActivityType--) | 获取活动的 'Activity Type' 字段的原始文本表示（如源文件中所示）。 |
| [getRawCompletePercentType()](#getRawCompletePercentType--) | 获取活动的 '% Complete Type' 字段的原始文本表示（如源文件中所示）。 |
| [getRawDurationType()](#getRawDurationType--) | 获取活动的 'Duration Type' 字段的原始文本表示（如源文件中所示）。 |
| [getRawStatus()](#getRawStatus--) | 获取活动的 'Status' 字段的原始文本表示（如源文件中所示）。 |
| [getRemainingEarlyFinish()](#getRemainingEarlyFinish--) | 获取剩余的提前完成日期——即活动剩余工作计划完成的日期。 |
| [getRemainingEarlyStart()](#getRemainingEarlyStart--) | 获取剩余的提前开始日期——即活动剩余工作计划开始的日期。 |
| [getRemainingExpenseCost()](#getRemainingExpenseCost--) | 获取剩余费用成本的值。 |
| [getRemainingLaborUnits()](#getRemainingLaborUnits--) | 获取剩余人工单位的值。 |
| [getRemainingLateFinish()](#getRemainingLateFinish--) | 获取剩余的延后完成日期。 |
| [getRemainingLateStart()](#getRemainingLateStart--) | 获取剩余的延后开始日期。 |
| [getRemainingNonLaborUnits()](#getRemainingNonLaborUnits--) | 获取剩余非人工单位的值。 |
| [getSecondaryConstraintDate()](#getSecondaryConstraintDate--) | 获取次要约束的日期。 |
| [getSecondaryConstraintType()](#getSecondaryConstraintType--) | 获取次要约束的类型。 |
| [getSequenceNumber()](#getSequenceNumber--) | 获取 WBS 项目的序列号（汇总任务）。 |
| [getUnitsPercentComplete()](#getUnitsPercentComplete--) | 获取单位完成百分比的值。 |
### getActivityId() {#getActivityId--}
```
public final String getActivityId()
```


获取活动 ID 字段——Primavera 使用的任务唯一标识符。

--------------------

仅适用于活动（非汇总任务）。

**Returns:**
java.lang.String - 活动 ID 字段 - 任务在 Primavera 中的唯一标识符。
### getActivityType() {#getActivityType--}
```
public final int getActivityType()
```


获取 'Activity Type' 字段的值。

--------------------

仅适用于活动（非汇总任务）。

**Returns:**
int - ‘Activity Type’ 字段的值。
### getActualExpenseCost() {#getActualExpenseCost--}
```
public final BigDecimal getActualExpenseCost()
```


获取实际费用成本的值。

**Returns:**
java.math.BigDecimal - 实际费用成本的值。
### getActualLaborCost() {#getActualLaborCost--}
```
public final BigDecimal getActualLaborCost()
```


获取实际人工成本的值。

**Returns:**
java.math.BigDecimal - 实际人工成本的值。
### getActualLaborUnits() {#getActualLaborUnits--}
```
public final double getActualLaborUnits()
```


获取实际人工单位的值。

**Returns:**
double - 实际人工单位的值。
### getActualMaterialCost() {#getActualMaterialCost--}
```
public final BigDecimal getActualMaterialCost()
```


获取实际材料成本的值。

**Returns:**
java.math.BigDecimal - 实际材料成本的值。
### getActualNonLaborUnits() {#getActualNonLaborUnits--}
```
public final double getActualNonLaborUnits()
```


获取实际非人工单位的值。

**Returns:**
double - 实际非人工单位的值。
### getActualNonlaborCost() {#getActualNonlaborCost--}
```
public final BigDecimal getActualNonlaborCost()
```


获取实际非人工成本的值。

**Returns:**
java.math.BigDecimal - 实际非人工成本的值。
### getActualTotalCost() {#getActualTotalCost--}
```
public final BigDecimal getActualTotalCost()
```


获取实际成本的总值。

**Returns:**
java.math.BigDecimal - 实际成本的总值。
### getBudgetedExpenseCost() {#getBudgetedExpenseCost--}
```
public final BigDecimal getBudgetedExpenseCost()
```


获取预算（或计划）费用成本的值。

**Returns:**
java.math.BigDecimal - 预算（或计划）费用成本的值。
### getBudgetedLaborCost() {#getBudgetedLaborCost--}
```
public final BigDecimal getBudgetedLaborCost()
```


获取预算（或计划）人工成本的值。

**Returns:**
java.math.BigDecimal - 预算（或计划）人工成本的值。
### getBudgetedMaterialCost() {#getBudgetedMaterialCost--}
```
public final BigDecimal getBudgetedMaterialCost()
```


获取预算（或计划）材料成本的值。

**Returns:**
java.math.BigDecimal - 预算（或计划）材料成本的值。
### getBudgetedNonlaborCost() {#getBudgetedNonlaborCost--}
```
public final BigDecimal getBudgetedNonlaborCost()
```


获取预算（或计划）非人工成本的值。

**Returns:**
java.math.BigDecimal - 预算（或计划）非人工成本的值。
### getBudgetedTotalCost() {#getBudgetedTotalCost--}
```
public final BigDecimal getBudgetedTotalCost()
```


获取预算（或计划）成本的总值。

**Returns:**
java.math.BigDecimal - 预算（或计划）成本的总值。
### getDurationPercentComplete() {#getDurationPercentComplete--}
```
public final double getDurationPercentComplete()
```


获取持续时间完成百分比的值。

**Returns:**
double - 持续时间百分比完成度的值。
### getDurationType() {#getDurationType--}
```
public final int getDurationType()
```


获取活动的 'Duration Type' 字段的值。

--------------------

仅适用于活动（非汇总任务）。

**Returns:**
int - 活动的 ‘Duration Type’ 字段的值。
### getPercentCompleteType() {#getPercentCompleteType--}
```
public final int getPercentCompleteType()
```


获取活动的 '% Complete Type' 字段的值。

--------------------

仅适用于活动（非汇总任务）。

**Returns:**
int - 活动的 ‘% Complete Type’ 字段的值。
### getPhysicalPercentComplete() {#getPhysicalPercentComplete--}
```
public final double getPhysicalPercentComplete()
```


获取实际完成百分比的值。

--------------------

仅适用于活动（非汇总任务）。

**Returns:**
double - 实际百分比完成度的值。
### getPlannedDuration() {#getPlannedDuration--}
```
public final Duration getPlannedDuration()
```


获取原始或计划的持续时间——从任务计划开始日期到计划完成日期的总工作时间。

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the original or planned duration -- the total working time from the task planned start date to the planned finish date.
### getPrimaryConstraintDate() {#getPrimaryConstraintDate--}
```
public final Date getPrimaryConstraintDate()
```


获取主要约束的日期。

**Returns:**
java.util.Date - 主要约束的日期。
### getPrimaryConstraintType() {#getPrimaryConstraintType--}
```
public final int getPrimaryConstraintType()
```


获取主要约束的类型。

**Returns:**
int - 主要约束的类型。
### getRawActivityType() {#getRawActivityType--}
```
public final String getRawActivityType()
```


获取活动的 'Activity Type' 字段的原始文本表示（如源文件中所示）。

--------------------

仅适用于活动（非汇总任务）。

**Returns:**
java.lang.String - 活动的 ‘Activity Type’ 字段的原始文本表示（如源文件中所示）。
### getRawCompletePercentType() {#getRawCompletePercentType--}
```
public final String getRawCompletePercentType()
```


获取活动的 '% Complete Type' 字段的原始文本表示（如源文件中所示）。

--------------------

仅适用于活动（非汇总任务）。

**Returns:**
java.lang.String - 活动的 ‘% Complete Type’ 字段的原始文本表示（如源文件中所示）。
### getRawDurationType() {#getRawDurationType--}
```
public final String getRawDurationType()
```


获取活动的 'Duration Type' 字段的原始文本表示（如源文件中所示）。

--------------------

仅适用于活动（非汇总任务）。

**Returns:**
java.lang.String - 活动的 ‘Duration Type’ 字段的原始文本表示（如源文件中所示）。
### getRawStatus() {#getRawStatus--}
```
public final String getRawStatus()
```


获取活动的 'Status' 字段的原始文本表示（如源文件中所示）。

--------------------

仅适用于活动（非汇总任务）。

**Returns:**
java.lang.String - 活动的 ‘Status’ 字段的原始文本表示（如源文件中所示）。
### getRemainingEarlyFinish() {#getRemainingEarlyFinish--}
```
public final Date getRemainingEarlyFinish()
```


获取剩余的提前完成日期——即活动剩余工作计划完成的日期。

**Returns:**
java.util.Date - 剩余提前完成日期 - 活动剩余工作计划完成的日期。
### getRemainingEarlyStart() {#getRemainingEarlyStart--}
```
public final Date getRemainingEarlyStart()
```


获取剩余的提前开始日期——即活动剩余工作计划开始的日期。

**Returns:**
java.util.Date - 剩余提前开始日期 - 活动的剩余工作计划开始的日期。
### getRemainingExpenseCost() {#getRemainingExpenseCost--}
```
public final BigDecimal getRemainingExpenseCost()
```


获取剩余费用成本的值。

**Returns:**
java.math.BigDecimal - 剩余费用成本的值。
### getRemainingLaborUnits() {#getRemainingLaborUnits--}
```
public final double getRemainingLaborUnits()
```


获取剩余人工单位的值。

**Returns:**
double - 剩余人工单位的值。
### getRemainingLateFinish() {#getRemainingLateFinish--}
```
public final Date getRemainingLateFinish()
```


获取剩余的延后完成日期。

**Returns:**
java.util.Date - 剩余延迟完成日期。
### getRemainingLateStart() {#getRemainingLateStart--}
```
public final Date getRemainingLateStart()
```


获取剩余的延后开始日期。

**Returns:**
java.util.Date - 剩余延迟开始日期。
### getRemainingNonLaborUnits() {#getRemainingNonLaborUnits--}
```
public final double getRemainingNonLaborUnits()
```


获取剩余非人工单位的值。

**Returns:**
double - 剩余非人工单位的值。
### getSecondaryConstraintDate() {#getSecondaryConstraintDate--}
```
public final Date getSecondaryConstraintDate()
```


获取次要约束的日期。

**Returns:**
java.util.Date - 次要约束的日期。
### getSecondaryConstraintType() {#getSecondaryConstraintType--}
```
public final int getSecondaryConstraintType()
```


获取次要约束的类型。

**Returns:**
int - 次要约束的类型。
### getSequenceNumber() {#getSequenceNumber--}
```
public final int getSequenceNumber()
```


获取 WBS 项目（汇总任务）的序列号。它用于在 Primavera 中对汇总任务进行排序。

--------------------

适用于 WBS 项目（汇总任务）。

**Returns:**
int - WBS 项目（汇总任务）的序列号。
### getUnitsPercentComplete() {#getUnitsPercentComplete--}
```
public final double getUnitsPercentComplete()
```


获取单位完成百分比的值。

**Returns:**
double - 完成百分比单位的值。
