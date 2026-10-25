---
title: "Tidslinje"
second_title: "Aspose.Tasks for Java API-referens"
description: "Definierar alternativ som anger hur tidslinjen ska renderas i Gantt-diagrammets uppgiftsanvändning eller resursanvändningsvyer när projektet exporteras till ett grafikformat."
type: docs
weight: 323
url: /sv/java/com.aspose.tasks/timescale/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class Timescale extends System.Enum
```

Definierar alternativ som anger hur tidslinjen ska renderas i Gantt-diagram, Uppgiftsanvändning eller Resursanvändning vyer när projektet exporteras till ett grafiskt format.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [Days](#Days) | Fördefinierad tvånivåers tidslinje där minsta detaljnivå är en dag. |
| [DefinedInView](#DefinedInView) | Använd tidslinjeinställningar som definierats i projektvyns egenskaper: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). |
| [Months](#Months) | Fördefinierad tvånivåers tidslinje där minsta detaljnivå är en månad. |
| [ThirdsOfMonths](#ThirdsOfMonths) | Fördefinierad tvånivåers tidslinje där detaljnivån är en tredjedel av en månad. |
### Days {#Days}
```
public static final int Days
```


Fördefinierad tvånivåers tidslinje där minsta detaljnivå är en dag.

### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


Använd tidslinjeinställningar som definierats i projektvyns egenskaper: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). Giltig för format som innehåller vydata. Till exempel projekt som läses från MPP-format.

--------------------

Om tidslinjeinställningarna inte är satta för vyn, används det fördefinierade Timescale.Days-inställningen istället.

### Months {#Months}
```
public static final int Months
```


Fördefinierad tvånivåers tidslinje där minsta detaljnivå är en månad.

### ThirdsOfMonths {#ThirdsOfMonths}
```
public static final int ThirdsOfMonths
```


Fördefinierad tvånivåers tidslinje där detaljnivån är en tredjedel av en månad.

