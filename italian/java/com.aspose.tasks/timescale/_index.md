---
title: "Timescale"
second_title: "Aspose.Tasks for Java API Reference"
description: "Definisce le opzioni che specificano come renderizzare la scala temporale nei diagrammi Gantt di utilizzo attività o utilizzo risorse quando il progetto è esportato in un formato grafico."
type: docs
weight: 323
url: /it/java/com.aspose.tasks/timescale/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class Timescale extends System.Enum
```

Definisce le opzioni che specificano come renderizzare la scala temporale nei diagrammi Gantt, nelle visualizzazioni Utilizzo attività o Utilizzo risorse quando il progetto viene esportato in un formato grafico.
## Campi

| Campo | Descrizione |
| --- | --- |
| [Days](#Days) | Scala temporale a due livelli predefinita dove il livello minimo di dettaglio è un giorno. |
| [DefinedInView](#DefinedInView) | Utilizza le impostazioni della scala temporale definite nelle proprietà della vista di progetto: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). |
| [Months](#Months) | Scala temporale a due livelli predefinita dove il livello minimo di dettaglio è un mese. |
| [ThirdsOfMonths](#ThirdsOfMonths) | Scala temporale predefinita a due livelli in cui il livello di dettaglio è un terzo del mese. |
### Days {#Days}
```
public static final int Days
```


Scala temporale a due livelli predefinita dove il livello minimo di dettaglio è un giorno.

### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


Utilizza le impostazioni della scala temporale definite nelle proprietà della vista del progetto: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). Valido per i formati che contengono dati di vista. Ad esempio, progetti letti dal formato MPP.

--------------------

Se le impostazioni della scala temporale non sono impostate per la vista, viene utilizzata invece l'impostazione predefinita Timescale.Days.

### Months {#Months}
```
public static final int Months
```


Scala temporale a due livelli predefinita dove il livello minimo di dettaglio è un mese.

### ThirdsOfMonths {#ThirdsOfMonths}
```
public static final int ThirdsOfMonths
```


Scala temporale predefinita a due livelli in cui il livello di dettaglio è un terzo del mese.

