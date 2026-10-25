---
title: "Timescale"
second_title: "Aspose.Tasks for Java API 参考"
description: "定义选项，指定在项目导出为图形格式时，如何在 Gantt Chart Task Usage 或 Resource Usage 视图中呈现时间尺度。"
type: docs
weight: 323
url: /zh/java/com.aspose.tasks/timescale/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class Timescale extends System.Enum
```

定义选项，指定项目导出为图形格式时，如何在甘特图、任务使用或资源使用视图中渲染时间尺度。
## 字段

| 字段 | 描述 |
| --- | --- |
| [Days](#Days) | 预定义的两层时间尺度，最小细节级别为一天。 |
| [DefinedInView](#DefinedInView) | 使用在项目视图属性中定义的时间尺度设置： `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). |
| [Months](#Months) | 预定义的两层时间尺度，最小细节级别为一个月。 |
| [ThirdsOfMonths](#ThirdsOfMonths) | 预定义的两层时间尺度，细节级别为一个月的三分之一。 |
### Days {#Days}
```
public static final int Days
```


预定义的两层时间尺度，最小细节级别为一天。

### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


使用在项目视图属性中定义的时间尺度设置： `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). 适用于包含视图数据的格式。例如，从 MPP 格式读取的项目。

--------------------

如果视图未设置时间尺度，则使用预定义的 Timescale.Days 设置。

### Months {#Months}
```
public static final int Months
```


预定义的两层时间尺度，最小细节级别为一个月。

### ThirdsOfMonths {#ThirdsOfMonths}
```
public static final int ThirdsOfMonths
```


预定义的两层时间尺度，细节级别为一个月的三分之一。

