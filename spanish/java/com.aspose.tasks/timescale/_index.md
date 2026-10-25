---
title: "Timescale"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Define opciones que especifican cómo renderizar la escala de tiempo en las vistas de Uso de tareas del diagrama de Gantt o Uso de recursos cuando el proyecto se exporta a un formato gráfico."
type: docs
weight: 323
url: /es/java/com.aspose.tasks/timescale/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class Timescale extends System.Enum
```

Define opciones que especifican cómo renderizar la escala de tiempo en vistas de Diagrama de Gantt, Uso de tareas o Uso de recursos cuando el proyecto se exporta a un formato gráfico.
## Campos

| Campo | Descripción |
| --- | --- |
| [Days](#Days) | Escala de tiempo de dos niveles predefinida donde el nivel mínimo de detalle es un día. |
| [DefinedInView](#DefinedInView) | Utilice la configuración de escala de tiempo definida en las propiedades de la vista del proyecto: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). |
| [Months](#Months) | Escala de tiempo de dos niveles predefinida donde el nivel mínimo de detalle es un mes. |
| [ThirdsOfMonths](#ThirdsOfMonths) | Escala de tiempo predefinida de dos niveles donde el nivel de detalle es un tercio del mes. |
### Days {#Days}
```
public static final int Days
```


Escala de tiempo de dos niveles predefinida donde el nivel mínimo de detalle es un día.

### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


Utilice la configuración de escala de tiempo definida en las propiedades de la vista del proyecto: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). Válido para formatos que contienen datos de vista. Por ejemplo, proyectos que se leen del formato MPP.

--------------------

Si la configuración de escala de tiempo no está establecida para la vista, se utiliza la configuración predefinida Timescale.Days.

### Months {#Months}
```
public static final int Months
```


Escala de tiempo de dos niveles predefinida donde el nivel mínimo de detalle es un mes.

### ThirdsOfMonths {#ThirdsOfMonths}
```
public static final int ThirdsOfMonths
```


Escala de tiempo predefinida de dos niveles donde el nivel de detalle es un tercio del mes.

