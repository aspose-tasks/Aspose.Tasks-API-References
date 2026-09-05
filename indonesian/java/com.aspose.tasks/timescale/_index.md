---
title: "Timescale"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mendefinisikan opsi yang menentukan cara merender skala waktu dalam tampilan Penggunaan Tugas Gantt Chart atau Penggunaan Sumber Daya ketika proyek diekspor ke format grafis."
type: docs
weight: 323
url: /id/java/com.aspose.tasks/timescale/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class Timescale extends System.Enum
```

Mendefinisikan opsi yang menentukan cara merender skala waktu dalam tampilan Gantt Chart, Task Usage, atau Resource Usage ketika proyek diekspor ke format grafis.
## Bidang

| Bidang | Deskripsi |
| --- | --- |
| [Days](#Days) | Skala waktu dua tingkat yang telah ditentukan sebelumnya dimana tingkat detail minimal adalah satu hari. |
| [DefinedInView](#DefinedInView) | Gunakan pengaturan skala waktu yang didefinisikan dalam properti tampilan proyek: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). |
| [Months](#Months) | Skala waktu dua tingkat yang telah ditentukan sebelumnya dimana tingkat detail minimal adalah satu bulan. |
| [ThirdsOfMonths](#ThirdsOfMonths) | Skala waktu dua tingkat yang telah ditentukan di mana tingkat detailnya adalah sepertiga bulan. |
### Days {#Days}
```
public static final int Days
```


Skala waktu dua tingkat yang telah ditentukan sebelumnya dimana tingkat detail minimal adalah satu hari.

### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


Gunakan pengaturan skala waktu yang didefinisikan dalam properti tampilan proyek: `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). Berlaku untuk format yang berisi data tampilan. Misalnya, proyek yang dibaca dari format MPP.

--------------------

Jika pengaturan skala waktu tidak diatur untuk tampilan, pengaturan Timescale.Days yang telah ditentukan akan digunakan sebagai gantinya.

### Months {#Months}
```
public static final int Months
```


Skala waktu dua tingkat yang telah ditentukan sebelumnya dimana tingkat detail minimal adalah satu bulan.

### ThirdsOfMonths {#ThirdsOfMonths}
```
public static final int ThirdsOfMonths
```


Skala waktu dua tingkat yang telah ditentukan di mana tingkat detailnya adalah sepertiga bulan.

