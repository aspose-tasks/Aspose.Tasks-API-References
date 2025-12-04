---
title: Timescale
second_title: Aspose.Tasks for Java API Reference
description: Defines options which specifies how to render timescale in Gantt Chart Task Usage or Resource Usage views when the project is exported to a graphic format.
type: docs
weight: 320
url: /java/com.aspose.tasks/timescale/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class Timescale extends System.Enum
```

Defines options which specifies how to render timescale in Gantt Chart, Task Usage or Resource Usage views when the project is exported to a graphic format.
## Fields

| Field | Description |
| --- | --- |
| [Days](#Days) | Predefined two-tiered timescale where minimal level of detail is one day. |
| [DefinedInView](#DefinedInView) | Use timescale settings defined in project view's properties: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). |
| [Months](#Months) | Predefined two-tiered timescale where minimal level of detail is one month. |
| [ThirdsOfMonths](#ThirdsOfMonths) | Predefined two-tiered timescale where level of detail is one third of month. |
### Days {#Days}
```
public static final int Days
```


Predefined two-tiered timescale where minimal level of detail is one day.

### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


Use timescale settings defined in project view's properties: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). Valid for formats which contains view data. For example, projects which are read from MPP format.

--------------------

If timescale settings are not set for the view, predefined Timescale.Days setting is used instead.

### Months {#Months}
```
public static final int Months
```


Predefined two-tiered timescale where minimal level of detail is one month.

### ThirdsOfMonths {#ThirdsOfMonths}
```
public static final int ThirdsOfMonths
```


Predefined two-tiered timescale where level of detail is one third of month.

