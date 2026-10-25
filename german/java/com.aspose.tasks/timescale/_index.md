---
title: "Zeitachse"
second_title: "Aspose.Tasks for Java API Reference"
description: "Definiert Optionen, die festlegen, wie die Zeitachse in den Gantt Chart Task Usage‑ oder Resource Usage‑Ansichten gerendert wird, wenn das Projekt in ein Grafikformat exportiert wird."
type: docs
weight: 323
url: /de/java/com.aspose.tasks/timescale/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class Timescale extends System.Enum
```

Definiert Optionen, die angeben, wie die Zeitskala in Gantt-Diagramm-, Aufgabenverbrauchs- oder Ressourcennutzungsansichten gerendert wird, wenn das Projekt in ein Grafikformat exportiert wird.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [Days](#Days) | Vordefinierte zweistufige Zeitachse, bei der die minimale Detailstufe ein Tag beträgt. |
| [DefinedInView](#DefinedInView) | Verwenden Sie die in den Eigenschaften der Projektansicht definierten Zeitskalen‑Einstellungen: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). |
| [Months](#Months) | Vordefinierte zweistufige Zeitachse, bei der die minimale Detailstufe ein Monat beträgt. |
| [ThirdsOfMonths](#ThirdsOfMonths) | Vordefinierte zweistufige Zeitachse, bei der die Detailstufe ein Drittel eines Monats beträgt. |
### Days {#Days}
```
public static final int Days
```


Vordefinierte zweistufige Zeitachse, bei der die minimale Detailstufe ein Tag beträgt.

### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


Verwenden Sie die in den Eigenschaften der Projektansicht definierten Zeitskalen‑Einstellungen: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). Gültig für Formate, die Ansichtsdaten enthalten. Zum Beispiel Projekte, die aus dem MPP‑Format gelesen werden.

--------------------

Wenn für die Ansicht keine Zeitskalen‑Einstellungen festgelegt sind, wird stattdessen die vordefinierte Einstellung Timescale.Days verwendet.

### Months {#Months}
```
public static final int Months
```


Vordefinierte zweistufige Zeitachse, bei der die minimale Detailstufe ein Monat beträgt.

### ThirdsOfMonths {#ThirdsOfMonths}
```
public static final int ThirdsOfMonths
```


Vordefinierte zweistufige Zeitachse, bei der die Detailstufe ein Drittel eines Monats beträgt.

