---
title: "Timescale"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Definieert opties die specificeren hoe de tijdsschaal moet worden weergegeven in Gantt‑diagram Taakgebruik‑ of Resourcegebruik‑weergaven wanneer het project wordt geëxporteerd naar een grafisch formaat."
type: docs
weight: 323
url: /nl/java/com.aspose.tasks/timescale/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class Timescale extends System.Enum
```

Definieert opties die specificeren hoe de tijdschaal moet worden gerenderd in Gantt-diagram-, taakgebruik- of resourcegebruikweergaven wanneer het project wordt geëxporteerd naar een grafisch formaat.
## Velden

| Veld | Beschrijving |
| --- | --- |
| [Days](#Days) | Vooraf gedefinieerde tweelaagse tijdsschaal waarbij het minimale detailniveau één dag is. |
| [DefinedInView](#DefinedInView) | Gebruik tijdsschaalinstellingen die zijn gedefinieerd in de eigenschappen van de projectweergave: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). |
| [Months](#Months) | Vooraf gedefinieerde tweelaagse tijdsschaal waarbij het minimale detailniveau één maand is. |
| [ThirdsOfMonths](#ThirdsOfMonths) | Vooraf gedefinieerde tweelaagse tijdschaal waarbij het detailniveau één derde van een maand is. |
### Days {#Days}
```
public static final int Days
```


Vooraf gedefinieerde tweelaagse tijdsschaal waarbij het minimale detailniveau één dag is.

### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


Gebruik de tijdschaalinstellingen die zijn gedefinieerd in de eigenschappen van de projectweergave: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). Geldig voor formaten die weergavegegevens bevatten. Bijvoorbeeld projecten die uit MPP-formaat worden gelezen.

--------------------

Als de tijdschaalinstellingen niet zijn ingesteld voor de weergave, wordt in plaats daarvan de vooraf gedefinieerde Timescale.Days-instelling gebruikt.

### Months {#Months}
```
public static final int Months
```


Vooraf gedefinieerde tweelaagse tijdsschaal waarbij het minimale detailniveau één maand is.

### ThirdsOfMonths {#ThirdsOfMonths}
```
public static final int ThirdsOfMonths
```


Vooraf gedefinieerde tweelaagse tijdschaal waarbij het detailniveau één derde van een maand is.

