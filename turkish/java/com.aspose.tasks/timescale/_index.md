---
title: "Timescale"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Proje bir grafik formatına dışa aktarıldığında Gantt Şeması Görev Kullanımı veya Kaynak Kullanımı görünümlerinde zaman ölçeğinin nasıl render edileceğini belirten seçenekleri tanımlar."
type: docs
weight: 323
url: /tr/java/com.aspose.tasks/timescale/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class Timescale extends System.Enum
```

Proje grafik formata dışa aktarıldığında Gantt Şeması, Görev Kullanımı veya Kaynak Kullanımı görünümlerinde zaman ölçeğinin nasıl render edileceğini belirten seçenekleri tanımlar.
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [Days](#Days) | Minimum detay seviyesinin bir gün olduğu önceden tanımlanmış iki katmanlı zaman ölçeği. |
| [DefinedInView](#DefinedInView) | Proje görünümünün özelliklerinde tanımlanan zaman ölçeği ayarlarını kullan: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). |
| [Months](#Months) | Minimum detay seviyesinin bir ay olduğu önceden tanımlanmış iki katmanlı zaman ölçeği. |
| [ThirdsOfMonths](#ThirdsOfMonths) | Önceden tanımlı iki katmanlı zaman ölçeği, burada ayrıntı seviyesi ayın üçte biri olur. |
### Days {#Days}
```
public static final int Days
```


Minimum detay seviyesinin bir gün olduğu önceden tanımlanmış iki katmanlı zaman ölçeği.

### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


Proje görünümünün özelliklerinde tanımlı zaman ölçeği ayarlarını kullanın: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). Görünüm verisi içeren formatlar için geçerlidir. Örneğin, MPP formatından okunan projeler.

--------------------

Eğer görünüm için zaman ölçeği ayarları belirlenmemişse, önceden tanımlı Timescale.Days ayarı kullanılır.

### Months {#Months}
```
public static final int Months
```


Minimum detay seviyesinin bir ay olduğu önceden tanımlanmış iki katmanlı zaman ölçeği.

### ThirdsOfMonths {#ThirdsOfMonths}
```
public static final int ThirdsOfMonths
```


Önceden tanımlı iki katmanlı zaman ölçeği, burada ayrıntı seviyesi ayın üçte biri olur.

