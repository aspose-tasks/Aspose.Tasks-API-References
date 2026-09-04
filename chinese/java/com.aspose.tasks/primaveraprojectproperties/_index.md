---
title: "PrimaveraProjectProperties"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示从 Primavera 文件 XER 或 P6XML 读取的项目的 Primavera 特定属性。"
type: docs
weight: 205
url: /zh/java/com.aspose.tasks/primaveraprojectproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectProperties
```

表示从 Primavera 文件（XER 或 P6XML）读取的项目的 Primavera 特定属性。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getBaselineProjects()](#getBaselineProjects--) | 获取当前项目的基线项目数组。 |
| [getCriticalActivitiesDefiningMethod()](#getCriticalActivitiesDefiningMethod--) | 获取用于定义关键活动的方法：最长路径或总浮动法。 |
| [getCriticalTotalFloatLimit()](#getCriticalTotalFloatLimit--) | 获取在使用 TotalFloat 方法时用于定义关键活动的阈值。 |
| [getCurrentBaselineProjectId()](#getCurrentBaselineProjectId--) | 获取当前基线项目的 Id。 |
| [getIgnoreOtherProjectRelationships()](#getIgnoreOtherProjectRelationships--) | 获取一个标志，用于定义是否忽略项目之间的活动关系。 |
| [getMakeOpenEndedActivitiesCritical()](#getMakeOpenEndedActivitiesCritical--) | 获取一个标志，用于定义在调度项目时是否应将活动标记为关键。 |
| [getRelationshipLagCalendar()](#getRelationshipLagCalendar--) | 获取一个选项，用于定义在 Primavera 项目中调度关系延迟时使用哪个日历。 |
| [getShortName()](#getShortName--) | 获取项目的短名称（项目 ID）。 |
| [getUseExpectedFinishDates()](#getUseExpectedFinishDates--) | 获取一个标志，用于定义活动完成日期是否应调度为预期完成日期。 |
### getBaselineProjects() {#getBaselineProjects--}
```
public final Project[] getBaselineProjects()
```


获取当前项目的基线项目数组。适用于读取包含已导出基线的 Primavera XML 文件的项目。

**Returns:**
com.aspose.tasks.Project[] - 当前项目的基线项目数组。
### getCriticalActivitiesDefiningMethod() {#getCriticalActivitiesDefiningMethod--}
```
public final int getCriticalActivitiesDefiningMethod()
```


获取用于定义关键活动的方法：最长路径或总浮动法。

**Returns:**
int - 用于定义关键活动的方法：最长路径或总浮动法。
### getCriticalTotalFloatLimit() {#getCriticalTotalFloatLimit--}
```
public final Double getCriticalTotalFloatLimit()
```


获取在使用 TotalFloat 方法时用于定义关键活动的阈值。

**Returns:**
java.lang.Double - 在使用 TotalFloat 方法时用于定义关键活动的阈值。
### getCurrentBaselineProjectId() {#getCurrentBaselineProjectId--}
```
public final int getCurrentBaselineProjectId()
```


获取当前基线项目的 Id。适用于读取包含已导出基线的 Primavera XML 文件的项目。

**Returns:**
int - 当前基线项目的 Id。
### getIgnoreOtherProjectRelationships() {#getIgnoreOtherProjectRelationships--}
```
public final boolean getIgnoreOtherProjectRelationships()
```


获取一个标志，用于定义是否忽略项目之间的活动关系。

**Returns:**
boolean - 一个标志，用于定义是否忽略项目之间的活动关系。
### getMakeOpenEndedActivitiesCritical() {#getMakeOpenEndedActivitiesCritical--}
```
public final boolean getMakeOpenEndedActivitiesCritical()
```


获取一个标志，用于定义在调度项目时是否应将活动标记为关键。

**Returns:**
boolean - 一个标志，用于定义在调度项目时是否应将活动标记为关键。
### getRelationshipLagCalendar() {#getRelationshipLagCalendar--}
```
public final int getRelationshipLagCalendar()
```


获取一个选项，用于定义在 Primavera 项目中调度关系延迟时使用哪个日历。

**Returns:**
int - 一个选项，用于定义在 Primavera 项目中调度关系延迟时使用哪个日历。
### getShortName() {#getShortName--}
```
public final String getShortName()
```


获取项目的短名称（项目 ID）。

**Returns:**
java.lang.String - 项目的短名称（项目 ID）。
### getUseExpectedFinishDates() {#getUseExpectedFinishDates--}
```
public final boolean getUseExpectedFinishDates()
```


获取一个标志，用于定义活动完成日期是否应调度为预期完成日期。

**Returns:**
boolean - 一个标志，用于定义活动完成日期是否应调度为预期完成日期。
